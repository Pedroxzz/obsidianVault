---
Index: "[[Processamento digital de Sinais]]"
---
**Objetivo**: Introduzir o conceito de filtros digitais e demonstrar seu papel no processamento de sinais.

#### O que são Filtros?

Filtros são sistemas projetados para enfatizar ou atenuar certas frequências de um sinal.

##### Tipos de Filtros

1. **Passa-Baixa**: Permite frequências abaixo de um limite.
    
2. **Passa-Alta**: Permite frequências acima de um limite.
    
3. **Passa-Banda**: Permite frequências dentro de uma faixa específica.
    
4. **Rejeita-Banda**: Bloqueia frequências dentro de uma faixa específica.
    

##### Resposta ao Impulso

A resposta ao impulso descreve como o filtro reage a um impulso unitário no tempo.

#### Projeto de Filtros

Os filtros podem ser projetados no domínio do tempo ou frequência. Alguns métodos populares incluem:

- **Filtros FIR (Finite Impulse Response)**: Resposta finita ao impulso.
    
- **Filtros IIR (Infinite Impulse Response)**: Resposta infinita ao impulso.
    

#### Atividade Prática

1. Criar um filtro passa-baixa em Python utilizando a biblioteca scipy.
    
2. Aplicar o filtro a um sinal de áudio ruidoso e comparar o sinal antes e depois do filtro.