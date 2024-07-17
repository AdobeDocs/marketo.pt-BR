---
unique-page-id: 1147027
description: Sincronizar pessoa ao SFDC - Documentação do Marketo - Documentação do produto
title: Sincronizar pessoa à SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 6%

---

# Sincronizar pessoa à SFDC {#sync-person-to-sfdc}

Esta etapa do fluxo inserirá as pessoas criadas pela Marketo como clientes em potencial no seu Salesforce CRM.

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

1. Por padrão, essa etapa do fluxo atribuirá aos proprietários de clientes potenciais com base nas regras de atribuição automática do Salesforce.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >O Salesforce exige que a pessoa tenha os campos Empresa e Sobrenome preenchidos. Caso contrário, ele rejeitará o registro de lead.

1. Você pode definir um usuário do Salesforce ou uma fila de clientes potenciais específica como o proprietário do cliente potencial.

   ![](assets/sync-person-to-sfdc-2.png)

   Ao usar essa etapa do fluxo, a pessoa é sincronizada como um lead do Salesforce imediatamente e não precisa aguardar a sincronização normal.

   >[!CAUTION]
   >
   >O Salesforce não permite que &quot;Contatos&quot; sejam atribuídos a filas de clientes potenciais. Nesse caso, a Marketo criará um &quot;Lead&quot; duplicado no Salesforce.
