---
unique-page-id: 1147034
description: Adicionar à campanha SFDC - Documentação do Marketo - Documentação do produto
title: Adicionar à campanha da SFDC
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 5%

---

# Adicionar à campanha da SFDC {#add-to-sfdc-campaign}

Essa etapa do fluxo pode ser usada em campanhas Marketo Engage ou como uma única etapa do fluxo para adicionar pessoas como leads em uma campanha do Salesforce. Se o lead ainda não existir no Salesforce, ele será sincronizado automaticamente e adicionado à campanha com o status especificado.

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

![](assets/add-to-sfdc-campaign-1.png)

## Uso {#usage}

1. Localize e selecione a campanha do Salesforce à qual deseja adicionar seus leads.

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >Se você não conseguir ver uma campanha do Salesforce na lista de campanhas:
   >
   >  1. Verifique se a [sincronização da campanha está habilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}.
   >  1. Confirme se o seu [Usuário de sincronização do Marketo](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} é um [Usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} no Salesforce.

   >[!TIP]
   >
   >Você pode usar a campanha [Meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} do Salesforce para facilitar a clonagem de programas.

1. Selecione o status do membro da campanha do Salesforce que você deseja atribuir aos clientes potenciais quando forem adicionados.

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >Se uma pessoa já for um membro líder da campanha do Salesforce, ela será ignorada e seu status NÃO será atualizado. Em vez disso, você pode usar [alterar seu status em uma campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}.
