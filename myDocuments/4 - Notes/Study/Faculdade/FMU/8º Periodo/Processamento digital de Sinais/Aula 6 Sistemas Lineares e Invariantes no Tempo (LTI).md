---
Index: "[[Processamento digital de Sinais]]"
---
**Objetivo**: Abordar os conceitos de linearidade e invariância no tempo em sistemas e sua importância no processamento digital de sinais.

#### Sistemas Lineares

Um sistema é linear se satisfaz os seguintes princípios:

- **Superposição**: A resposta a uma soma de entradas é igual à soma das respostas individuais.
    
- **Escalabilidade**: Se a entrada for escalada por um fator, a saída será escalada pelo mesmo fator.
    

#### Sistemas Invariantes no Tempo (LTI)

Um sistema é invariante no tempo se sua resposta a uma entrada não depende de quando a entrada é aplicada.

#### Resposta ao Impulso

A resposta ao impulso de um sistema LTI é a saída quando a entrada é um impulso unitário. Para um sistema com entrada e saída , a saída pode ser calculada como a convolução da entrada com a resposta ao impulso :

#### Função de Transferência

A função de transferência descreve o comportamento do sistema no domínio da frequência. Para sistemas discretos, ela é obtida pela Transformada Z da resposta ao impulso.

#### Aplicações Práticas

1. Modelagem de sistemas como circuitos elétricos e filtros digitais.
    
2. Previsão de como sistemas respondem a diferentes entradas.
    

#### Atividade Prática

1. Determinar a resposta ao impulso de um sistema LTI em Python.
    
2. Calcular a função de transferência para um filtro digital simples e plotar sua resposta em frequência.