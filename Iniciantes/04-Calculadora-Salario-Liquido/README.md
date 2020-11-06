# Calculadora de salário líquido
Uma das coisas que quem trabalha como CLT quer saber. Quanto vou receber líquido do meu salário?

## Como funciona
Vamos fazer o calculo do salário com os descontos de INSS e IRPF.

Para isso, precisamos saber calcular cada imposto desse para subtrair do salário.

Os valores para cálculo de cada imposto varia de acordo com o valor do salário bruto. Vamos ver a tabela de desconto e faixas de valores:

| Salário | Alíquota | Parcela` a deduzir |
| --- | --- | --- |
| R$ 1.045,00	| 7,5% | 0 |
| De R$ 1.045,01 a R$ 2.089,60 | 9% | 15,67 |
| De R$ 2.089,61 a R$ 3.134,40 | 12% | 78,36 |
| De R$ 3.134,41 a R$ 6.101,06 | 14% | 141,05 |
| Acima de 6.101,06 | desconto fixo de 713.10 | - |


A fórmula para saber o valor do INSS é a seguinte: 
```
DESCONTO_INSS = (SALÁRIO_BRUTO x ALÍQUOTA) - PARCELA_A_DEDUZIR
```

Assim sabemos o valor do desconto, INSS. Com esse valor em mãos, basta subtrair ele do salário bruto!

Exemplo:
```
SALÁRIO_SEM_INSS = SALÁRIO_BRUTO - DESCONTO_INSS;
```

Lembrando que, caso o salário bruto supere o valor de `6.101,06`, então deve ser descontado apenas o valor fixo. Exemplo:

```
SALÁRIO_SEM_INSS = SALÁRIO_BRUTO - 713.10
```

É com o valor do salário já descontado o INSS que fazemos o cálculo do imposto IRPF

| Salário sem INSS | Alíquota | Parcela a deduzir |
| --- | --- | --- |
| Até 1.903,98	| ISENTO | 0 |
| De R$ 1.903,99 até R$ 2.86,65 |	7,5% | 142,80 |
| De R$ 2.826,66 até R$ 3.751,05 | 15% |	354,80 |
| De R$ 3.751,06 até R$ 4.664,68 |	22,5% |	636,13 |
| Acima de R$ 4.664,68 | 27,5% | 869,36 |



O cálculo do IRPF é praticamente o mesmo do salário líquido:
```
DESCONTO_IRPF = (SALÁRIO_SEM_INSS * ALÍQUOTA) - PARCELA_A_DEDUZIR
```

Com o valor do IRPF em mãos. O salário líquido fica:

```
SALÁRIO_LÍQUIDO = SALÁRIO_BRUTO - DESCONTO_INSS - DESCONTO_IRPF
```

## Proposta
- Criar interface para capturar o salário bruto
- botão para disparar ação de calcular
- Mostrar na interface o salário líquido

## Dicas/Lembretes

Esse é um desafio com muitos resultados diferentes.

Mais uma vez, lembre de quebrar em pequenas tarefas. Basicamente você vai fazer 4 etapas macro:
- Capturar informação do salário bruto
- Calcular INSS
- Calcular IRPF
- Apresentar resultado com os descontos