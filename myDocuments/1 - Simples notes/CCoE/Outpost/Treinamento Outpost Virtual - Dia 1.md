---
Data de criação: 2025-05-13
---
# Agenda
## Day 1
- Amazon VPC Design for AWS Outpost
- AWS Outposts Governance
- Local Gateway Deep Dive
- Security in Outposts

##  Day 2
- Infrastructure automation in Outpost
- SDK Structure with Outpost (EC2, EBS, S3, ALB and RDS)
- ALB Deep Dive on Outposts

## Day 3
- Resiliency in Outposts (PG, Multi A-Z, Fail over, Fail-Back)
- EKS in Outpost
- Design Clinic (ACME Inc case, reading)
- Design Clinic (review)

# Day 1

## Application continuum
![[Pasted image 20250513134703.png]]
![[Pasted image 20250513135121.png]]
![[Pasted image 20250513135130.png]]
![[Pasted image 20250513135205.png]]
Infraestrutura física, de fácil instalação, é esta todo o tempo conectado nas regiões da AWS
![[Pasted image 20250513135320.png]]
![[Pasted image 20250513135333.png]]
## Amazon VPC Designs with Outposts
![[Amazon VPC Designs with Outposts.png]]
- É necessário entregar algumas configs, como o CIDR block
- Precisam fazer um plano de capacidade dos CIDRs para não ter preocupação como o consumo dos IPs dessa VPC para os Workloads
- Pode criar uma vpc sem subntes na região, e criar elas se você precisar no Outpost
	- Faz sentido se os workloads não tem ligação com a região
- A criação de uma vpc no Outpost é o mesmo processo que na AWS
	- Vocês não precisam indicar algum dado especifico do outpost quando for criar uma vpc

## Routing Local Network
![[Routing Local Network.png]]
- O conceito de AZ nos racks não mudam. Outpost ID 
- Local gateway
- Legacy on premisses - configurar na routetable a subnet particular, uma entrada para os seguimentos da rede interna

## Customer's Segmentation
### VPC Mapping
![[Customer's Segmentation - VPC Mapping.png]]
- Não pode ter overlapping dos blocos do cidr entre eles
- Até 4 rtbs - contextos - local gtw
## Centralized Governance - AWS Outpost
![[Centralized Governance - AWS Outpost.png]]
### Option 1: Network-pro account owned Amazon VPC
![[Pasted image 20250513161446.png]]
### Option 3: Outpost owner account-owned AMZ VPC
![[Pasted image 20250513161932.png]]![[Pasted image 20250513163956.png]]
![[Pasted image 20250513164112.png]]

![[Pasted image 20250513164537.png]]

![[Pasted image 20250513170310.png]]
## Local Gateway Deep Dive
![[Pasted image 20250513171850.png]]
# Day 2
![[Pasted image 20250514134632.png]]
- **CloudFormation**: ferramenta da AWS para criar infraestrutura como código (IaC).  
- **AWS Outposts**: leva a infraestrutura da AWS para o seu data center local.
1. **Permite criar EC2 localmente via template** YAML/JSON.
2. **Usa os mesmos comandos e estrutura** que na nuvem pública.
3. Você **deve informar o Outpost** usando:
    - `SubnetId` associada ao Outpost
    - `Placement` com `Tenancy` e, se necessário, `HostId`

- Use **AMIs compatíveis com Outposts**
- A **sub-rede deve estar vinculada ao Outpost**
- Verifique se o **Outpost tem capacidade suficiente**

- Mesma experiência da AWS, mas **local**
- Ideal para **baixa latência** e **requisitos regulatórios**
- **Automação e versionamento** da infraestrutura local

- **não é obrigatório usar diretamente o `OutpostId` no template do CloudFormation** para criar uma instância EC2 no Outposts. A **chave para direcionar a criação ao Outposts** é usar uma **sub-rede (`SubnetId`) que pertence ao Outpost**.
- EBS só tem armazenamento GP2 - Gen1

## S3 on Outpost
![[S3 on Outpost.png]]
- Apenas um tipo de S3 - S3 Outpost
	- Não tem a movimentação de tier
	- Consegue fazer o lifecycle na região

Apenas integração com:
- Ebs snapshoot
- RDS - Backup de dados
- EC2 - Endpoint, ACP 


- 3 coisas principais
	- Bucket S3 
	- S3 Access Point para cada um
		- Pode ter até 100 s3 na aplicação - diferentes tiers de storage 
	- Criar um Endpoint de s3
		- uso de ens
		- permitir as instancias ec2 ter acesso aos buckets
		- RAM - pode compartilhar o uso dos buckets para as contas filhas - nos workloads
- Precisa ter o SubnetID e o SGID - para o endpoint
- Precisa ter o  BucketName e OutpostID - para o Bucket
- Precisa ter o Bucket e o endpoint 

- Pode controlar esses acessos por meio de uma S3 Policy
	- Precisa criar com uma estrutura arn própria para outpost


## Where is my data stored?
- Data is always stored on the Outpost
	- Object data
	- Object system and user metadata
	- Object tags
 
- Buckets are created and managed in the Outpost home region

- Telemetry is available in the home region
![[Pasted image 20250514135947.png]]
- dados SEMPRE são salvos localmente
- toda a volumetria e o acesso aos s3, tem uma 


## ALB on AWS Outpost
### SDK Structure with Outpost (EC2, EBS, S3, ALB and RDS)
### ALB on AWS Outpost
- Automatically distribute trafic across multiple targets on Outposts rack and on-premises
- Target include Amazon EC2 instances, ECS/EKS, and IP addresses
- Support for HTTP and HTTPS protocols
- Operates in a single subnet
- Support for internal and external load-balancers
	- External load-balancer can use COIP or Amazon IP
- Scale automatically up to the capacity available on the Outpost rack
- Visibility thru CLoudWatch metrics, access logs, and PHD notification
- Requires CS, MS, RS, CSD, MSD, RSD instances types on Outpost rack
![[Pasted image 20250514144024.png]]
- Só pode fazer o load balance para dentro do mesmo Outpost ID


![[Pasted image 20250514144355.png]]
![[Pasted image 20250514144850.png]]![[Pasted image 20250514145819.png]]
![[Pasted image 20250514145902.png]]
### Capacity Estimate 
![[Pasted image 20250514145951.png]]


|         | c5/c5d | r5/r5d | m5/m5d |
| ------- | ------ | ------ | ------ |
| large   | 16     | 13     | 9      |
| xlarge  | 28     | 26     | 18     |
| 2xlarge | 55     | 50     | 35     |
| 4xlarge | 28100  | 96     | 65     |
![[Pasted image 20250514154302.png]]

# Day 3
![[Pasted image 20250515134522.png]]
![[Pasted image 20250515135228.png]]
![[Pasted image 20250515143307.png]]![[Pasted image 20250515143312.png]]