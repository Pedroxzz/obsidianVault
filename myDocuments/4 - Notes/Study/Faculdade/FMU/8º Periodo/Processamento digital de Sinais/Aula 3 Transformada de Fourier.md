---
Index: "[[Processamento digital de Sinais]]"
---
**Objetivo**: Introduzir o conceito de Transformada de Fourier e sua aplicação na análise de sinais no domínio da frequência.

#### O que é a Transformada de Fourier?

A Transformada de Fourier (TF) permite decompor um sinal no domínio do tempo em suas componentes de frequência. Para um sinal contínuo :

#### Propriedades da TF

- **Linearidade**: A transformada de uma soma é a soma das transformadas.
    
- **Deslocamento no Tempo**: Um atraso no tempo resulta em um deslocamento de fase.
    
- **Dualidade**: Relaciona a forma do sinal no domínio do tempo e da frequência.
    

#### Aplicações Práticas

1. Análise de áudio para identificar frequências dominantes.
    
2. Compressão de dados (MP3 utiliza TF).
    

#### Transformada Discreta de Fourier (TDF)

A versão discreta da TF é usada para sinais digitalizados. Dada uma sequência :

#### Atividade Prática

1. Gerar um sinal composto por duas senoidais de diferentes frequências e calcular sua TDF.
    
2. Visualizar o espectro de frequência utilizando Python (bibliotecas: numpy e matplotlib).