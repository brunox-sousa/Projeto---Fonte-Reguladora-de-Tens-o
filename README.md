# PROJETO - FONTE REGULADORA DE TENSÃO
 Este projeto, realizado para a disciplina de [SSC0180 - Eletrônica para Computação](https://gitlab.com/simoesusp/disciplinas/-/tree/master/SSC0180-Eletronica-para-Computacao#passarinho-experto-a-prova-de-recupera%C3%A7%C3%A3o-ser%C3%A1-explicar-o-que-aconteceu) ministrada pelo professor Eduardo do Valle Simoes no ICMC-USP, tem por objetivo apresentar as etapas de eleaboração de uma fonte de tensão ajustável de 3v à 12v e que possui capacidade de 100mA.

## Tabela de Componentes

| Quantidade |        Componente        |         Preço        |
|------------|--------------------------|----------------------|
|      4     | Diodo Retificador 1N4007 |  R$0,20 x 4 = R$0,80 |
|      1     |    Capacitor 560uF/25v   |        R$1,05        |
|      1     |  LED 5mm Vermelho Difuso |        R$0,50        |
|     10     |       Resistor 1k        | R$0,07 x 10 = R$0,70 |
|     10     |       Resistor 2.2k      | R$0,07 x 10 = R$0,70 |
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
![image](https://user-images.githubusercontent.com/110194295/182062733-424f7300-8b65-4b87-83dc-28815466f454.png)

![image](https://user-images.githubusercontent.com/110194295/182062795-dbb1f197-3781-4426-8972-95e1a8302b59.png)

![image](https://user-images.githubusercontent.com/110194295/182062844-801c1442-2378-4a80-b296-a1b4dfeb2987.png)

![image](https://user-images.githubusercontent.com/110194295/182062882-c6d2f7b5-be3c-444d-9eeb-636303889e4d.png)

![image](https://user-images.githubusercontent.com/110194295/182062938-5bca1e00-affa-4714-a9d4-b5c86aca256e.png)

![image](https://user-images.githubusercontent.com/110194295/182062960-e11ce317-69ef-482b-a0a4-4e72ffa0e95e.png)

![image](https://user-images.githubusercontent.com/110194295/182063082-70365d61-22fe-4733-8033-bd3c659df753.png)

![image](https://user-images.githubusercontent.com/110194295/182063142-ee391f97-7702-45a4-a69b-a15086605860.png)

## Imagens da Protoboard com o Circuito Montado
<a href="url"><img src="https://user-images.githubusercontent.com/102570129/182054968-985940d6-9b80-48c1-acee-eb616a9a944a.jpg" align="left" height="600" width="400" ></a>
<a href="url"><img src="https://user-images.githubusercontent.com/102570129/182055083-e05aca17-5829-42e1-b606-c6084b62087b.jpg" height="600" width="400" ></a>  
<a href="url"><img src="https://user-images.githubusercontent.com/102570129/182055172-47f3e9c4-d8d2-430d-a495-0fe2998bde1b.jpg" height="600" width="400" ></a>
![20220731_190105](https://user-images.githubusercontent.com/102570129/182055705-d1603daa-b353-4b3b-9344-5467e9f531fc.jpg)

## Vídeo Explicativo
Clique [aqui] para assistir ao vídeo explicativo acerca dos cálculos feitos para a elaboração do projeto e do circuito no Falstad, bem como para ver a fonte em funcionamento.

## Grupo
  - [Bruna Romero Arraes](https://github.com/bruromero)
  - [Bruno Santos de Sousa](https://github.com/brunox-sousa)
  - [Johana J. Pizarro Laquise](https://github.com/JohanaPizarroL)
  - [Livia Rosito Reis dos Santos](https://github.com/liviarosito)
