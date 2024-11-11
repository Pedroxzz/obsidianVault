---
Data de criação: 2024-11-05
Index: "[[Certifications]]"
My Tags: "[[AWS]]"
tags:
  - "#aws"
---

Material abordado no programa da Latam AWS Partner Certification onde foi abordado os temas principais e importantes para a certificação Cloud Practitioner 

---
# Conceitos de computação em nuvem 
## O que é um [[data center]]?
Um local físico que armazena máquinas de computação e seus equipamentos de hardware relacionados. Ele contém a infraestrutura de computação necessária para os sistemas de TI, como servidores, unidades de armazenamento de dados e equipamentos de rede. É a instalação física que guarda os dados digitais de qualquer empresa.
### Data Centers Tradicionais
A empresa é 100% responsável por adquirir o local, desenvolvê-lo e garantir sua segurança. O hardware adequado deve ser adquirido, instalado e mantido.
### Serviços de nuvem
O "trabalho pesado indiferenciado" de gerenciar o data center é realizado pelo provedor de serviços em nuvem, permitindo que os clientes se concentrem na entrega de valor.


## O que é [[nuvem]]?
- Modelo de responsabilidade compartilhada
- Não cuida do hardware, apenas do serviço

Computação em nuvem é a entrega sob demanda de recursos de TI pela Internet com pagamento conforme o uso. Em vez de comprar, possuir e manter data centers e servidores físicos, as organizações podem adquirir serviços de tecnologia, como poder de computação, armazenamento, bancos de dados e outros serviços conforme a necessidade.
### On-premises
Tradicionalmente, uma empresa precisava investir em todo o hardware físico necessário para operar os sistemas de negócios na utilização máxima.
### Cloud
Com a computação em nuvem, as empresas agora podem acessar esses recursos por meio de um provedor de serviços em nuvem, como a AWS, e pagar apenas pelo que realmente utilizam.


## O que é uma nuvem híbrida?

Um design de infraestrutura de TI que integra os recursos internos de TI de uma empresa com a infraestrutura e os serviços de provedores de nuvem de terceiros. Permite armazenar dados e executar aplicações em diversos ambientes. O ambiente de nuvem híbrida ajuda a provisionar, escalar e gerenciar centralmente seus recursos de computação.

### Benefícios
- aumento da agilidade de desenvolvimento  
- maior escalabilidade  
- continuidade dos negócios
### Casos de uso
- aplicações de baixa latência  
- processamento de dados localmente  
- atendimento à conformidade regulatória  
- expansão do data center  
- suporte à migração para a nuvem


## Resumo do modelo de implantação
### Resumo das três formas diferentes de implantar suas cargas de trabalho:

#### [[On-premises]]
Implantar recursos no local, usando virtualização e ferramentas de gerenciamento de recursos, é às vezes chamado de "nuvem privada". Na maioria dos casos, esse modelo de implantação é semelhante à infraestrutura de TI legada, utilizando tecnologias de gerenciamento de aplicações e virtualização para tentar aumentar a utilização dos recursos.

#### Cloud
Uma aplicação baseada em nuvem é totalmente implantada na nuvem, e todas as partes da aplicação são executadas na nuvem. As aplicações na nuvem foram criadas diretamente na nuvem ou migradas de uma infraestrutura existente para aproveitar os benefícios da computação em nuvem.
#### Hybrid
Uma implantação híbrida é uma maneira de conectar infraestruturas e aplicações entre recursos baseados em nuvem e recursos existentes que não estão localizados na nuvem. A forma mais comum de implantação híbrida é entre a nuvem e a infraestrutura local existente, para expandir e aumentar a infraestrutura de uma organização na nuvem, conectando recursos da nuvem a sistemas internos.
## Modelos de computação em nuvem
### [[IaaS]]
Contém os blocos básicos para TI em nuvem e normalmente fornece acesso a recursos de rede, computadores (virtuais ou em hardware dedicado) e espaço de armazenamento de dados.

### [[PaaS]]
- Responsabilidade do provedor
Elimina a necessidade de as organizações gerenciarem a infraestrutura subjacente (geralmente hardware e sistema operacional) e permite que você se concentre na implantação e no gerenciamento de suas aplicações.
### [[SaaS]]
Fornece um produto completo que é executado e gerenciado pelo provedor de serviços. Na maioria dos casos, ao se referir a software como serviço, está se referindo a aplicações voltadas para o usuário final.

# Proposta de valor da Nuvem

# Infraestrutura Global AWS
## [[AWS Regions]]

**O que há em uma Região?**  
Cada Região da AWS consiste em várias Zonas de Disponibilidade isoladas e fisicamente separadas.

**Por que são importantes?**  
As Regiões da AWS são totalmente isoladas umas das outras, criando a maior tolerância a falhas e estabilidade possíveis.


## AWS Availability Zones (AZs)

**Por que são importantes?**  
As Zonas de Disponibilidade (AZs) oferecem aos clientes a capacidade de operar aplicativos de produção e bancos de dados que são mais altamente disponíveis, tolerantes a falhas e escaláveis do que seria possível em um único data center.  
As AZs são conectadas entre si por redes privadas de fibra ótica rápidas, permitindo que você projete facilmente aplicativos que realizam failover automaticamente entre as AZs sem interrupção.


## Edge Locations

**O que são?**  
São [[Endpoint|endpoints]] menores usados para hospedar dados em cache.

**Por que são importantes?**  
Os Pontos de Presença permitem que o Amazon CloudFront entregue dados, vídeos, aplicativos e APIs de forma segura para os clientes globalmente, com baixa latência e altas velocidades de transferência, tudo dentro de um ambiente amigável para desenvolvedores.


## [[Amazon CloudFront]]

Content Delivery Network ([[CDN]]), com baixa latência e alta velocidade de transferência

**Resumo do Serviço**  
Serviço web que acelera a distribuição de conteúdo estático e dinâmico para os usuários finais. Roteia as solicitações de conteúdo para a localização de borda com a menor latência para otimizar o desempenho.

**Casos de Uso**  
• Entregar sites rápidos e seguros  
• Acelerar a entrega de conteúdo dinâmico e APIs  
• Transmitir vídeo ao vivo e sob demanda  
• Distribuir patches e atualizações


## Container
- Camada de virtualização [[Hipervisor]]
	- AWS Nitro 

