---
unique-page-id: 2953469
description: SFDC Sync - Sincronização do Campaign - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização do Campaign
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 6%

---

# Sincronização do SFDC: sincronização de campanha {#sfdc-sync-campaign-sync}

Os Programas do Marketo podem ser sincronizados com [!DNL Salesforce] Campanhas. Esta é uma visão geral de como isso funciona.

## Por que devo sincronizar programas do Marketo com [!DNL Salesforce] campanhas? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Use os recursos avançados de um Programa Marketo.
* Mantenha os membros e seus status sincronizados entre um programa do Marketo e uma Campanha do [!DNL Salesforce].
* Toque nos recursos de relatório no Marketo e [!DNL Salesforce].

## Como um Programa Marketo e uma campanha [!DNL Salesforce] são sincronizados? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

No Marketo, você tem a opção de criar um mapeamento um para um entre um programa e uma campanha [!DNL Salesforce].

![](assets/image2015-7-8-9-3a43-3a8.png)

O **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** e o **[custo do período](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** na Marketo sincronizam com [!DNL Salesforce] como o **tipo de campanha** e o **custo real**. Esta sincronização está **unidirecional**, do Marketo para o [!DNL Salesforce].

Os **membros do programa** do Marketo e seus **[status de progressão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** são mantidos em sincronia com os **[!DNL Salesforce]membros da campanha** e os **status dos membros da campanha**. Esta é uma **sincronização bidirecional**, portanto, quaisquer alterações feitas no Marketo ou [!DNL Salesforce] serão refletidas em ambos os sistemas.

>[!NOTE]
>
>Se houver membros do programa Marketo que não existam em [!DNL Salesforce], a Marketo criará essas pessoas como clientes em potencial em [!DNL Salesforce].

## Quais são os acionadores/filtros relacionados às campanhas? {#what-are-the-triggers-filters-related-to-campaigns}

Gatilhos:

* Adicionado à campanha da SFDC
* Removido da campanha da SFDC
* O status é alterado na campanha da SFDC

Filtros:

* Membro da campanha da SFDC

## Posso adicionar Pessoas da Marketo à minha campanha do SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sim, use a [ação Adicionar ao fluxo de campanha do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Se essa pessoa não existir em [!DNL Salesforce], o Marketo a criará em [!DNL Salesforce] e a adicionará à campanha.

## Posso remover membros da minha campanha do SFDC usando o Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sim, use a ação de fluxo [Remover do SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md){target="_blank"}.

## Posso alterar o status do membro da campanha usando o Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sim, usar a [ação Alterar status no fluxo do SFDC Campaign](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.

## Por que não consigo ver nenhuma das minhas campanhas [!DNL Salesforce]? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Veja algumas coisas que você pode verificar:

1. Verifique se a [sincronização da campanha está habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Confirme se o seu [Usuário de sincronização do Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) é um [Usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) em [!DNL Salesforce].

>[!NOTE]
>
>Se a campanha [!DNL Salesforce] e o programa Marketo mapeado tiverem status de programa incompatíveis, você poderá receber uma mensagem de erro. Recomendamos que você [corresponda aos status do programa antes da sincronização](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronizar uma Campanha do SFDC com um Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}
>* [Noções básicas sobre a associação ao programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md){target="_blank"}
>* [Habilitar/Desabilitar a Sincronização de Campanha](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}
>* [Transformar o usuário de sincronização do Marketo em um usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}
