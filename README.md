# PROJETO - FONTE REGULADORA DE TENSÃO
 Este projeto, realizado para a disciplina de [SSC0180 - Eletrônica para Computação](https://gitlab.com/simoesusp/disciplinas/-/tree/master/SSC0180-Eletronica-para-Computacao#passarinho-experto-a-prova-de-recupera%C3%A7%C3%A3o-ser%C3%A1-explicar-o-que-aconteceu) ministrada pelo professor Eduardo do Valle Simoes no ICMC-USP, tem por objetivo apresentar as etapas de eleaboração de uma fonte de tensão ajustável de 3v à 12v e que possui capacidade de 100mA.

## Tabela de Componentes

| Quantidade |        Componente        |         Preço        |
|------------|--------------------------|----------------------|
|      4     | Diodo Retificador 1N4007 |  R$0,20 x 4 = R$0,80 |
|      1     |    Capacitor 560uF/25v   |       R$00,00        |
|      1     |  LED 5mm Vermelho Difuso |        R$0,50        |
|     10     |       Resistor 1k        | R$0,07 x 10 = R$0,70 |
|     10     |       Resistor 2k        | R$0,07 x 10 = R$0,70 |
|     10     |       Resistor 120       | R$0,07 x 10 = R$0,70 |
|      1     |      Potenciômetro       |        R$7,00        |
|      1     |  Diodo Zener 13v 1N4743  |        R$0,48        |
|      1     |   Transistor NPN BC337   |        R$0,69        |
|   Total    |                          |       R$00,00        |

## Componentes - Funções
### Ponte de Diodo Retificador:
Elaborada a partir de quatro diodos, essa estrutura funciona como um circuito que converte uma corrente alternada (valor da tensão varia entre positivo e negativo) em corrente contínua (valor da tensão se mantém positivo), de modo a torná-la útil para o funcionamento de diferentes aparelhos;
### Capacitor:
Dispositivo cuja principal função consiste em armazenar cargas elétricas, de maneira a armazenar elétrons quando a tensão sobe e liberá-los para o restante do circuito quando a tensão desce (libera corrente quando a tensão interna é menor que a tensão da sua própria estrutura). Esse processo auxilia na diminuição da taxa de ripple;
###LED:
Auxilia no funcionamento do circuito - indica se a fonte a fonte está ligada;
### Resistores:
Limitam a passagem (intensidade) de corrente elétrica a fim de evitar a danificação dos componentes do circuito;
### Potenciômetro:
Permite a variação do valor resistivo pelo movimento de um eixo, possibilitando o ajuste do controle da tensão dentro do circuito entre 3V e 12V;
### Diodo Zener:
Utilizado no ajuste de tensão de ruptura do circuito.  Quando está polarizado diretamente, funciona como outro diodo qualquer, ou seja, não conduz corrente elétrica enquanto a tensão aplicada aos seus terminais for acima de 13V;
### Transistor:
Utilizado para amplificar ou atenuar a intensidade da corrente elétrica em circuitos.

## Circuito no Falstad
Clique [aqui] para acessar o simulador do circuito.

## Circuito no Eagle
#### ESQUEMÁTICO
![image](https://user-images.githubusercontent.com/110194295/182027842-3a6b480c-c10b-42d0-bb2b-19c50572bc6b.png)

#### PCB
![image](https://user-images.githubusercontent.com/110194295/182030894-70d9658b-b65b-4af7-95b9-fdeca1006a37.png)

##### PCB - PARTE INFERIOR DA PLACA (visto de baixo/espelhado)
![image](https://user-images.githubusercontent.com/110194295/182032220-3c0c380b-916b-4055-a38d-6e59ba4621fd.png)

## Cálculos

## Imagens da Protoboard com o Circuito Montado

## Vídeo Explicativo
Clique [aqui] para assistir ao vídeo explicativo acerca dos cálculos feitos para a elaboração do projeto e do circuito no Falstad, bem como para ver a fonte em funcionamento.

## Grupo
  - [Bruna Romero Arraes](https://github.com/bruromero)
  - [Bruno Santos de Sousa](https://github.com/brunox-sousa)
  - [Johana J. Pizarro Laquise](https://github.com/JohanaPizarroL)
  - [Livia Rosito Reis dos Santos](https://github.com/liviarosito)
