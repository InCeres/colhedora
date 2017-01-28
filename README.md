# Colheitadeira

## Objetivos

O principal objetivo desse teste é entender o seu mindset e como vc busca solucionar problemas complexos com restrições definidas.

Queremos ver qualquer código, mesmo que não esteja atendendo 100% do problema.

## Descrição

Nesse desafio, o objetivo é criar um arquivo com o resultado da colheita de uma área. Para isso, o software precisa ler do sensor de colheita e registrar a quantidade colhida para aquela área.

Nossa colheitadeira possui módulos de colheita com larguras variáveis. A mais comum possui uma largura de 10 metros. Além disso, o sensor de acumula o resultado da colheita e libera esse valor a cada 10 metros percorridos pela colheitadeira fechando assim a área mínima de registro.

O arquivo de saída do software deve contar a lista das coordenadas geográficas dos centros das áreas mínimas e o valor colhido nessa área no seguinte formato:

    [
        {"lat": 43.998778,"lng": 22.887686,"value": 46.45},        
        {"lat": 43.000322,"lng": 22.887686,"value": 44.23},        
    ]
    
## Regras

O sinal do GPS e a saída do sensor de colheitas devem ser simulados pela solução de qualquer maneira possível.

A área de colheita é um polígono de 4 lados e estão definidos pelas coordenadas geográficas passadas.

A colheitadeira inicia o seu trabalho no canto superior esquerdo da área. Ao chegar no limte da área de colheita, ela seguirá no sentido oposto, uma faixa abaixo, seguindo assim até o final da área 

Será fornecido um desenho representando a área de colheita.

A simulação do sensor de colheita deve estar dentro do intervalo de cada curva de valor no desenho da área, sendo que as coordenadas que delimitam cada área também estão especificadas no desenho abaixo. Ou seja, se a colheitadeira estiver dentro de uma área cujo o intervalo está definido como 30-60 isso quer dizer que o valor da simulação colhida naquele quadrado deve ser um número qualquer entre 30 e 60.

## Considerações

Deve ser feito em Python e/ou Javascript.

Faça testes unitários. Testes funcionais é um bônus.

Use o Gitlab, crie sua conta caso não tenha, faça fork desse projeto e depois pe

É possível usar qualquer lib externa que ajude a resolver o problema. Existem algorítmos prontos na internet para isso. Por favor, não os use. Precisamos que vc desenvolva seu próprio algorítmo.

Você deve usar 100% OOP para esse desafio.

O projeto deve ser entregue com todas as instruções para ser instalado e executado.

É necessário fornecer algum tipo de feedback para indicar que a colheita está acontecendo.

A velocidade da colheitadeira não faz parte do problema.

