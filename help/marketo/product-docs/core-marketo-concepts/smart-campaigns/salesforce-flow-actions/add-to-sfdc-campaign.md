---
unique-page-id: 1147034
description: Adicionar à Campanha SFDC - Documentos do Marketing - Documentação do produto
title: Adicionar à Campanha SFDC
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Adicionar à Campanha SFDC {#add-to-sfdc-campaign}

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

## Visão geral {#overview}

Essa etapa de fluxo pode ser usada no Marketing campanha ou como uma única etapa de fluxo para adicionar pessoas como clientes potenciais em uma campanha do Salesforce. Se o cliente potencial ainda não existir no Salesforce, ele será sincronizado e adicionado automaticamente à campanha com o status especificado.

![](assets/image2014-9-22-15-3a43-3a36.png)

## Uso {#usage}

1. Localize e selecione a campanha do Salesforce à qual deseja adicionar seus clientes potenciais.

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >Se você não conseguir ver uma campanha do Salesforce na lista da Campanha:
   >
   >  1. Certifique-se de que [sincronização de campanha esteja ativada](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md).
   >  1. Confirme se seu [usuário de sincronização de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) é um [usuário de marketing](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md) no Salesforce.


   >[!TIP]
   >
   >Você pode usar a campanha do Salesforce [Meus tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) para facilitar a clonagem de programas.

1. Selecione o status do membro da campanha do Salesforce que você deseja atribuir aos clientes potenciais quando eles forem adicionados.

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >Se uma pessoa já for um membro líder da campanha Salesforce, ela será ignorada e seu status NÃO será atualizado. Você pode usar [alterar seu status em uma campanha SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md).
