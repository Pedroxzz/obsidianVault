---
tags:
  - dictionary
Index: "[[Dictionary]]"
---

## Visão Geral

O propósito da abordagem de CI/CD é otimizar e acelerar o ciclo de vida de desenvolvimento de software.
![[Pasted image 20240517160807.png]]

### Conceito
A integração continua (CI) é  a pratica de integrar, de forma automática e frequente, mudanças a um repositório de código.
Cada Integração é verificada, varias vezes ao dia de modo automatizado. O objetivo da CI é detectar erros de integração o mais cedo possível, antes que eles causem problemas.

Já a implantação e/ou entrega contínua (CD) é um processo em duas etapas relacionado a integração, teste e entrega de mudanças no código. A entrega continua garante que o código esteja sempre em estado pronto para implantação em produção, tornando a implantação um processo simples e repetível.

A entrega contínua é quase uma implantação automática em produção, enquanto a implantação contínua implica em automaticamente lançar atualizações no ambiente de produção.

Juntas , essas práticas relacionadas são muitas vezes chamadas de pipeline de CI/CD.

---
## Processo
1. Um desenvolvedor envia o código para um repositório Git.
2. Um servidor de integração (CI) monitora o repositório e detecta a alteração. (Jenkins).
3. O servidor CI realiza a construção do código executa testes automatizados.
4. Se os testes forem bem-sucedidos, o código é implantado em um ambiente de homologação
5. Testes adicionais, como testes de aceitação, são executados no ambiente de homologação.
6. Se todos os testes forem aprovados, o código é implantado em produção.
7. O aplicativo é monitorando em produção, e quaisquer problemas são detectados e tratados imediatamente. 

---
## Benefícios

A CI/CD oferece uma série de benefícios:

1. **Detecção precoce de Erros**: A CI verifica constantemente o código, identificando erros e problemas de integração no estágio mais inicial do desenvolvimento. 
2. **Maior qualidade de Software**: A execução de testes automatizados e a revisão contínua do código ajudam a garantir que o software seja mais confiável e livre de bugs.
3. **Automatização de Tarefas**: A CD automatiza a construção, testes e implantação, economizando tempo e reduzindo a possibilidade de erros humanos.
4. **Implantações mais Rápidas:** Com a CD, as implantações em produção podem ser feitas com mais frequência e mais facilidade, resultando em ciclos de desenvolvimento mais curtos.
5. **Colaboração Eficiente:** A CI promove a colaboração contínua entre membros da equipe, garantindo que o código seja sempre integrado e testado.
6. **Maior Confiança e Transparência:** Com a CI/CD, a equipe tem mais confiança na estabilidade do código e pode rastrear as alterações com mais facilidade.

---
## Referencias
- https://www.redhat.com/pt-br/topics/devops/what-is-ci-cd
- https://medium.com/@habbema/desvendando-ci-cd-b56f515ddd20
