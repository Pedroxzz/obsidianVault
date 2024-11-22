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
## Principais vantagens da nuvem em relação ao local

1- Opex - Vpex
2- Economias em escala
3- Elasticidade
4- Agilidade e velocidade
5- Menos gasto em data center 
6- Presença global

### Despesa de capital comercial por despesa variável 
- Despesa de capital
	- Dinheiro que uma organização gasta para comprar, manter ou melhorar ativos fixos
- Despesa variável / operacional 
	- Despesas contínuas necessárias para administrar o negocio
### Economia de escala
#### **Custos variáveis mais baixos**
O uso de centenas de milhares de clientes é agregado na nuvem. A AWS obtém grandes economias de escala ao ser agregadora desse uso.

- **Efeito Flywheel** - Mias usuários na nuvem, maior volume de compras de componentes, menores preços por unidade
- **Economia de repasse** - Nossos baixos custos variáveis se traduzem em economias para nossos clientes, maiores do que poderiam ser obtidas por você mesmo

#### **Capacidade de infraestrutura**
O local exige decisões de capacidade antes de realmente implantar um aplicativo

- Sob provisão - o crescimento de seus negócios ou a experiencia do cliente são limitados por restrições de capacidade
- Provisão excessiva - Seus recursos caros ficam ociosos

#### Capacidade escalonada

A infraestrutura baseada em nuvem permite que você aumente ou diminua seus serviços com apenas alguns minutos de antecedência. Isso permite que você acesse a capacidade necessária ou mínima. Provisione dinamicamente sua infraestrutura de nuvem para atender às necessidades reais de capacidade.
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
Os Pontos de Presença permitem que o [[Amazon CloudFront]] entregue dados, vídeos, aplicativos e APIs de forma segura para os clientes globalmente, com baixa latência e altas velocidades de transferência, tudo dentro de um ambiente amigável para desenvolvedores.


## [[Amazon CloudFront]]

Content Delivery Network ([[CDN]]), com baixa latência e alta velocidade de transferência

**Resumo do Serviço**  
Serviço web que acelera a distribuição de conteúdo estático e dinâmico para os usuários finais. Roteia as solicitações de conteúdo para a localização de borda com a menor latência para otimizar o desempenho.

**Casos de Uso**  
• Entregar sites rápidos e seguros  
• Acelerar a entrega de conteúdo dinâmico e APIs  
• Transmitir vídeo ao vivo e sob demanda  
• Distribuir patches e atualizações

# Introdução aos Serviços da AWS
## Computação
---
- Instancias
	- Amazon EC2
- Contêineres 
	- Amazon ECS
	-  Amazon EKS
	- Amazon Fargate
- Serverless
	- AWS Lambda
---
### Amazon EC2

==Capacidade computacional segura e redimensionável para suportar praticamente qualquer carga de trabalho==

Um serviço web que fornece capacidade computacional segura e redimensionável na nuvem. Ele foi projetado para facilitar a computação em nuvem em escala web para desenvolvedores
- Escala 
	- Aumente ou diminua a capacidade em minutos e forneça 99,99% de disponibilidade para cada região do Amazon EC2
- Preço
	- Oferece cinco modelos de prelos para pagar pelas instancias ECC2: sob demanda, planos de economia, host dedicados, instancias spot e instancias reservadas

### AWS Lambda

==Execute código sem gerenciar servidores==

O AWS Lambda é um serviço computacional sem servidor e orientado por eventos que permite executar  código para praticamente qualquer tipo de aplicativo ou serviço de back-end sem provisionar ou gerenciar servidores

Você pode adicionar o Lambda a partir de mais de 200 serviços da AWS e aplicativos de software como serviço (SaaS) e pagar apenas pelo que usar 

### Imagens de máquina da Amazon (AMI)

==Informações criticas necessárias ao iniciar instâncias EC2==

- Contém as informações necessárias para iniciar uma instancia EC2

- Deve ser especificado ao iniciar uma instancia

- Várias instancias podem ser excetuadas a partir de uma única AMI

- Pode incluir o software desejado para ser instalado na instancia do EC2 no momento da inicialização 

### AWS Cloud Formation

### Container
- Camada de virtualização [[Hipervisor]]
	- AWS Nitro 

### Amazon Elastic Container Service ECS

### Amazon Elastic Kubernets EKS

### AWS Fargate 

## Armazenamento de dados
### Amazon Elastic File System EFS

### Amazon FSx

###  Amazon Elastic Block Storage EBS

### Amazon S3

## Classes de armazenamento do S3

## Networking 
### Amazon VPC 

### Security Group e NACLs

### Amazon Route 53 

## Ofertas de Banco de dados 