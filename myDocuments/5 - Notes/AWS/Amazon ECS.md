
# O que é o Amazon Elastic Container Service?

O Amazon Elastic [[Container]] Service (Amazon ECS) é um serviço totalmente gerenciado de orquestração de contêineres que ajuda a implementar, gerenciar e escalar aplicações em contêineres de maneira mais eficiente.  Ele se integra totalmente ao ambiente da AWS para fornecer uma solução rápida e fácil de usar para executar workloads de contêineres na nuvem e [[On-Premise]] com atributos de segurança avançados usando o Amazon ECS Anywhere.

## Como funciona
Basta descrever suas aplicações e os recursos necessários, e o Amazon Elastic Conteiner Service (Amazon ECS) vai executar, monitorar e escalar a aplicação em opções flexíveis de computação com integração automáticas com outros serviços de suporte da AWS de que sua aplicação precise. Execute operações do sistema, como criar regras personalizadas de escalabilidade e capacidade além de observar e consultar dados de logs de aplicações e telemetria. 

## Recursos
### Principais recursos
#### Integrado e sem servidor por padrão com o AWS Fargate
O AWS Fargate é integrado ao Amazon ECS, então você não precisa mais se preocupar com o gerenciamento de servidores, o planejamento da capacidade ou a descoberta de como isolar as workloads do contêiner para segurança. Basta definir os requisitos da sua aplicação, selecionar o AWS Fargate como o tipo de execução no console ou na interface de linha de comando (CLI), e o AWS Fargate cuidará de todo o gerenciamento de escalabilidade e infraestrutura necessários para executar seus contêineres em opções de computação flexíveis, com integrações automáticas com outros serviços de suporte da AWS de que sua aplicação precisa.

#### Implantações híbridas
Com o Amazon ECS Anywhere, você pode usar o mesmo console e as ferramentas de operação familiares do Amazon ECS para gerenciar suas workloads de contêiner on-premises para ter uma experiência consistente em suas aplicações baseadas em contêiner. Você também pode usar o Amazon ECS no AWS Outposts para executar aplicações conteinerizadas que exigem latências particularmente baixas em sistemas on-premises.

#### Segurança e isolamento por padrão
O Amazon ECS se integra nativamente com as ferramentas de segurança, identidade e gerenciamento e governança nas quais você já confia, o que ajuda você a entrar em produção com rapidez e sucesso. Você pode atribuir permissões detalhadas para cada um de seus contêineres, proporcionando um alto nível de isolamento ao criar suas aplicações. Execute seus contêineres com os níveis de segurança e compatibilidade que você espera da AWS. E, por meio de integrações com o Amazon GuardDuty, você pode detectar de forma rápida e fácil ameaças externas às suas workloads antes que elas piorem.

#### Operações do ambiente de gerenciamento autônomo 
O Amazon ECS é um serviço de orquestração de contêiner totalmente gerenciado, com configuração e práticas recomendadas operacionais da AWS integradas e sem plano de controle, nós ou complementos para você gerenciar. Ele se integra nativamente com a AWS e ferramentas de terceiros para fazer com que seja mais fácil para as equipes se concentrar na criação de aplicações, e não no ambiente.
### Desenvolvimento 
#### Compatibilidade com contêineres do Windows
O Amazon ECS oferece suporte ao gerenciamento de contêineres do Windows. Uma imagem de máquina da Amazon (AMI) de Windows otimizada para o Amazon ECS oferece performance aprimorada de inicialização de instância e contêiner, bem como visibilidade de métricas de CPU, utilização de memória e reservas.

#### AWS Copilot
A CLI do AWS Copilot é uma ferramenta que permite aos desenvolvedores criar, lançar e operar aplicações conteinerizadas prontas para produção no Amazon ECS e no AWS Fargate. O Copilot incorpora as práticas recomendadas, da infraestrutura à entrega contínua, e as disponibiliza aos clientes no conforto de sua linha de comando. Você também pode monitorar a integridade do seu serviço visualizando o status ou os logs do serviço, aumentar ou diminuir os serviços de produção e ativar um novo ambiente para testes automatizados.

#### Suporte a repositórios
O Amazon ECS pode ser usado com qualquer repositório de imagens do Docker ou registro privado do Docker acessível hospedado por terceiros, como o Docker Hub e o Amazon Elastic Container Registry (ECR). Basta especificar o repositório em uma definição de tarefas. O Amazon ECS recuperará as imagens apropriadas para os aplicativos.