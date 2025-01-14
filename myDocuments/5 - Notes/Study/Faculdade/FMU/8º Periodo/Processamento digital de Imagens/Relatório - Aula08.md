---
Index: "[[Processamento digital de Imagens]]"
---
Nome: João P S Oliveira / 2893577 - Eng da Computação

`import numpy as np` 
`import matplotlib.pyplot as plt` 
`%pip install scikit-image` 
`from skimage import io, transform, img_as_float`

1) Qual é a função das matrizes de transformação afim (como identidade, escala etc.) e como cada elemento da matriz afeta a imagem transformada? As matrizes de transformação afim são usadas para aplicar operações geométricas em imagens, como: • Identidade: Mantém a imagem inalterada. • Escala: Aumenta ou diminui o tamanho da imagem ao multiplicar as coordenadas por fatores específicos. • Rotação: Gira a imagem em torno de um ponto de origem usando ângulos em radianos. • Translação: Move a imagem de um ponto para outro sem alterar sua forma. Cada elemento da matriz afim define uma parte da transformação: • Os elementos na diagonal controlam o escalamento. • Os elementos fora da diagonal (para rotação e cisalhamento) ajustam a forma. • A última coluna geralmente define a translação (deslocamento). 2) Como a escolha das diferentes variáveis de transformação, como escalamento, rotação e translação, influencia o resultado final? Escalamento: Modifica o tamanho da imagem. Fatores maiores ampliam a imagem, enquanto menores reduzem. Rotação: Gira a imagem em torno de um ponto de referência. O ângulo determina o quanto a imagem é rotacionada. Translação: Move a imagem para uma nova posição. Valores maiores deslocam a imagem mais longe do ponto original. A combinação dessas variáveis pode deformar, mover ou ajustar o tamanho e orientação da imagem de forma significativa. 3) Principais Conclusões do Código O código aplica diferentes transformações afins a uma imagem usando funções predefinidas. Cada transformação (identidade, escala, rotação, translação, cisalhamento) altera a imagem de forma previsível e visualmente distinta. O uso de matrizes permite manipular facilmente as propriedades geométricas da imagem, ajustando seu tamanho, forma e posição.

