# Sobre o exame
- 90 minutos
- 65 perguntas
- 100 a 1000 (mais de 700 para aprovar)
- $100 USD por tentativa
- Perguntas de múltipla escolha 
- Opção de apresenta-lo pessoalmente ou virtualmente 
# AWS Cloud Practitioner v.2
## Tópicos principais do exame

| % do exame | dominio                  | areas de enfoque                                                                  |
| ---------- | ------------------------ | --------------------------------------------------------------------------------- |
| 34%        | Tecnologia               | Infraestrutura global da AWS, serviços principais da AWS                          |
| 24%        | Conceito de nuvem        | Proposta de valor da nuvem                                                        |
| 30%        | Segurança e conformidade | Modelo de respnsabilidade compartilhada, serviços básicos de segurança            |
| 12%        | Faturamento e preços     | Ferramentas de análise de preço/custo, modelos de preços de serviços, faturamento |
## Você está pronto ?
- Voucher para as 5 primeiras pontuações (elas devem ter pelo menos 70% de respostas corretas)
- em caso de empate, o tempo de resposta é o critério de desempate
- válido somente para a certificação Cloud Practitioner
- as condições para resgatar 
## Perguntas
### Q1 - O
Uma empresa está executando um aplicativo que consulta um banco de dados no Amazon RDS. Ultimamente, houve um aumento na latência das consultas durante os horários de pico de demanda. Qual serviço da AWS você pode usar para reduzir a carga do banco de dados e melhorar os tempos de resposta para consultas de leitura repetidas e frequentes?

a) Acelerador Amazon DynamoDB (DAX)
<mark style="background: #BBFABBA6;">b) ElasticCache</mark>
c) Amazon EMR
d) Amazon Redshift
#### Bancos de dados na memória
- Maior desempenho com custos otimizados adicioando uma camada de cache para dados lidos com frequência para otimizar os recursos.
- Um serviço gerenciado que simplifica o gerenciamento, o monitoramento e a operação de ambientes na memória. O serviço também está disponível em uma versão sem servidor.
- Tempos de resposta de microssegundos em centenas de milhões de operações por segundo
### Q2 - X
Uma empresa armazena informações comerciais no Amazon S3. Você precisa ser capaz de identificar se há informações confidenciais (PII) para validar se elas estão protegidas adequadamente. Qual serviço da AWS permite que você use o aprendizado de máquina (ML) e o reconhecimento de padrões para identificar esse tipo de dados confidenciais armazenados?

a) inspetor da Amazon
b) Amazon GuardDuty
c) Gerente de auditoria da AWS
<mark style="background: #BBFABBA6;">d) Amazon Macie</mark>
- Inspector só trabalaha com EC2
- Guarduty vai trabalhar com monitoria mas não trabalha com PII
- Audit manager só com auditoria, serviços, e só mostra os dados principais
#### Detecção de dados confidenciais
- O Amazon Macie é um serviço de segurança de dados que descobre dados confidenciais por meio de aprendizado de máquina e correspondência de padrões, fornece visibilidade dos riscos de segurança de dados e permite proteção automatizada contra esses riscos.
- Com o Amazon Macie, você pode automatizar a descoberta, o registro e a emissão de relatórios de dados confidenciais em seu patrimônio de dados do Amazon S3.
### Q3 - O

Quais dos seguintes NÃO são fatores a serem considerados ao escolher uma região geográfica na AWS? (Escolha dois)

a) Custos
b) Latência
<mark style="background: #BBFABBA6;">c) O número de parceiros da AWS na região</mark>
d) Disponibilidade dos serviços
<mark style="background: #BBFABBA6;">e) O idioma oficial do país onde a região está localizada</mark>
f) Conformidade e regulamentação locais

#### Shortlist potential Rgions for your workload

Let's follow the best practice on Region selection in the sustainability pillar of AWS Well-Architected Framework. The first step is to assess and shortlist potential Regions for your workload based on your business requirements.
In What to Consider when Selecting a Region for your Workloads, there are four key business factors to consider when evaluating and shortlisting each AWS Region for a workload:
• Latency
Cost
• Services and features
• Compliance

- O numero de parceiros não importa 
- Idioma oficial também não importa

## Q4 - X
Qual das seguintes opções é de responsabilidade da AWS, de acordo com o modelo de responsabilidade compartilhada para instâncias do Amazon EC2?

a) Configuração do Amazon VPC
b) Gerenciamento de código de aplicativo
c) Aplicação de patches ao sistema operacional
<mark style="background: #BBFABBA6;">d) Gerenciamento de infraestrutura de rede  </mark>

![[Modelo de responsabilidade compartilhada EC2.png]]

## Q5 - O
Qual serviço da AWS pode oferecer recomendações para reduzir custos, aumentar a segurança, melhorar o desempenho e a disponibilidade

a) Otimização da AWS
- Não é a melhor opção porque é um conceito e não um serviço
B) Inspetor da Amazon
- Só para EC2
<span style="color:rgb(0, 176, 80)">c) consultor confiável da AWS </span>
d) AWS CloudWatch

## Q6 - O
Não são perspectivas do AWS Cloud Adoption Framework ()AWS CAF) - Selecione DOIS
a) Pessoas
b) Plataforma
c) Segurança
<span style="color:rgb(0, 176, 80)">d) Desempenho</span>
e) Operações
<span style="color:rgb(0, 176, 80)">f) Custos</span>
![[Estrutura de adoção da nuvem da AWS.png]]
## Q7 - O
Que tipos de armazenamento de dados no EC2 oferece alto desempenho de E/S, é temporário e é perdido se a instância for interrompida ou encerrada?

a) Amazon S3 para EC2
b) Amazon EBS
c) Amazon EFS
<mark style="background: #BBFABBA6;">d) Armazenamento de instâncias do Amazon EC2</mark>

![[Amazenamento de instancias do Amazon EC2.png]]
## Q8 - X
Qual estratégia de migração para a nuvem envolve reescrever ou redesenhar aplicativos usando arquiteturas nativa da nuvem ?
a) Rehospedar
b) Mudança de plataforma
<mark style="background: #BBFABBA6;">c) Refatorar</mark>
d) Realocar
![[Sete estratégias de migração.png]]
## Q9 - O
Uma empresa global de comércio eletrônico quer otimizar seus custos da AWS e implementar o rastreamento de alocação de custos. Com vários departamentos operando aplicativos em várias regiões da AWS, a equipe financeira precisa entender os padrões de gastos para implementar uma estratégia eficaz de controle de custos. Quais opções ajudariam a atingir esses requisitos?

a) Use os orçamentos da AWS para definir limites de gastos mensais e configurar o AWS Shield Advanced para proteção de custos.

<mark style="background: #BBFABBA6;">b) Crie contas separadas da AWS para cada departamento, consolide-as usando o AWS Organizations e use o Cost Explorer para analisar padrões de gastos.
</mark>
c) Configure o AWS CloudWatch para monitorar a utilização de recursos e use o Amazon Inspector para rastrear anomalias de custo.

d) Habilite as categorias de custo da AWS para agrupar custos por diferentes unidades de negócios e use o AWS Marketplace para comprar ferramentas de otimização de custos.

## Q10 - O
Qual afirmação é verdadeira sobre a relação entre sub-redes e zonas de disponibilidade? 
a) Você pode criar somente uma sub-rede por zona de disponibilidade
<mark style="background: #BBFABBA6;">b) Você ode criar uma ou mais sub-redes em cada zona de disponibilidade </mark>
c) As sub-redes abrangem várias zonas de disponibilidade
d) As sub-redes podem ser estendidas para outras regiões

## Q11 - O/X
Quais dos seguintes são os princípios de design do pilar de segurança do Well-Architected Framework? (Selecione DOIS)

a) Experimentação mais frequente
<mark style="background: #BBFABBA6;">b) Mantendo a rastreabilidade</mark>
c) Testando procedimentos de recuperação 
d) Mudanças frequentes, pequenas e reversíveis 
<mark style="background: #BBFABBA6;">e) Proteção de dados em trânsito e em repouso</mark>

https://aws.amazon.com/pt/architecture/well-architected/?wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc&wa-guidance-whitepapers.sort-by=item.additionalFields.sortDate&wa-guidance-whitepapers.sort-order=desc

## Q12 - O
Uma empresa precisa de um relatório automatizado de avaliação de segurança que identifique exposições desnecessárias no nível da rede e
vulnerabilidades comuns em aplicativos executados em instâncias do Amazon EC2. Qual serviço ou recurso da AWS a empresa deve usar para atender a esse requisito?
a) Consultor confiável da AWS
b) AWS GuardDuty
c) Amazon Macie
<mark style="background: #BBFABBA6;">d) Inspetor da Amazon</mark>
#### Detecte vulnerabilidades em aplicativos
• Detecte vulnerabilidades de software e exposição de rede não intencional quase em tempo real nas cargas de trabalho da AWS, como Amazon EC2, funções do AWS Lambda e Amazon ECR.
- Use a pontuação de risco altamente precisa do Amazon Inspector para priorizar com eficácia a resolução de seus problemas
## Q13 - O
Um cliente tem 250 TB de dados estruturados a serem migrados para um sistema de armazenamento para permitir a execução de consultas SQL complexas. Que solução econômica e eficiente permitiria que os dados fossem armazenados e analisados e, em seguida, integrados às ferramentas de BI?
<mark style="background: #BBFABBA6;">a) Amazon Redshift</mark> 
b) Amazon RDS
c) Amazon ElastiCache
d) Instâncias do EC2 MySQL em Multi-AZ

#### Serviço de análise escalável
- Armazém de dados em nuvem totalmente gerenciada e escalável
- Ele usa SQL padrão e tem integração com várias ferramentas de inteligência de negócios (BI) do mercado
- Dimensione para petabytes
- Opção sem servidor
## Q14 - X
Um cliente tem uma arquitetura de rede distribuída em sub-redes públicas e privadas. Qual componente da VPC pode ser implementado para proteger os recursos no nível da sub-rede?
a) Grupo de segurança
<mark style="background: #BBFABBA6;">b) ACL de rede</mark>
c) Registros de fluxo da VPC
d) Autenticação com IAM

#### Filtragem de tráfego na VPC
Firewall virtual para controlar o tráfego de entrada e saída de uma ou mais sub-redes.
- Uma lista de controle de acesso à rede (ACL) permite ou nega tráfego especifico de uma entrada ou saída no nível da sub-rede
- O VPC Default já tem uma lista de padrão de controle de acesso à rede que permite todo o tráfego de entrada e saída da sub-rede
## Q15 - O
Qual das seguintes opções de preços é a mais econômica para o Amazon RDS, se seu uso for necessário por 3 anos, com uso permanente (24 horas por dia, 7dias por semana)?
a) Sob demanda
b) Spot
<mark style="background: #BBFABBA6;">c) Instancias reservadas</mark>
d) Planos de poupança
- Spot é para quando você precisa de pouco tempo