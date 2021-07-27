---
description: Notas de versão atuais - Documentação do Marketo - Documentação do produto
title: Notas de versão atuais
source-git-commit: 97f6aeeb5c808df780b9b7bafd1bea5b1b805e5a
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 0%

---

# Notas de versão: Agosto de 2021 {#release-notes-aug-21}

Os seguintes recursos estão incluídos na versão de 21 de agosto. Verifique sua edição de Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage de Adobe para saber mais.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **20 de agosto de 2021**.

## Integração do Adobe Experience Platform {#adobe-experience-platform-integration}

* **Autenticação de usuário do Marketo Engage via Adobe**: A partir de setembro de 2021, os novos usuários do Marketo Engage com pacotes empresariais serão integrados usando as credenciais do usuário do Adobe ID. A migração dos usuários atuais para o sistema de identidade integrado não ocorrerá até meados de 2022 e nenhuma ação será necessária até novo aviso. A autenticação de usuário de identidade do Adobe permite que administradores de TI/segurança gerenciem várias instâncias de produto do Marketo Engage junto com outras soluções do Experience Cloud, bem como a configuração de SSO por meio de um console comum. Administradores podem gerenciar convenientemente grupos de usuários e direitos de usuário em um local.

## Automação de experiência {#experience-automation}

* **Aninhamento** da campanha executável: As campanhas executáveis agora também podem chamar outras campanhas executáveis, permitindo aninhá-las com até três níveis de profundidade. Isso permite consolidar ainda mais os fluxos operacionais comuns e melhora o gerenciamento do Smart Campaign.

* **Ação de fluxo único na página** Detalhes da pessoa: Execute ações de fluxo como enviar emails, alterar o proprietário da pessoa ou qualquer outra ação de campanha inteligente em pessoas individuais na página de detalhes da pessoa usando o menu de ação de fluxo sem alternar para a exibição de grade do banco de dados.

* **Exportação** de atividades personalizadas: A exportação de metadados agora é compatível com todos os objetos e respectivos metadados que podem ser usados para compartilhar, analisar e projetar seu modelo de dados de assinatura.

## Melhorias da API {#api-enhancements}

* **API** de metadados de campos personalizados: Simplifique a criação e o gerenciamento de campos personalizados no Marketo Engage para integrações de parceiros. Crie novos campos em um objeto de lead automaticamente e faça atualizações de campo em várias instâncias de Marketo Engage imediata e simultaneamente.

* **Filtragem** aprimorada: Várias APIs agora oferecem suporte para mais filtragem, como adicionar um filtro de intervalo de datas a ativos de email e campos de membros do programa. Agora é possível extrair apenas os dados atualizados dentro de um determinado período para as seguintes APIs...
   * Obter Membros do Programa
   * Obter emails
   * Extração de Atividade em Massa

* **API** de envio de formulário: Quando um endereço de email é duplicado em dois ou mais registros de lead, atualizamos o registro &quot;última atualização&quot; em vez de ignorá-lo completamente. Fornece paridade com a API do Forms 2.0.

* **API** de email: Recupere ativos de email campeão ou desafiante.

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **Visibilidade aprimorada para atividades de lead, contato, conta e oportunidade para usuários** do Salesforce CRM: O envolvimento com clientes potenciais durante longos ciclos de vendas é mais informado devido a um número maior de registros de envolvimento no Sales Insight. Os momentos interessantes, a atividade da Web, o email e as guias de pontuação mostram até 400 atividades em objetos de Lead, Contato, Conta e Oportunidade.

## SalesConnect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Limitação da conexão de email (GA)**: Melhore a capacidade de fornecimento de email e dimensione a comunicação personalizada de vendas com o controle da conexão de email para o Sales Connect. Essa nova tecnologia gerencia automaticamente o tempo de envio de emails para criar experiências ininterruptas para usuários do Exchange e Gmail. Diminua ou elimine o uso de aplicativos de envio de email em massa de terceiros e envie todos os seus emails do Sales Connect com confiança.

* **Insights** aprimorados da atividade de vendas: Capture e ative o envolvimento personalizado com base nas atividades anteriores da sua equipe de vendas. Novos atributos como Link de registro da chamada de vendas, Nome da campanha de vendas e Assunto do email de vendas podem ser usados em listas inteligentes Marketo Engage.  Essas atividades podem ser exportadas e relatadas por meio da API REST do Marketo Engage ou Exportar em massa e estão disponíveis em filtros e acionadores como restrições adicionais para listas inteligentes.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integração** Bizible LinkedIn Lead Gen Forms: Os profissionais de marketing agora podem executar a atribuição de receita em conversões que ocorrem quando o LinkedIn captura formulários de preenchimentos por meio de suas unidades de anúncio Forms de Geração de lead. Esses insights podem ser usados para otimizar o desempenho do formulário e os investimentos em mídia paga. O linkedIn Lead Gen Forms é uma das ofertas de mídia paga de mais rápido crescimento da LinkedIn e esse novo recurso está incluído em nossa integração do LinkedIn Ads com a Bizible. 
 
* **Painel** Velocity melhorado: Adicionamos uma nova métrica de velocidade e um filtro de painel para obter insights mais profundos. Esse painel é usado pelos profissionais de marketing para entender a velocidade de oportunidade e o avanço de cada estágio e a eficiência de diferentes formas de envolvimento de marketing e vendas.

* **Novo painel** de Jornada de cascata de coorte: Isso permitirá que os profissionais de marketing visualizem a progressão de um coorte selecionado por meio de um conjunto clássico de &quot;cascata de demanda&quot;, fornecendo uma compreensão rápida das taxas de conversão e o nexo de causalidade de conversão de estágio implícito em cada estágio.

## Integração Bizible com o Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Esta seção inclui novos recursos para usuários Bizible que concluíram sua migração para o Adobe Identity Management System (IMS). Se tiver migrado, você verá seu novo Adobe ID em Configurações da Bizible na guia Adobe ID . Todas as contas devem ser migradas até o final de 2021.

* **Integração Bizible com o Adobe Privacy Service**  (disponível em setembro de 2021): A integração da Bizible com o Privacy Service do Adobe centraliza a conformidade com as regulamentações críticas de privacidade de dados (como o GDPR) em todos os aplicativos Adobe Experience Cloud. Agora você pode aproveitar esse serviço e gerenciar todas as solicitações de privacidade centralmente para que as solicitações de alteração que entram na Bizible e outros produtos do Adobe sejam refletidas em todos os aplicativos.

* **Bizible em Adobe Unified Shell**: A adoção do Adobe Unified Shell pela Bizible fornece aos usuários novos recursos que aparecerão na barra de cabeçalho do aplicativo Bizible e incluem melhor acesso a recursos de suporte e switching de aplicativos. O Adobe Unified Shell ajuda a criar uma experiência consistente entre a Bizible e outros aplicativos Adobe Experience Cloud.

* **Propriedade de domínio Bizible e autogerenciamento**: Os usuários da Bizible podem aproveitar o Adobe Admin Console para gerenciar os domínios que desejam que a Bizible rastreie. Isso oferece autoatendimento a um processo manual anterior e fornece uma experiência consistente em como a propriedade e o rastreamento de domínio são gerenciados nos aplicativos Adobe Experience Cloud.

## Anúncios {#announcements}

* **Atualização das configurações** da ID universal de assinatura: Para dar suporte à futura integração do Marketo Engage e do Adobe Identity para os usuários existentes, todas as assinaturas do Marketo Engage serão unificadas na ativação do suporte à Universal ID.
