---
unique-page-id: 1147034
description: Adicionar à campanha SFDC - Documentos do Marketo - Documentação do produto
title: Adicionar à campanha da SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 4%

---

# Adicionar à campanha da SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

## Visão geral {#overview}

Essa etapa do fluxo pode ser usada em campanhas do Marketo ou como uma única etapa do fluxo para adicionar pessoas como leads em uma campanha do Salesforce. Se o lead ainda não existir no Salesforce, será sincronizado e adicionado automaticamente à campanha com o status especificado.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Uso {#usage}

1. Localize e selecione a campanha do Salesforce à qual deseja adicionar seus leads.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Se você não conseguir ver uma campanha do Salesforce na lista Campanha:
   >
   >  1. Certifique-se de que a [sincronização de campanha está ativada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Confirme se seu [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) é um [Marketing User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) no Salesforce.


   >[!TIP]
   >
   >Você pode usar o Salesforce campaign [My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) para facilitar a clonagem de programas.

1. Selecione o status do membro da campanha do Salesforce que você deseja atribuir aos leads quando eles forem adicionados.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Se uma pessoa já for um membro líder da campanha do Salesforce, ela será ignorada e seu status NÃO será atualizado. Em vez disso, você pode usar [alterar seu status em uma campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).
