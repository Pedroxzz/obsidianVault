---
tags:
  - aws
---

**S3 Intelligent-Tiering**: Para dados com padrões de acesso desconhecidos ou imprevisíveis, movendo automaticamente os dados entre duas camadas de acesso (frequente e infrequente) com base nos padrões de acesso.

---

A Amazon S3 Intelligent-Tiering é o primeiro armazenamento em nuvem que reduz automaticamente os custos de armazenamento em um nível de objeto granular, movendo automaticamente os dados para o nível de acesso mais econômico com base na frequência de acesso , sem impacto sobre a performance, taxas de recuperação ou sobrecarga operacional. A S3 Intelligent-Tiering oferece latência de milissegundos e alta performance de taxa de transferência para dados acessados com muita frequência, com pouca frequência e raramente acessados nos níveis Frequent Access, Infrequent Access e o Archive Instant Access.

Para garantir uma pequena taxa mensal de automação e monitoramento de objetos, O S3 Intelligent-Tiering monitora os padrões de acesso e move automaticamente os objetos que não foram acessados para níveis de acesso de custo inferior. O S3 Intelligent-Tiering armazena objetos automaticamente em **três níveis de acesso: um nível que é otimizado para acesso frequente, um nível de custo 40% mais baixo que é o otimizado para acesso não frequente e um nível de custo 68% mais baixo otimizado para dados raramente acessados.**
Por uma pequena cobrança mensal de monitoramento e automação por objeto, a S3 Intelligent-Tiering monitora padrões de acesso e move objetos que não foram acessados por mais de 30 dias consecutivos para o nível Infrequent Access e, agora, após 90 dias sem acesso, para o novo nível Archive Instant Access. Para dados que não exigem recuperação imediata, você pode configurar o S3 Intelligent-Tiering para monitorar e mover automaticamente objetos que não são acessados por 180 dias ou mais para o nível Deep Archive Access para obter até 95% de economia de custo de armazenamento.

	Nenhuma taxa adicional de camada se aplica quando objetos são movidos entre as camadas de acesso na categoria de armazenamento S3 Intelligent-Tiering.


Principais Recursos:
- Economia automática de custos para dados com padrões de acesso desconhecidos ou variáveis 

- Os níveis de acesso frequente e infrequente têm as mesmas baixas latência e performance de alto throughput do S3 Standard 

- O nível de acesso infrequente economiza até 40% em custos de armazenamento 

- O nível Archive Instant Acess econimiza até 68% em custos de armazenamento

- Ativa recursos de arquivamento e acesso para arquivamento profundo têm a mesma performance que as classes Glacier e Glacier Deep Archive e economizam até 95% para objetos raramente acessados

- Projetado para oferecer disponibilidade de 99,9% com um SLA de disponibilidade de 99%

- Pequena cobrança mensal de monitoramento e automação

- Sem sobrecarga operacional, sem encargos de ciclo de vida, sem encargos de recuperação e sem duração mínima de armazenamento

- Objetos menores que 128KB podem ser acessados na S3 Intelligent-Tiering, mas sempre serão cobrados pelas taxas de camadas de acesso frequente, sem cobrança de monitoramento de automação
