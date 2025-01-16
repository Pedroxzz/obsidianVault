---
Index: "[[Processamento digital de Sinais]]"
---
**Objetivo**: Introduzir o conceito de processamento multirresolução e demonstrar o uso da Transformada Wavelet em aplicações práticas.

#### Conceitos de Multirresolução

O processamento multirresolução permite analisar sinais em diferentes níveis de detalhe ou escalas, útil para sinais com características que variam no tempo e na frequência.

- **Análise no Domínio do Tempo-Frequência**: Combina a análise temporal e espectral.
- **Aplicações**: Processamento de imagens, compressão de dados, e detecção de eventos em sinais biomédicos.

#### Transformada Wavelet

A Transformada Wavelet decompõe um sinal em componentes associadas a diferentes escalas (resoluções).

##### Comparação com Fourier

- A Transformada de Fourier (TF) não captura bem as mudanças locais no tempo.
- A Wavelet resolve isso com janelas adaptativas, permitindo análise local.

#### Tipos de Wavelets

- **Haar**: Simples, ideal para introdução.
- **Daubechies**: Mais sofisticadas, usadas em processamento de imagens.

#### Atividade Prática

1. Implementar a Transformada Wavelet Discreta (DWT) em Python.
2. Aplicar DWT para compressão de imagem e observar diferenças na qualidade.