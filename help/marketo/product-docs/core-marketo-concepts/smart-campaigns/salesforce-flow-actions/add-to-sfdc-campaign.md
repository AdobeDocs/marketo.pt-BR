---
unique-page-id: 1147034
description: Adicionar à campanha SFDC - Documentação do Marketo - Documentação do produto
title: Adicionar à campanha da SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Adicionar à campanha da SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

## Visão geral {#overview}

Essa etapa do fluxo pode ser usada em campanhas do Marketo ou como uma única etapa do fluxo para adicionar pessoas como clientes em potencial em uma campanha do Salesforce. Se o lead ainda não existir no Salesforce, ele será sincronizado automaticamente e adicionado à campanha com o status especificado.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Uso {#usage}

1. Localize e selecione a campanha do Salesforce à qual deseja adicionar seus leads.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Se você não conseguir ver uma campanha do Salesforce na lista Campanha:
   >
   >  1. Verifique se [a sincronização da campanha está habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Confirme se o [Usuário de sincronização do Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) é um [Usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) no Salesforce.

   >[!TIP]
   >
   >Você pode usar a campanha do Salesforce [Meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) para facilitar a clonagem de programas.

1. Selecione o status do membro da campanha do Salesforce que você deseja atribuir aos clientes potenciais quando forem adicionados.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Se uma pessoa já for um membro líder da campanha do Salesforce, ela será ignorada e seu status NÃO será atualizado. Você pode usar [alterar o status em uma campanha do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md) em vez disso.
