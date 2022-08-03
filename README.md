# PROJETO - FONTE REGULADORA DE TENSÃO
 Este projeto, realizado para a disciplina de [SSC0180 - Eletrônica para Computação](https://gitlab.com/simoesusp/disciplinas/-/tree/master/SSC0180-Eletronica-para-Computacao#passarinho-experto-a-prova-de-recupera%C3%A7%C3%A3o-ser%C3%A1-explicar-o-que-aconteceu) ministrada pelo professor Eduardo do Valle Simoes no ICMC-USP, tem por objetivo apresentar as etapas de eleaboração de uma fonte de tensão ajustável de 3v à 12v e que possui capacidade de 100mA.

## Tabela de Componentes

| Quantidade |        Componente        |         Preço        |
|------------|--------------------------|----------------------|
|      4     | Diodo Retificador 1N4007 |  R$0,20 x 4 = R$0,80 |
|      1     |      Capacitor 470uF     |        R$1,05        |
|      1     |  LED 5mm Vermelho Difuso |        R$0,50        |
|      3     |       Resistor 1k        |  R$0,07 x 3 = R$0,21 |
|      2     |       Resistor 2.2k      |  R$0,07 x 2 = R$0,14 |
|      1     |       Resistor 120       |        R$0,07        |
|      1     |    Potenciômetro 10k     |        R$7,00        |
|      1     |  Diodo Zener 13v 1N4743  |        R$0,48        |
|      1     |   Transistor NPN BC337   |        R$0,69        |
|   Total    |                          |       R$10,94        |

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

## Etapas da fonte

## Transformação

![50](https://user-images.githubusercontent.com/102570129/182647829-498c49b5-bd4e-4a82-8535-ebc7b4c46b57.png)


Na etapa de transformação é utilizado o transformador para reduzir a diferença de potencial elétrico. A fonte de corrente alternada, que no caso é uma tomada comum de 127 Volts é reduzida para um valor que é mais apropriado para o circuito e garante uma fonte estável, no projeto foi usado um transformador de 24 Volts.
Com os cálculos, podemos perceber que a tensão elétrica máxima dessa fonte é 127 vezes raiz de 2 = 179,6 Volts e a tensão de pico é 24 vezes raiz de 2 = 33,94 Volts.

## Retificação

![05-1](https://user-images.githubusercontent.com/102570129/182647906-8cb85a5f-d465-4933-b308-4492c8417ad3.png)

![img fonte](https://user-images.githubusercontent.com/102570129/182648392-18a7fe21-a47d-4b28-90e4-2390da4d11ae.png)


Na etapa de retificação ocorre a conversão de energia alternada para a contínua, é composta por uma ponte de diodos e permite o aproveitamento dos dois semiciclos da tensão de alimentação da carga, esse processo é denominado como retificação de onda completa.
Cada diodo utilizado consome 0,7 Volts de tensão, utilizando 24 Volts no circuito, temos os cálculos de tensão elétrica do diodo máximo, quando a corrente passa por um diodo há uma queda de 0,7 Volts, no circuito passa por dois diodos ao mesmo tempo resultando em 1,4 Volts. 

## Filtragem

![06-1](https://user-images.githubusercontent.com/102570129/182648050-cb2a3c4d-8795-4525-97da-a63ab330a7d7.png)


![02-2](https://user-images.githubusercontent.com/102570129/182648230-3c3e029e-27b5-42f1-b4c9-22b27d90f328.png)

Na etapa de filtragem é utilizado o capacitor para fazer com que o sinal pulsante fique o mais próximo possível de um sinal linear de corrente contínua, a função do capacitor nessa etapa é liberar corrente quando a tensão elétrica interna é menor que a tensão da sua própria estrutura, fazendo com que ocorra uma diminuição no valor do Ripple. E quanto menor o Ripple melhor é a fonte de alimentação. Para os cálculos foi determinado em até 10%.

## Regulação

![07_02](https://user-images.githubusercontent.com/102570129/182648294-16f2c754-ea98-46bb-bd60-a41323ccda33.png)

A última etapa é a regulação onde deve-se tornar o máximo possível a saída da fonte na tensão de forma linear, com isso é possível estabilizar variações na corrente e temperaturas por mais estáveis que sejam na entrada do regulador. Nessa etapa é utilizado o diodo zener e quando está polarizado diretamente, funciona como outro diodo qualquer, não conduz corrente elétrica enquanto a tensão aplicada aos seus terminais for acima de 13V. 
Sendo assim, o resistor tem a função de determinar a corrente que passará pelo diodo zener e por ser uma fonte de tensão ajustável o potenciômetro controla a tensão através da queda de potencial conforme o valor de saída determinada.


## Circuito no Falstad
Clique [aqui](https://tinyurl.com/23vrahcq) para acessar o simulador do circuito.
![image](https://user-images.githubusercontent.com/110194295/182157687-5cb9467f-244c-4408-8ff7-5a813cbcbaed.png)

## Circuito no Eagle
#### ESQUEMÁTICO
![image](https://user-images.githubusercontent.com/110194295/182173824-c7ec1ec5-741a-4eab-8ed7-2a1ab1dd1761.png)

#### PCB
![image](https://user-images.githubusercontent.com/110194295/182181389-09cfb162-e1af-4029-b0ba-90f598b5cfde.png)

##### PCB - PARTE INFERIOR DA PLACA (visto de baixo/espelhado)
![image](https://user-images.githubusercontent.com/110194295/182032220-3c0c380b-916b-4055-a38d-6e59ba4621fd.png)

## Cálculos

                                       | Cálculos tensão elétrica |
                                       |--------------------------|


![image](https://user-images.githubusercontent.com/110194295/182062733-424f7300-8b65-4b87-83dc-28815466f454.png)

![correçao1](https://user-images.githubusercontent.com/102570129/182645445-a0bc7136-9196-4aba-b2fd-37c9a6d67a20.png)

![correçao2](https://user-images.githubusercontent.com/102570129/182645498-8666deb6-4a51-41b4-804e-1b9fd9844ed8.png)

-------------------------------------- Cálculos corrente elétrica ----------------------------------



![correçao3](https://user-images.githubusercontent.com/102570129/182645540-ae68d785-2402-482f-bf11-2a388a639ba0.png)

![correçao4](https://user-images.githubusercontent.com/102570129/182645567-35f9d6b9-abaa-4fad-85dd-cbb62803d1d3.png)

![correçao5](https://user-images.githubusercontent.com/102570129/182645603-1f6eed02-96bf-43e5-93b3-63c2d180e6b1.png)

![correçao6](https://user-images.githubusercontent.com/102570129/182645636-b52ea0f1-13f8-499d-982d-ebd3d6a2e3e5.png)

---------------------------------------- Cálculos capacitor ----------------------------------------



![correçao7](https://user-images.githubusercontent.com/102570129/182645663-e01d93fc-bd28-4830-bbb5-8153c0994bd4.png)


## Imagens da Protoboard com o Circuito Montado
<a href="url"><img src="https://user-images.githubusercontent.com/102570129/182054968-985940d6-9b80-48c1-acee-eb616a9a944a.jpg" align="left" height="600" width="400" ></a>

<a href="url"><img src="https://user-images.githubusercontent.com/102570129/182055083-e05aca17-5829-42e1-b606-c6084b62087b.jpg" height="600" width="400" ></a>

<a href="url"><img src="https://user-images.githubusercontent.com/102570129/182055172-47f3e9c4-d8d2-430d-a495-0fe2998bde1b.jpg" height="600" width="400" ></a>

![20220731_190105](https://user-images.githubusercontent.com/102570129/182055705-d1603daa-b353-4b3b-9344-5467e9f531fc.jpg)

## Vídeo Explicativo
![image](https://user-images.githubusercontent.com/110194295/182183682-81e2761e-01ba-4ab8-a5a4-055e92e36033.png)

Clique [aqui](https://www.youtube.com/watch?v=eEh-RMIG-vI) para assistir ao vídeo explicativo acerca dos cálculos feitos para a elaboração do projeto e do circuito no Falstad, bem como para ver a fonte em funcionamento.

## Grupo
  - [Bruna Romero Arraes](https://github.com/bruromero)
  - [Bruno Santos de Sousa](https://github.com/brunox-sousa)
  - [Johana J. Pizarro Laquise](https://github.com/JohanaPizarroL)
  - [Livia Rosito Reis dos Santos](https://github.com/liviarosito)
