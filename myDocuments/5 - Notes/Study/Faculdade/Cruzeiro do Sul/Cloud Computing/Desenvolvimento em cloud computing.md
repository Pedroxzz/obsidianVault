---
Index: "[[Cloud Computing]]"
---
# Apresentação
A computação em nuvem permite o fornecimento de serviços de computação, os quais incluem desde servidores até ambientes de desenvolvimento de software e o software propriamente dito.

Para começar a desenvolver softwares para computação em nuvem, é interessante conhecer os modelos de programação mais utilizados, os quais incluem, por exemplo, o MapReduce. Além disso, é importante entender como é feito o desenvolvimento utilizando o modelo PaaS e o fornecimento utilizando o SaaS.

Nesta Unidade de Aprendizagem, você vai aprender detalhes sobre os principais modelos de programação para nuvem. Além disso, você vai examinar o desenvolvimento de software e, por fim, traçar um paralelo entre os modelos PaaS e SaaS para adoção e utilização de computação em nuvem.

# Infográfico

O modelo de plataforma como um serviço (PaaS) foi criado com o intuito de suportar todo o processo de desenvolvimento de aplicações. Suas vantagens vão desde a redução do tempo de codificação até a gerência simplificada do ciclo de vida do aplicativo. Muitas têm sido as aplicações desenvolvidas utilizando esse modelo.

Após a fase de desenvolvimento, o aplicativo é disponibilizado utilizando outro modelo de nuvem, o modelo de software como um serviço (SaaS). Neste, o cliente pode acessar o aplicativo direto pelo navegador, sem baixar nenhum software para seu computador. Esses dois modelos auxiliam tanto o desenvolvedor quanto o cliente que vai utilizá-lo no futuro.

## Uso dos modelos PaaS e SaaS para desenvolvimento e fornecimento de software 
A computação em nuvem surgiu surgiu para auxiliar tantos os provedores quanto os clientes.
Cada modelo de serviços tem suas particularidades e aplicabilidade no contexto da internet.
Vejamos como os modelos PaaS e SaaS podem ser aplicados no desenvolvimento e fornecimento de softwares.

### Plataforma como Serviço (PaaS)
No PaaS, uma plataforma que suporta um conjunto de determinadas linguagens e tecnologias é fornecida. Nesse caso, a empresa pode alugar o serviço para comprar ou criar suas próprias aplicações. O acesso e o gerenciamento podem ser feitos pelo navegador de um cliente proprietário da empresa de computação em nuvem ou de algum ambiente de desenvolvimento integrado (IDE).

### Software como Serviço (SaaS)
No SaaS, um software é oferecido, e o cliente somente o utiliza. Esse software provavelmente foi desenvolvido utilizando um PaaS e agora está pronto e instalado na infraestrutura da nuvem. Na visão do cliente, não é possível gerenciar nem conhecer detalhes físicos de onde o software é executado, tais como rede, disco, sistema operacional, entre outros. Na maior parte das vezes, o cliente necessita de Internet e acessa o software via navegador.


### Aplicações que seguiram esses modelos
- SCRIBD
- Spotify
- COMCAST
- airbnb
- coursera
- Pinterest
- SOUNDCLOUD
- NETFLIX
- Sнаzам

O modelo PaaS auxilia no desenvolvimento de um software, automatizando a implantação e o teste e reduzindo o trabalho e os custos envolvidos com a etapa de desenvolvimento de uma aplicação. Já o modelo SaaS altera a maneira como o sistema é entregue. Utilizando esses modelos em conjunto, a empresa pode desenvolver e disponibilizar para os clientes o acesso ao seu sistema

# Na prática.
Um dos desafios que o desenvolvedor tem é entender o problema e decidir qual abordagem de computação em nuvem deve ser utilizada. Essas decisões podem variar de acordo com o tipo de aplicação e com os requisitos buscados.

Por exemplo, se segurança é um requisito do projeto, o uso de nuvens privadas deve ser considerado. Por sua vez, se a escalabilidade é importante, uma nuvem pública de um provedor conhecido é a melhor opção.

Neste Na Prática, você vai conhecer um estudo de caso com base no desenvolvimento de um algoritmo para comparar o gosto musical de usuários de um aplicativo de relacionamentos, e a empresa decidiu utilizar o serviço de computação em nuvem Amazon Lambda para hospedar.​​​

## Estudo de caso

A empresa suíça Classify é conhecida por seus aplicativos de localização de pessoas para encontros. Atualmente, seu aplicativo cruza dados de redes sociais, localizando pessoas geograficamente próximas.

Júlia foi contratada pela Classify para criar um algoritmo que, dado o ranking de músicas de determinada pessoa, consulta o banco de dados para encontrar pessoas com gostos similares. Júlia decidiu utilizar um algoritmo que conta inversões para fazer isso de forma eficiente.

Após Júlia desenvolver seu algoritmo, a empresa decidiu utilizar o serviço AWS Lambda para executar códigos sem ter que gerenciar os servidores, o que daria muito trabalho com o crescente aumento do número de usuários que o aplicativo vinha recebendo.

Para tanto, Júlia, que já utilizava em sua empresa outros serviços da Amazon, como o banco de dados DynamoDB, alterou seu código Python para que, a cada requisição do aplicativo para  calcular o ranking de músicas de duas pessoas, essa operação fosse enviada para execução no AWS Lambda. Assim, o número de requisições poderia tanto aumentar como diminuir que, automaticamente, o AWS Lambda escalaria a aplicação.

Após um conjunto de testes, Júlia e sua equipe perceberam que o algoritmo tinha funcionado e que a utilização do AWS Lambda facilitou a administração do aplicativo, auxiliando principalmente nos quesitos escalabilidade e disponibilidade.


# Saiba mais
## Veja por que o PaaS é a nova tendência para o crescimento do seu negócio
https://blog.cronapp.io/veja-por-que-o-paas-e-a-nova-tendencia-para-o-crescimento-do-seu-negocio/
## O que é e como lançar um _software_ como serviço (SaaS)
https://www.youtube.com/embed/mxHBmFv7mMM

## Desenvolvendo aplicações MapReduce
https://imasters.com.br/banco-de-dados/solucione-problemas-de-big-data-relacionados-a-nuvem-com-mapreduce