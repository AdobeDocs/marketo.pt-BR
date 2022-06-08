---
unique-page-id: 2953469
description: Sincronização SFDC - Sincronização de Campanha - Documentos Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Campanha
exl-id: 62435e00-9c59-4dee-a9b7-ccf1d1f41b78
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 5%

---

# Sincronização SFDC: Sincronização de campanha {#sfdc-sync-campaign-sync}

Os Programas Marketo podem ser sincronizados com as Campanhas do Salesforce. Esta é uma visão geral de como isso funciona.

## Por que devo sincronizar programas Marketo com campanhas do Salesforce? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Use os recursos avançados de um Programa Marketo.
* Mantenha os membros e seu status sincronizados entre um programa do Marketo e uma Campanha do Salesforce.
* Toque nos recursos de relatórios no Marketo e no Salesforce.

## Como um Programa Marketo e uma campanha do Salesforce são sincronizados? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

No Marketo, você tem a opção de criar um mapeamento de um para um entre um programa e uma campanha do Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

O **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** e **[custo do período](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** no Marketo, sincronize com o Salesforce como o **tipo de campanha** e **custo real**. Esta sincronização é **uma via**, do Marketo para o Salesforce.

Marketo **membros do programa** e seus **[status de progressão](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)** são mantidas em sincronia com o **Membros da campanha Salesforce** e **status dos membros da campanha**. Isso é uma **sincronização bidirecional**, portanto, todas as alterações feitas no Marketo ou no Salesforce são refletidas em ambos os sistemas.

>[!NOTE]
>
>Se houver membros no programa Marketo que não existam no Salesforce, o Marketo criará essas pessoas como leads no Salesforce.

## Quais são os acionadores/filtros relacionados às campanhas? {#what-are-the-triggers-filters-related-to-campaigns}

Gatilhos:

* Adicionado à campanha da SFDC
* Removido da campanha da SFDC
* O status é alterado na campanha da SFDC

Filtros:

* Membro da campanha da SFDC

## Posso adicionar Pessoas do Marketo à minha campanha SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sim, use o [Adicionar à ação de fluxo de campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Se essa pessoa não existir no Salesforce, o Marketo a criará no Salesforce e o adicionará à campanha.

## Posso remover membros da minha campanha SFDC usando o Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sim, use o [Remover da ação de fluxo de campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## É possível alterar o status do membro da campanha usando o Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sim, use o [Alterar status na ação de fluxo de campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Por que não posso ver nenhuma das minhas campanhas do Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Veja coisas que você pode verificar:

1. Certifique-se de que o [a sincronização de campanha está ativada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Confirme que a [Usuário do Marketo Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) é um [Usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) em Salesforce.

>[!NOTE]
>
>Se sua campanha do Salesforce e o programa Marketo mapeado tiverem status de programa incompatíveis, você poderá receber uma mensagem de erro. Recomendamos que você [corresponder aos status do programa antes da sincronização](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronizar uma campanha SFDC com um programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Compreensão da assinatura do programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Ativar/desativar sincronização de campanha](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Tornar o usuário do Marketo Sync um usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

