---
unique-page-id: 2953469
description: Sincronização SFDC - Sincronização do Campaign - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização do Campaign
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 5%

---

# Sincronização SFDC: Sincronização de Campanha {#sfdc-sync-campaign-sync}

Os programas de Marketo Engage podem ser sincronizados com as Campanhas do Salesforce. Aqui está uma visão geral de como isso funciona.

## Por que devo sincronizar programas do Marketo com campanhas do Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Use os recursos avançados de um Programa Marketo.
* Mantenha os membros e seus status sincronizados entre um programa do Marketo e uma campanha do Salesforce.
* Aproveite os recursos de relatórios no Marketo e Salesforce.

## Como um programa do Marketo e uma campanha do Salesforce são sincronizados? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

No Marketo, você tem a opção de criar um mapeamento um para um entre um programa e uma campanha do Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

A variável **[channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}** and **[period cost](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md){target="_blank"}** na sincronização do Marketo com o Salesforce como o **tipo de campanha** e **custo real**. Esta sincronização está **unidirecional**, do Marketo para o Salesforce.

Marketo **membros do programa** e seus **[status de progressão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}** são mantidos em sincronia com a **Membros da campanha do Salesforce** e **status dos membros da campanha**. Este é um **sincronização bidirecional**, portanto, quaisquer alterações feitas no Marketo ou no Salesforce serão refletidas em ambos os sistemas.

>[!NOTE]
>
>Se houver membros do programa Marketo que não existam no Salesforce, a Marketo criará essas pessoas como clientes em potencial no Salesforce.

## Quais são os acionadores/filtros relacionados às campanhas? {#what-are-the-triggers-filters-related-to-campaigns}

Gatilhos:

* Adicionado à campanha da SFDC
* Removido da campanha da SFDC
* O status é alterado na campanha da SFDC

Filtros:

* Membro da campanha da SFDC

## Posso adicionar pessoas da Marketo à minha campanha do SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sim, use o [Adicionar à ação de fluxo de campanha do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md){target="_blank"}. Se essa pessoa não existir no Salesforce, o Marketo a criará no Salesforce e a adicionará à campanha.

## Posso remover membros da minha campanha do SFDC usando o Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sim, use o [Remover da ação de fluxo de campanha do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Posso alterar o status do membro da campanha usando o Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sim, use o [Alterar status na ação de fluxo de campanha do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Por que não consigo ver nenhuma das minhas campanhas do Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Veja algumas coisas que você pode verificar:

1. Verifique se [a sincronização da campanha está habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
1. Confirme se o [Usuário de sincronização do Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} is a [Marketing User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} no Salesforce.

>[!NOTE]
>
>Se sua campanha do Salesforce e o programa Marketo mapeado tiverem status de programa incompatíveis, você poderá receber uma mensagem de erro. Recomendamos que você [corresponder aos status do programa antes da sincronização](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Sincronizar uma campanha SFDC com um programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Noções básicas sobre a associação ao programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Ativar/desativar a sincronização do Campaign](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Transformar o usuário da sincronização do Marketo em um usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
