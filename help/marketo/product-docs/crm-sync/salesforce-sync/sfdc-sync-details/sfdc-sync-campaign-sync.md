---
unique-page-id: 2953469
description: Sincronização SFDC - Sincronização de Campanha - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de Campanha
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de campanha {#sfdc-sync-campaign-sync}

Programas de marketing podem ser sincronizados com o Salesforce Campanha. Esta é uma visão geral de como isso funciona.

## Por que devo sincronizar programas de marketing com o Salesforce campanha? {#why-should-i-sync-marketo-programs-with-salesforce-campaigns}

* Use os recursos avançados de um Programa de marketing.
* Mantenha os membros e seu status sincronizados entre um programa do Marketo e uma Campanha do Salesforce.
* Toque nos recursos do relatórios no Marketo e no Salesforce.

## Como um Programa de marketing e uma campanha do Salesforce são sincronizados? {#how-is-a-marketo-program-and-a-salesforce-campaign-synced}

No Marketing, você tem a opção de criar um mapeamento de um para um entre um programa e uma campanha do Salesforce.

![](assets/image2015-7-8-9-3a43-3a8.png)

O **[canal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)** e **[custo do período](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-period-costs.md)** no Marketo sincronizam com o Salesforce como **tipo de campanha** e **custo real**. Essa sincronização é **unway**, de Marketo a Salesforce.

Os membros do programa Marketo **e seus**[ status de progressão ](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)**são mantidos em sincronia com os** membros da campanha Salesforce **e** status de membro da campanha **.** Essa é uma **sincronização bidirecional**, portanto, todas as alterações feitas no Marketo ou no Salesforce são refletidas em ambos os sistemas.

>[!NOTE]
>
>Se há membros do programa Marketo que não existem no Salesforce, Marketo cria essas pessoas como líderes no Salesforce.

## Quais são os acionadores/filtros relacionados ao campanha? {#what-are-the-triggers-filters-related-to-campaigns}

Acionadores:

* Adicionado à Campanha SFDC
* Removido da Campanha SFDC
* O status é alterado na Campanha SFDC

Filtros:

* Membro da Campanha SFDC

## Posso adicionar Marketo People à minha campanha SFDC? {#can-i-add-marketo-people-to-my-sfdc-campaign}

Sim, use a ação [Adicionar ao fluxo de campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/add-to-sfdc-campaign.md). Se essa pessoa não existir em Salesforce, Marketo a criará em Salesforce e o adicionará à campanha.

## Posso remover membros da minha campanha SFDC usando o Marketo? {#can-i-remove-members-from-my-sfdc-campaign-using-marketo}

Sim, use a ação [Remover do fluxo de Campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/remove-from-sfdc-campaign.md).

## Posso alterar o status do membro da campanha usando o Marketo? {#can-i-change-campaign-member-status-using-marketo}

Sim, use [Alterar status na ação de fluxo de Campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).

## Por que não consigo ver nenhuma das minhas campanhas do Salesforce? {#why-cant-i-see-any-of-my-salesforce-campaigns}

Estas são as coisas que você pode verificar:

1. Certifique-se de que [sincronização de campanha esteja ativada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
1. Confirme se seu [usuário de sincronização de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) é um [usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) no Salesforce.

>[!NOTE]
>
>Se sua campanha do Salesforce e o programa do Marketo mapeado tiverem status de programa incompatíveis, você poderá receber uma mensagem de erro. Recomendamos que você [corresponda aos status do programa antes da sincronização](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md).

>[!MORELIKETHIS]
>
>* [Sincronizar uma Campanha SFDC com um Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md)
>* [Compreensão da associação ao Programa](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md)
>* [Ativar/desativar sincronização de Campanha](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)
>* [Tornar usuário de sincronização de marketing um usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)

