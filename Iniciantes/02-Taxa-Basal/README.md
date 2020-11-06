# Taxa Metabólica Basal (TMB)
A taxa metabólica basal pode ser entendida como a energia mínima que o corpo necessita para manter seu funcionamento. 

Obs: É claro que o cálculo que vamos é básico. As necessidades mínimas de um indivíduo deve ser preescrito por um profissional, já que tem muitas outras variáveis para levar em consideração.

## Como funciona
Para calcular a TMB, precisamos coletar algumas informações do usuário:
- Sexo
- Peso
- Altura em cm
- Idade

O fórmula é diferente para cada sexo.

Homens:
```
TMB = 66,5 + (13,75 x PESO) + (5,0 x ALTURA_EM_CM) – (6,8 x IDADE).
``` 

Mulheres:
```
TMB = 665,1 + (9,56 x PESO) + (1,8 x ALTURA_EM_CM – (4,7 x IDADE).
```

O resultado da fórmula aplicado para cada indivíduo do sexo correspondente é a quantidade mínima de calorias diária que a pessoa precisa consumir para manter o seu corpo em bom funcionamento

## Proposta
- Crie um pequeno formulário para capturar os dados do usuário que necessitam para o cálculo
- Crie o botão que vai disparar a ação que gera o resultado
- Apresente visualmente o resultado, ex: Você precisa de 1550,00 calorias diária

## Dica/Lembrete

- Quebre o desafio em micro tarefas e vá resolvendo uma a uma
- Com as tarefas resolvidas, integre elas (Ex: cálculo homem + cálculo mulher + captura de informações + verifica sexo)

