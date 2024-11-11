---
tags:
  - dictionary
Index: "[[Dictionary]]"
---
# O que é Web Application Firewall (WAF)?

O WAF, ou firewall de aplicativos web, ajuda a proteger os aplicativos web ao filtrar e o monitorar o tráfego HTTP entre o aplicativo web e a internet. Ele geralmente protege os aplicativos web contra ataques como [[Falsificação de solicitação de sites]], [[Cross-site-scripting (XSS)]], inclusão de arquivos e [[Injeção de SQL]], entre outros.

O WAF é uma defesa de protocolo da camada 7 (no modelo OSI) e não foi desenvolvido para defender contra todos os tipos de ataques. Esse método de mitigação de ataques costuma fazer parte de um conjunto de ferramentas que, juntas criam uma defesa holística contra diversos vetores de ataque.

Com a implantação de um WAF à frente da aplicação web, é colocado um escudo entre a aplicação e a internet. Enquanto um servidor proxy protege a identidade da máquina cliente com o uso de um intermediário, o WAF é um tipo de [[Proxy reverso]] que protege o servidor contra a exposição, já que seus clientes passam pelo WAF antes de chegar ao servidor.

O WAF funciona por meio de um conjunto de regras normalmente chamadas de "Politicas". As politicas tem como objetivo proteger o aplicativo contra vulnerabilidades filtrando o tráfego malicioso. O valor de um WAF deve-se, em parte à velocidade e À facilidade com que a modificação das politicas pode ser implantada, permitindo uma resposta mais rápida a variados vetores de ataque. Durante um ataque DDos, o rate limiting pode ser implantado rapidamente  modificando-se as politicas do WAF.