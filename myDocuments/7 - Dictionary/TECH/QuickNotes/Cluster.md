---
tags:
  - quicknotes
Index: "[[Dictionary]]"
---

Um cluster geralmente se refere a um grupo de recursos de computação que trabalham juntos para alcançar um objetivo comum. Dependendo do serviço, no caso da AWS, o conceito de cluster pode variar.

**Em todos esses casos, o termo "cluster" implica uma coleção de recursos que funcionam em conjunto para suportar tarefas ou serviços específicos, oferecendo escalabilidade, alta disponibilidade e capacidade de processamento distribuído.**

## Aqui estão alguns exemplos de clusters em diferentes serviços da AWS:
1. [[Amazon ECS]]
	- **Cluster ECS**: Um cluster no ECS é um grupo lógico de instancias de contêineres onde você pode executar tarefas e serviços. As instancias podem ser instancias do EC2 ou contêineres gerenciados pelo AWS Fargate. 
2. Amazon EKS (Elastic Kubernetes Service):
	- **Cluster EKS**: Um cluster EKS é um ambiente gerenciado para executar aplicações Kubernetes. O cluster consiste em um plano de controle gerenciado pela AWS e nós de trabalho (work nodes) que são executados em instâncias do EC2 ou Fargate. 
3. Amazon EMR (Elastic MapReduce):
	- **Cluster EMR**: Um cluster EMR é um conjunto de instâncias EC2 que trabalham juntas para executar grandes processos de dados, como análise de dados, processamento de big data com Hadoop, Spark, HBase, Presto, etc.
4. Amazon Redshift:
    - **Cluster Redshift**: Um cluster Redshift é um conjunto de nós (nodes) usados para armazenação e processamento de dados em um data warehouse. O cluster pode incluir nós de computação e um nó líder que gerencia as consultas e coordena a comunicação entre os nós de computação.
5. AWS ParallelCluster:
    - **Cluster ParallelCluster**: Um cluster ParallelCluster é uma ferramenta gerenciada pela AWS para criar e gerenciar clusters de computação de alta performance (HPC). Ele permite que você configure e implante clusters de computação para simulações científicas, análise de dados e outras cargas de trabalho intensivas em computação.