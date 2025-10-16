---
description: Notas de versão - agosto de 2021 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Agosto de 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 1%

---

# Notas de versão: agosto de 2021 {#release-notes-aug-21}

Os seguintes recursos estão incluídos na versão de agosto de 2021. Verifique a edição do Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Adobe Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **20 de agosto de 2021**.

## Automação de experiência {#experience-automation}

* **Autenticação de usuário do Marketo Engage por meio da Adobe Identity**: em breve, novos usuários do Marketo Engage com pacotes Enterprise serão integrados usando as credenciais de usuário do Adobe ID. A migração dos atuais utilizadores para o sistema de identidade integrado só ocorrerá em meados de 2022 e não é necessária qualquer ação até nova ordem. A autenticação de usuário de identidade da Adobe permite que os administradores de TI/segurança gerenciem várias instâncias de produtos da Marketo Engage juntamente com outras soluções da Experience Cloud, além de configurar o SSO por meio de um console comum. Os administradores podem gerenciar convenientemente grupos de usuários e direitos de usuário em um único local.

* **Aninhamento de campanhas executáveis**: campanhas executáveis agora também podem chamar outras campanhas executáveis, permitindo que você as aninhe em até três níveis. Isso permite uma maior consolidação de fluxos operacionais comuns e melhora o gerenciamento do Smart Campaign.

* **Ação de fluxo única na página Detalhes da pessoa** (Disponível até 9 de setembro): execute ações de fluxo, como enviar email, alterar o proprietário da pessoa ou qualquer outra ação de campanha inteligente em pessoas individuais na página Detalhes da pessoa usando o menu de ação de fluxo sem alternar para a exibição de grade do banco de dados.

* **[Exportação de Atividades Personalizadas](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: a exportação de metadados agora oferece suporte a todos os objetos e respectivos metadados que podem ser usados para compartilhar, analisar e projetar seu modelo de dados de assinatura.

## Aprimoramentos na API {#api-enhancements}

* **Enviar API de Formulário**: quando um endereço de email é duplicado em dois ou mais registros de cliente potencial, atualizamos o registro &quot;última atualização&quot; em vez de ignorarmos completamente. Fornece paridade com a API do Forms 2.0.

* **API de email**: recupere ativos de email de campeão ou desafiante. Recupere ativos de email usando o filtro de intervalo de datas.

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## [!DNL Sales Insight] {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **Visibilidade aprimorada das atividades de cliente potencial, contato, conta e oportunidade para usuários do Salesforce CRM**: o engajamento com clientes potenciais durante longos ciclos de vendas é mais informado devido a um maior número de registros de engajamento em [!DNL Sales Insight]. As guias de momentos interessantes, atividade da Web, email e pontuação mostram até 400 atividades em objetos de cliente potencial, contato, conta e oportunidade.

## [!DNL Sales Connect] {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Limitação da Conexão de Email (Beta)**: melhore a capacidade de entrega de emails e dimensione a comunicação de vendas personalizada com a limitação da conexão de email para o Sales Connect. Esta nova tecnologia gerencia automaticamente o tempo de envio de email para criar experiências perfeitas para os usuários do [!DNL Exchange] e do Gmail. Diminua ou elimine o uso de aplicativos de envio de email de terceiros em massa e envie todos os seus emails do [!DNL Sales Connect] com confiança.

>[!NOTE]
>
>A limitação de email está disponível no Beta agora. [Saiba mais](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Insights Aprimorados da Atividade de Vendas**: capture e ative o envolvimento personalizado com base nas atividades anteriores de sua equipe de vendas. Novos atributos, como Link de registro de chamada de vendas, Nome da campanha de vendas e Assunto do email de vendas, podem ser usados nas listas inteligentes do Marketo Engage.  Essas atividades podem ser exportadas e relatadas por meio da API REST do Marketo Engage ou Exportação em massa e estão disponíveis em filtros e acionadores como restrições adicionais para smart lists.

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible]&#x200B;[!DNL LinkedIn] Integração do Forms com a Geração de Clientes Potenciais**: os profissionais de marketing agora podem realizar atribuição de receita em conversões que ocorrem quando [!DNL LinkedIn] captura preenchimentos de formulário por meio de suas unidades de anúncio do Forms de Geração de Clientes Potenciais. Esses insights podem ser usados para otimizar o desempenho do formulário e os investimentos em mídia paga. A Geração líder de Forms [!DNL LinkedIn] é uma das ofertas de mídia paga de crescimento mais rápido da [!DNL LinkedIn] e esse novo recurso está incluído na integração existente do [!DNL LinkedIn] Ads com o [!DNL Bizible].

* **Painel do Velocity aprimorado**: adicionamos uma nova métrica de velocidade e um novo filtro de painel para obter insights mais profundos. Esse painel é usado pelos profissionais de marketing para entender a velocidade do lead e da oportunidade estágio por estágio e a eficiência de diferentes formas de envolvimento de marketing e vendas.

* **Novo Painel de Jornada em cascata de coorte**: isso permitirá que os profissionais de marketing visualizem a progressão de uma coorte selecionada por meio de um conjunto clássico de estágios de &quot;cascata de demanda&quot;, fornecendo um rápido entendimento das taxas de conversão e da causalidade de conversão de estágio implícita em cada estágio.

## Integração do [!DNL Bizible] com o Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Esta seção inclui novos recursos para usuários do Bizible que concluíram a migração do Adobe Identity Management System (IMS). Se tiver migrado, você verá seu novo Adobe ID nas Configurações do [!DNL Bizible] na guia Adobe ID. Todas as contas devem ser migradas até o final de 2021.

* **[!DNL Bizible]Integração com o Adobe Privacy Service** (disponível em setembro de 2021): a integração do [!DNL Bizible] com o Adobe Privacy Service centraliza a conformidade com as regulamentações críticas de privacidade de dados (como o GDPR) em todos os aplicativos da Adobe Experience Cloud. Agora você pode aproveitar esse serviço e gerenciar todas as solicitações de privacidade centralmente para que as solicitações de alteração que entram no [!DNL Bizible] e em outros produtos da Adobe sejam refletidas em todos os aplicativos.

* **[!DNL Bizible]no Adobe Unified Shell**: a adoção do Adobe Unified Shell por [!DNL Bizible] fornece aos usuários novos recursos que aparecerão na barra de cabeçalho do aplicativo [!DNL Bizible] e incluirão melhor acesso aos recursos de suporte e à alternância de aplicativos. O Adobe Unified Shell ajuda a criar uma experiência consistente entre o [!DNL Bizible] e outros aplicativos da Adobe Experience Cloud.

* **[!DNL Bizible]Propriedade e Autogerenciamento do Domínio**: [!DNL Bizible] usuários podem aproveitar o Adobe Admin Console para gerenciar os domínios que o [!DNL Bizible] deseja rastrear. Isso leva o autoatendimento a um processo anteriormente manual e fornece uma experiência consistente sobre como a propriedade e o rastreamento de domínios são gerenciados nos aplicativos da Adobe Experience Cloud.

## Anúncios {#announcements}

* **Atualização das Configurações de Assinatura da Universal ID**: para oferecer suporte à futura integração da Marketo Engage e da Adobe Identity para usuários existentes, todas as assinaturas do Marketo Engage serão unificadas na habilitação do suporte à Universal ID. Mais informações [podem ser encontradas aqui](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar de lançamento de produto_**

[Webinário da versão de agosto de 2021 do Marketo Engage](https://engage.marketo.com/August21_Release_Webinar.html)
