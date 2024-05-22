#dicty #sec 
[[_DICTY_]]

# DNS
O DNS (Domain Name System - Sistema de nome de domínio) converte nomes de domínio legíveis por humanos (por exemplo, www,amazon.com) em endereços IP legíveis por máquinas (por exemplo, 192.0.2.44)

## Fundamentos do DNS
Todos os computadores da internet, abrangendo de smartphones ou laptops a servidores que distribuem conteúdo para grandes websites do comércio, se encontram e se comunicam entre si usando números. Esses numero são conhecidos como **endereços IP**. Ao abrir um navegador e acessar um site, você não precisa lembrar-se de um longo número nem digita-lo. Em vez disso, você poderá informar um **nome de domínio**.

Um serviço DNS, como o [[Amazon Route 53]], é um serviço globalmente distribuído que converte nomes legíveis por humanos, como www,exemplo.com, em endereços IP numéricos como 192.0.2.1, usados pelos computadores para se conectarem entre si. O sistema DNS convertem solicitações de nomes em endereços IP, controlando servidor um usuário final alcançara quando digitar um nome de domínio no navegador web. Essas solicitações são chamadas **consultas**.

## Tipos de serviços DNS
### DNS autoritativo
Disponibiliza um mecanismo de atualização que os desenvolvedores usam para gerenciar seus nomes DNS Públicos. Em seguida, ele responde a consultas do DNS, convertendo nomes de domínio em endereços IP de forma que os computadores possam se comunicar entre si.

### DNS Recursivo
Geralmente, os clientes não fazem consultas diretamente para os serviços DNS autoritativos. Em vez disso, eles se conectam de modo geral a outro tipo de serviços DNS conhecido como **resolvedor** ou **DNS Recursivo**. Ele age como o concierge de um hotel: embora não tenha nenhum registro DNS, ele atua como um intermediário que pode obter informações de DNS por você. Se um DNS recursivo tiver a referencia do DNS armazenado em cache, ou armazenada durante um período, ele responderá a consulta do DNS ao disponibilizar as informações sobre a origem ou o IP. Caso contrario, ele encaminhará a consulta para um ou mais servidores DNS autoritativos para encontrar as informações. 

---
## Como o DNS direciona o tráfego para a sua aplicação web?

O diagrama a seguir disponibiliza uma visão geral sobre como os serviços DNS recursivos e autoritativos funcionam em conjunto para direcionar um usuário final para o seu site ou aplicação.
![[dnsExample.png]]

1. Um usuario abre o navegador, digita www,exemplo.com na barra de endereços e aperta Enter.

2. A solicitação é direcionada para um resolvedor DNS, que geralmente é geralmente gerenciada pelo ISP (Internet Service Provider) do usuario, como um provedor de internet a cabo, um provedor de banda larga DSL ou rede corporativa.

3. O resolvedor DNS do ISP encaminha a solicitação, que sai de da url e passa para um serviço de nome raiz DNS

4. O resolvedor DNS do ISP encaminha novamente a solicitação da url, mas desta vez para um dos servidores de nome [[TLD]] de dominios .com. O servidor de dome dos dominios responde a solicitação com os nomes dos quatros servidores de nome do Amazon Route 53 que estão associados ao domínio.