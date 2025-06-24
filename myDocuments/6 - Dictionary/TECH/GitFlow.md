---
tags:
  - dictionary
Index:
---


GitFlow é uma estratégia de branching (ramificação) no Git que ajuda a organizar e gerenciar o fluxo de desenvolvimento de software de forma estruturada. Ela é especialmente útil para projetos com ciclos de desenvolvimento complexos ou contínuos. A estratégia define um conjunto de ramificações e regras para interagir com elas

### 1. Branches principais
- **'main'**: Também chamada de 'master' em alguns projetos, é a branch principal que contém a versão estável do código. Normalmente, essa branch só contém código pronto para ser lançado
- **'develop'**: Esta é a branch principal de desenvolvimento. Todas as novas funcionalidades e correções são integradas aqui antes de serem lançadas

### 2 .Branches de suporte
- **'feature/'**: Essas branches são usadas para desenvolver novas funcionalidades. Cada funcionalidade deve ter sua própria branch derivada de **'develop'**. Quando a funcionalidade é concluída, a branch é mesclada de volta em **'develop'**.
- **'release/'**: Quando o código na branch 'develop' está pronto para um novo lançamento, uma branch de release é criada. Esta branch permite que se façam ajustes finais e testes antes de mesclar o código na **'main'** e na **'develop'**. Após o lançamento, a branch de release é mesclada nas branches **'main'** e **'develop'**, e depois deletada
