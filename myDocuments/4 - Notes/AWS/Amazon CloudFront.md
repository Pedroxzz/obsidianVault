---
tags:
  - aws
---


# Amazon CloudFront

O Amazon Cloudfront é um serviço de rede de entrega de conteúdo ([[CDN]]) criado para alta performace, segurança e conveniência do desenvolvedor.

## Casos de uso
- **Forneça sites rápidos e seguros**: Alcance visualizadores em todo o mundo em milissegundos com a compactação de dados integrada recursos de [[Computação de borda]] e criptografia em nível de campo.
- **Acelere a entrega de conteúdo dinâmico e as APIs**: Otimize a entrega de contudo da Web com a infraestrutura de rede global da AWS desenvolvida para fins específicos e rica em recursos que oferece suporte à terminação de borda e WebSockets.
- **Transmita vídeos ao vivo e sob demanda:** Inicia streams rapidamente, reproduza-os com consistência e entregue vídeos de alta qualidade para qualquer dispositivo com a integração do AWS Media Service e AWS Elemental.
- **Distribua patches e atualizações**: Dimensione automaticamente para fornecer software, patches de jogos e atualizações de IoT over-the-air (OTA) em grande escala com altas taxas de transferência. 
---
## Conceitos Básicos

O Amazon CloudFront é uma rede de entrega de conteúdo (CDN)  que acelera a entrega de conteúdo estático e dinâmico da Web para usuários finais.

O CloudFront distribui o conteúdo por meio de uma rede global de datacenters denominados **locais de borda**. Quando um usuário final solicita um conteúdo que você está fornecendo no CloudFront, a solicitação é roteada ao local da borda mais próximo ao usuário final com a menor latência.

O CloudFront entrega conteúdos usando a rede global da AWS que conecta os locais de borda da AWS às regiões da AWS. A movimentação do trafego ao longo da rede da AWS reduz a latência e aprimora a postura de segurança da aplicação. Aumente a confiabilidade e a disponibilidade das suas aplicações Web ao ter copias dos arquivos em cache em diversos locais da borda em todo o mundo.

---


