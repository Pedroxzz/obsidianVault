---
Index: "[[Processamento digital de Sinais]]"
---
**Objetivo**: Ensinar como sinais contínuos podem ser transformados em discretos, respeitando as regras de amostragem e quantização.

#### Amostragem

A amostragem é o processo de capturar valores de um sinal contínuo em intervalos regulares. Isso é necessário para representar sinais no domínio digital.

##### Teorema de Nyquist-Shannon

Para evitar perda de informação, a frequência de amostragem (Fs) deve ser pelo menos o dobro da maior frequência presente no sinal (Fmax):

**Exemplo**: Um áudio com frequências até 10 kHz deve ser amostrado com pelo menos 20 kHz.

##### Efeitos da Subamostragem (Aliasing)

- **Aliasing** ocorre quando Fs < 2·Fmax, causando sobreposição de frequências no espectro.
    
- **Demonstração**: Amostrar uma onda senoidal de 5 Hz com Fs = 8 Hz resulta em uma frequência percebida errada.
    

##### Como Evitar Aliasing

- **Filtro Anti-Aliasing**: Remove componentes de alta frequência antes da amostragem.
    

#### Quantização

A quantização converte valores contínuos de amplitude em níveis discretos.

##### Processo

1. Divida o intervalo de amplitude em níveis iguais.
    
2. Atribua cada valor de entrada ao nível mais próximo.
    

##### Erros de Quantização

- **Erro**: Diferença entre o valor real e o valor quantizado.
    
- **Relação Sinal-Ruído (SNR)**: Medida da qualidade do sinal após quantização. Depende do número de bits usados.
    

Onde é o número de bits.

#### Atividade Prática

1. Amostrar uma função senoidal em Python com diferentes Fs e observar o aliasing.
    
2. Implementar quantização de sinais com 8 e 16 bits e calcular o SNR.
    

---