# Colhedora

## Objetivo

O objetivo principal deste teste é descobrir como você pensa. Queremos entender como você busca solucionar problemas complexos, com restrições definidas.

Mesmo que não consiga completar 100% o desafio, envie o seu código, queremos vê-lo mesmo assim. 


## Descrição

Neste desafio, o objetivo é criar um arquivo com o resultado da colheita de uma área. Para isso, o software precisa ler do sensor de colheita e registrar a quantidade colhida para aquela área.

Cada modelo de colheitadera possui uma largura diferente em que colhe uma plantação, como indica na figura abaixo. Porém, a mais comum possui é a de 10 metros. Além disso, o sensor acumula o resultado da colheita e libera esse valor a cada 10 metros percorridos pela colheitadeira fechando assim a área mínima de registro. Neste caso 10m x 10m.

![](h_colhedora5_762x458.jpg)

O arquivo de saída do software deve conter a lista das coordenadas geográficas dos centros das áreas mínimas e o valor colhido nessa área no seguinte formato:

```json
[
    {"lat": -22.550718, ,"lng": -47.720137,"value": 7.89},
    {"lat": -22.550581,"lng": -47.719979,"value": 10.76},
    {"lat": -22.550447 ,"lng": -47.719781,"value": 13.9}
]
```
    
## Regras

1. O sinal do GPS e a saída do sensor de colheitas devem ser simulados usando qualquer recurso de software que você quiser.

2. A área de colheita é um polígono de 4 lados e estão definidos pelas coordenadas geográficas passadas na seção Dados.

3. A colhedora inicia o seu trabalho no canto superior esquerdo da área (ponto A) e deve seguir em direção ao canto superior direito (ponto B). Ao chegar no limte da área de colheita, ela seguirá no sentido oposto, uma faixa abaixo, seguindo assim até o final da área.

4. A simulação do sensor de colheita deve estar dentro do intervalo de cada curva de valor no desenho da área, sendo que as coordenadas que delimitam cada área também estão especificadas no desenho abaixo. Ou seja, se a colhedora estiver dentro de uma área cujo o intervalo está definido como 30-60 isso quer dizer que o valor da simulação colhida naquele quadrado deve ser um número qualquer entre 30 e 60.

## Dados

### Imagem

Essa imagem está no arquivo `desafio-inceres-colhedora.png` nessa pasta.

![](desafio-inceres-colhedora.png)


### Coordenadas da área de colheita

#### Área Amarela

* Ponto A: **22° 33' 2.686" S** - **47° 43' 13.134" W**
* Ponto B: **22° 32' 44.243" S** - **47° 42' 48.881" W**
* Ponto C: **22° 32' 58.938" S** - **47° 42' 44.014" W**
* Ponto D: **22° 33' 13.421" S** - **47° 43' 3.094" W**

#### Área Laranja

* Ponto A1: **22° 33' 2.970" S** - **47° 43' 7.496" W**
* Ponto B1: **22° 32' 52.591" S** - **47° 42' 56.142" W**
* Ponto C1: **22° 32' 57.941" S** - **47° 42' 48.647" W**
* Ponto D1: **22° 33' 7.787" S**  - **47° 42' 59.926" W**

#### Área Vermelha SW

* Ponto A2: **22° 33' 2.722" S** - **47° 43' 5.218" W**
* Ponto B2: **22° 32' 59.010" S** - **47° 43' 1.009" W**
* Ponto C2: **22° 33' 2.686" S** - **47° 42' 55.908" W**
* Ponto D2: **22° 33' 5.537" S** - **47° 43' 0.930" W**

#### Área Vermelha NE

* Ponto A3: **22° 32' 57.264" S** - **47° 42' 58.187" W**
* Ponto B3: **22° 32' 54.982" S** - **47° 42' 55.872" W**
* Ponto C3: **22° 32' 58.117" S** - **47° 42' 50.386" W**
* Ponto D3: **22° 33' 0.936" S** - **47° 42' 53.438" W**

### Intervalos de valores de colheita

* Área amarela: **5-15**
* Área laranja: **15-30**
* Área vermelha SW: **30-45**
* Área vermelha NE: **30-60**

## Considerações

* Deve ser feito em Python e/ou Javascript;
* Faça testes unitários. Testes funcionais é um bônus;
* Use o Gitlab, crie sua conta caso não tenha, faça fork desse projeto e torne ele privado (é de graça no GitLab). Adicione o nosso usuário (inceres-team) como membro do projeto para acompanharmos. Quando pronto, nos avise que iremos fazer nosso code review. Seus commits também serão analisados. É uma boa forma de ver seu fluxo de pensamento;
* Você tem 7 dias para terminar o teste;
* É possível usar qualquer lib externa que ajude a resolver o problema. Existem algorítmos prontos na internet para isso. Por favor, não os use. Precisamos que você desenvolva seu próprio algorítmo;
* Você deve usar 100% OOP para esse desafio. Mostre que você gosta de Design Patterns; :sunglasses:
* O projeto deve ser entregue com todas as instruções para ser instalado e executado;
* É necessário fornecer algum tipo de feedback para indicar que a colheita está acontecendo;
* A velocidade da colhedora não faz parte do problema, mas fique a vontade para criar. Representar a colhedora se movendo no OpenLayers é um grande bônus. :wink:

## Bom código e divirta-se!

:tractor:
