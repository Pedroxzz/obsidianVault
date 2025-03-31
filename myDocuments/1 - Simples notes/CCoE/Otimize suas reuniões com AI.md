---
tags:
  - "#aws"
---
# Desafios das Reuniões atuais

1 - Fazer anotações e participar ativamente de forma simunltânea
2- Buscar informações em tempo real
3 - Atualizar participantes ausentes ou atrasados
4 - Barreira linguistica
5 - Documentaçãp pés reunião

# Live Meeting Assistant (LMA)
## O que é ?
O Live Meeting Assistant LMA é uma solução que utiliza inteligência artificial para transcrever reuniões em tempo real. gerar resumos, identificar tópicos e extrair insights, proporcionando aos participantes um conteúdo mais rico e informativo
- Amazon Transcribe
- Amazon Bedrock
- Amazon Q Bussiness

## Principais características do LMA
### Transcrição ao Vivo com a Atribuição do Palestrante
O LMA utiliza o Amazon Transcribe para converter o áudio em texto em tempo real. Ele permite que você configure vocabulários personalizados e recursos de modelo de idioma

### Tradução ao Vivo em até 75 idiomas 
O LMA utiliza o Amazon Transcribe para traduzir cada segmento da conversa para o idioma que você escolher 

### Ok, Assistant!
O LMA utiliza o Amazon Q Bussiness, Knowledge Bases ou LLMs do Amazon Bedrock para fornecer respostas as perguntas ao vivo por meio de fontes confiáveis 

### Chatbot
O LMA conta com o Meeting Assistant Bot, que permite ao usuário esclarecer dúvidas durante ou após a reunião, utilizando o Amazon Bedrock para responder com base na transcrição.

Cada bloco de ação pode ser personalizado com prompts criados pelo próprio usuário e integrados ao sistema.

### Meeting Query Tool
O LMA armazena todas as transcrições e resumos das suas reuniões em uma base de conhecimento do Bedrock separada e fornece uma interface de bate-papo onde você pode pesquisar respostas e referências em todas as suas reuniões.

### Inventário
Após o termino da reunião, o LMA disponibiliza um inventário com um histórico de todas as reuniões realizadas, por meio de uma lista pesquisável,

### Arquitetura
![[LMA Arquiteura.png]]

## Implantação: Pré-Registros
### Essenciais:
- Acesso a uma conta da AWS
- Usuario do AWS IAM com permissões para cirar e gerenciar os recusos e componentes necessários para este aplicativo.
- Acesso aos modelos do Bedrock
### Opcionais:
- Criação de uma base de conhecimento;
- Utilização de uma base de conhecimento ou o uso de um aplicativo Amazon Q Business já existente

## Como subir a infraestrutura ?
### De forma rápida, fácil e econômica:
- Acessar o link:
- Escolher em qual região você deseja implantar a sua stack do CloudFormation

| Região                            | Botão de fácil implantação |
| --------------------------------- | -------------------------- |
| Leste dos EUA (Norte da Vírgínia) | Launch Stack               |
| Oeste dos EUA (Oregon)            | Launch Stack               |
| AP Sudeste (Sydney)               | Launch Stack               |

### Preenchimento da Stack:
1- Web UI Authentication
Admin Email Address
Authorized Account Email Domain(s)

2. Meeting Assist Options
Meeting Assist Service:
- BEDROCK_LLM
- BEDROCK_KNOWLEDGE BASE (Use Existing) ou (Create)
- BEDROCK_AGENT (Use Existing)
- Q_BUSINESS (Use Existing)
- BEDROCK_AGENT_WITH_KNOWLEDGE_BASE (Create)

4.  Meeting Assist Wake Phrase Regular Expression
(OK\Okay){,.!} * {Aa}ssistant ou personalizar da forma que você preferir

5. Retention Settings
- Meeting Record Expiration in Days
- Transcription Expiration in Days
- Audio Recording Expiration in Days
- CloudWatch Logs Expiration in Days

6. Transcript Event Processing Comnfiguration
End of Call Transcript Summary
- Amazon Bedrock - Preencher o campo **<mark style="background: #FFB8EBA6;">BedrockModelID</mark>**
- AWS Lambda - Preencher o campo **<mark style="background: #FFB8EBA6;">Lambda Hook Function ARN</mark>**

7. Amazon Transcribe Configuration
- Language for Transcription
- TranscribeLanguageOptions
	- TranscribePreferredLanguage - importante deixar esse campo vazio, para que o LMA não venha te ignorar quando você utilizar o comando OK, ASSISTANT!

8. Para todos os outros parâmetros, use os valores padrão
Você poderá utilizar a pilha novamente depois sem perder nenhum dos seus dados

9. Marque as caixas de confirmação e selecione CRIAR PILHA
As pilhas levam cerca de 35-40 minutos para serem implantadas. O status da pilha principal deve constar como CREATE_COMLPETE quando tudo é implantado

# Personalização do LMA
## Principais Recursos:
1. Enable Content Reduction for Transcripts
2. Transcription Custom Vocabulary Name
3. Personalização dos Prompts
4. Código-fonte disponível no Github

Amazon Transcribe - Amazon DynamoDB - AWS CloudFormation

# Monitoramento e Solução de Problemas
## Pontos Importantes:
1. Falha no CloudFormation
2. VPCs
3. Amazon Transcribe
4. Transcript Knowledge Base

O LMA possui integração ao Amazon CloudWatch Logs, para monitorar todos os serviços que compõem sua arquitetura.

# Custos
- Custos Fixos 
- $250-300 mensais
- Custos variáveis

# Atualizar e Deletar a Stack
## Atualizar:
- Acesso o CloudFormation e selecionar a sua pilha LMA existente
- Clique em Atualizar
- Após finalizar as alteraçõs, clique em <mark style="background: #FFB8EBA6;">Substituir modelo atual</mark>

## Deletar
- Acesso o CloudFormation e selecionar a sua Pilha LMA já existente
- Clique em Deletar
- Alguns recursos precisam ser excluídos manualmente, como Bucket S3, DynamoDB e os grupos CloudWatch Logs