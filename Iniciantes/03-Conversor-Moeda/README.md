# Conversor de moedas
Vamos criar um conversor de moedas onde é possível combinar qualquer uma e obter o valor convertido.

## Como funciona
Um conversor de moedas serve para saber o valor que uma moeda tem em relação a outra moeda internacional.

Exemplos:
- 1 Dólar vale R$5,53
- 35 dólares valem 29.58 euros
- 50 Libras esterlinas valem 65.77 dólares

Então, para realizar o calculo, precisamos:
- Capturar o valor da moeda de origem
- Capturar o tipo da moeda origem (dólar, euro, libra, real, etc.)
- Capturar o tipo da moeda destino (dólar, euro, libra, real, etc.)

Com os valores em mãos, aplicar o cálculo de conversão (pesquisa sobre como fazer esse cálculo)

OBS: Faça o programa de um jeito que possa converter combinando qualquer tipo de moeda origem e destino, mesmo que tenha umas 200 moedas diferentes

## Proposta
- Capture via interface os valores necessários (`input text` para o valor da moeda e `select` comos tipos de moeda)
- Deve vir com o valor 1 na moeda origem e o tipo dólar como padrão
- Deve vir como padrão o tipo da moeda destino como real e o seu valor já calculado com base em 1 dólar
- Ao digitar o valor da moeda origem ou trocar seu tipo, o valor da moeda destino deve ser automaticamente calculado e já preenchendo o resultado
- Realize o calculo
- Traga a resposta para o usuário


## Dica/Lembrete
- Mais uma vez, quebre em micro tarefas separado pelo que é entrada e dados, processamento no JavaScript e saída (resultado para o usuário)
  - Você pode primeiro deixar os dados marretados de moedas e valores e concentrar no calculo
  - Quando a função que calcula estiver certinho, você se concentra em capturar as informações
  - Capturando as informações e processando, você foca em mostrar o resultado
