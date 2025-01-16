---
Index: "[[Processamento digital de Sinais]]"
---
**Objetivo**: Explicar os fundamentos da compressão de sinais e como implementá-la para áudio, imagens e vídeo.

#### O que é Compressão?

A compressão reduz o tamanho dos dados de um sinal, facilitando o armazenamento e a transmissão. Existem dois tipos principais:

- **Compressão Lossless**: Nenhuma informação é perdida (ex.: FLAC, PNG).
- **Compressão Lossy**: Parte da informação é descartada para maior eficiência (ex.: MP3, JPEG).

#### Técnicas Comuns

- **Codificação Entropia**: Usa métodos como Huffman para compressão sem perdas.
- **Transformada e Quantização**: Aplica transformações (Fourier ou Wavelet) para descartar componentes de menor importância.

#### Exemplos de Compressão

- **Áudio**: MP3 usa transformadas e codificação perceptual.
- **Imagens**: JPEG comprime através da DCT (Transformada Discreta do Cosseno).
- **Vídeo**: Codecs como H.264 combinam compressão espacial e temporal.

#### Atividade Prática

1. Implementar compressão de imagem em Python usando a biblioteca PIL e comparar resultados com diferentes níveis de qualidade.
2. Experimentar a compactação de áudio com ferramentas disponíveis.