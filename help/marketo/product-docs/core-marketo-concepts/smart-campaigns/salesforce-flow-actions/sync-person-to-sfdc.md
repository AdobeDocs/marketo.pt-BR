---
unique-page-id: 1147027
description: Sincronizar pessoa com o SFDC - Documentação do Marketo - Documentação do produto
title: Sincronizar pessoa ao SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 6%

---

# Sincronizar pessoa ao SFDC {#sync-person-to-sfdc}

Esta etapa de fluxo inserirá as pessoas criadas pela Marketo como clientes potenciais no Salesforce CRM.

>[!NOTE]
>
>Disponível somente quando integrado com [!DNL Salesforce].

1. Por padrão, essa etapa do fluxo atribuirá aos proprietários de clientes potenciais com base nas regras de atribuição automática do Salesforce.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] exige que a pessoa tenha os campos Empresa e Sobrenome preenchidos. Caso contrário, ele rejeitará o registro de lead.

1. Você pode definir um usuário [!DNL Salesforce] específico ou uma fila de clientes potenciais como o proprietário principal.

   ![](assets/sync-person-to-sfdc-2.png)

   Ao usar essa etapa do fluxo, a pessoa é sincronizada como um cliente em potencial [!DNL Salesforce] imediatamente e não precisa aguardar a sincronização normal.

   >[!CAUTION]
   >
   >[!DNL Salesforce] não permite que &quot;Contatos&quot; sejam atribuídos a filas de clientes potenciais. Nesse caso, a Marketo criará um &quot;Lead&quot; duplicado em [!DNL Salesforce].
