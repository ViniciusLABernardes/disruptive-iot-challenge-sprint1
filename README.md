# UWBike 
## Sistema de Mapeamento de Motos nos Pátios da Mottu com ESP32 + UWB

## O UWBike será um sistema de localização precisa de motos nos pátios da mottu. A ideia consiste em implantar 3 esp32 com uwb nos cantos do pátio, colocar etiquetas uwb nas motos e, quando a etiqueta da moto estiver ativa
## ela enviara sinais para os receptores(esp32) que pegaram no formato double a distancia da moto de cada receptor e enviaram para uma API JAVA
## A API então chama uma função responsável por calcular a posição exata da moto no pátio usando essas três distâncias e as coordenadas conhecidas das âncoras.
## Esse cálculo é feito através de um método chamado trilateração, que é uma técnica matemática usada para determinar uma posição no espaço a partir de três pontos de referência. A ideia é encontrar o ponto (x, y) que satisfaz as três distâncias medidas a partir das âncoras.

# Integrantes:
 - Vinicius Leandro de Araujo Bernardes RM554728 TURMA 2TDSPY
 - Edvan Davi Murilo Santos do Nascimento RM554733 TURMA 2TDSPZ
- Rafael Romanini de Oliveira RM554637 TURMA 2TDSPZ

## Procedimentos para rodar a simulação:
- ### Tenha uma conta no wokwi
- ### Instale as extensões Wokwi Simulator e PlatformIO IDE
- ### Rode os comandos no terminal dentro da pasta raiz do projeto:
- - pip install platformio
  - pio run -e ancora1
  - pio run -e ancora2
  - pio run -e ancora3
- ### Abra cada pasta ancora em uma janela diferente no vscode
- ### Abra a pagina index.html do projeto
 ### Pronto, agora você verá um dashboard trazendo as informações da distancia da moto(atualmente mockada) de cada âncora(atualmente simulada)
