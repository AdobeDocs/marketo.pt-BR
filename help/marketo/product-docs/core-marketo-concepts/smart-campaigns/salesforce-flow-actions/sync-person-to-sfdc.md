---
unique-page-id: 1147027
description: Sincronizar pessoa com o SFDC - Documentos do Marketo - Documentação do produto
title: Sincronizar pessoa à SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 6%

---

# Sincronizar pessoa à SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

## Visão geral {#overview}

Essa etapa de fluxo inserirá pessoas criadas pela Marketo como leads em seu CRM do Salesforce.

![](assets/sync-person-to-sfdc.png)

## Uso {#usage}

1. Por padrão, essa etapa do fluxo será atribuída aos proprietários de clientes potenciais com base nas regras de atribuição automática do Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >O Salesforce requer que a pessoa tenha campos Empresa e Sobrenome preenchidos. Caso contrário, ele rejeitará o registro de lead.

1. Você pode definir um usuário ou fila de lead específica do Salesforce como proprietário do lead.

   ![](assets/sync-person-to-sfdc-2.png)

   Ao usar essa etapa de fluxo, a pessoa é sincronizada como um lead do Salesforce imediatamente e não precisa aguardar a sincronização regular.

   >[!CAUTION]
   >
   >O Salesforce não permite que &quot;Contatos&quot; sejam atribuídos a filas de lead. Nesse caso, a Marketo criará uma duplicata &quot;Lead&quot; no Salesforce.
