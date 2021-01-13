# Projeto

## Descrição

O projeto consiste no desenvolvimento de um modelo para detecção de comportamentos do gado leiteiro 
por meio de dados de sensores (acelerômetro, giroscópio, magnetômetro e GPS) embutidos em uma coleira.

Comportamentos como andando, ócio, pastando e ruminando são interessantes para otimização de recursos
no manejo dos animais. Dentre tais informações de comportamento, é possível destacar a ruminação do 
animal na detecção de doenças e no cio. Portanto, monitorar os comportamentos dos animais é uma tarefa
muito importante para ajudar o produtor numa melhor tomada de decisão.

## Base de Dados

A base utilizada foi criada mediante uma parceria realizada pela UFMS e a Embrapa.

Dados dos experimentos:

* 2 períodos: 1º experimento foi realizado no período de 25/03/15 a 30/03/15. O 2º de 06/04/15 a 09/04/15
* 4 animais (3 distintos)
* Foram utilizadas 4 coleiras (A, B, C e D). Entretanto, houve algumas falhas durante o experimento e, no final, ficaram as seguintes bases:
  - A2 e A3
  - B2 e B3
  - C3 e C4
  - D1, D2, D3 e D4
* Dispositivo: coleira
* Sensores: acelerômetro, giroscópio, magnetômetro e GPS
* Classes de comportamentos: pastar, em pé, deitado e andando

O arquivo embrapa.csv contém todos os dados aglutinados que foram utilizados. A estrutura do arquivo foi definida da seguinte forma:

IdColar | AccX | AccY | AccZ | MagX | MagY | MagZ | GirX | GirY | GirZ | Horario | Data | VelocidadeDeslocamento | Comportamento 
 --- | --- | --- |--- |--- |--- |--- |--- |--- |--- |--- |---|---|---
A2 | -11889 | 11184 | -17877 | -1280 | -73 | -309 | -4013 | 1260 | -31 | 131911.203 | 250515 | 000.0 | Comendo/Procurando
A2 | -9144 | 8945 | -11799 | -1213 | 707 | -238 | -394 | 2278 | -602 | 131949.203 | 250515 | 000.0 | Comendo/Procurando
A2 | 6391 | 9265 | -11767 | 570 | -405 | -1533 | -1072 | -1094 | 1854 | 132148.203 | 250515 | 000.0 | EmPe
A2 | -1394 | 10206 | -13229 | 671 | -73 | -1590 | 287 | 2253 | -2760 | 132151.203 | 250515 | 000.0 | Comendo/Procurando
...| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... 
D4 | 2152 | 7619 | -7736 | -1650 | 788 | 43 | -2980 | 3678 | -1357 | 122529.111 | 040715 | 000.0 | Comendo/Procurando

No total há 13088 amostras. A tabela a seguir mostra a segmentação das amostras por coleira

A2 | A3 | B2 | B3 | C3 | C4 | D1 | D2 | D3 | D4 | Total
--- | --- | --- |--- |--- |--- |--- |--- |--- |--- |--- | 
1112 | 2033 | 1131 | 1735 | 1852 | 406 | 1126 | 1690 | 1598 | 405 | 13088

