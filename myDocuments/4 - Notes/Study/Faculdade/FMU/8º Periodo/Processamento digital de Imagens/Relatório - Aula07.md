---
Index: "[[Processamento digital de Imagens]]"
---
1. A média das imagens combina os pixels, fazendo com que o ruído se cancele e a imagem fique mais limpa.
2. O código não vai funcionar, porque as imagens precisam ter o mesmo tamanho. Você precisaria redimensionar a imagem menor.
3. A imagem resultante ficará toda preta (pixels com valor zero), e isso não causa problemas.
4. O OpenCV transforma esses valores negativos em zero, então a área correspondente ficará preta na imagem.