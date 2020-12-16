---
unique-page-id: 1147027
description: Sincronizar pessoa com SFDC - Documentos do Marketing - Documentação do produto
title: Sincronizar Pessoa com SFDC
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# Sincronizar Pessoa com SFDC {#sync-person-to-sfdc}

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

## Visão geral {#overview}

Esta etapa de fluxo inserirá pessoas criadas pelo Marketing como clientes potenciais no seu CRM do Salesforce.

![](assets/sync-person-to-sfdc.png)

## Uso {#usage}

1. Por padrão, essa etapa de fluxo será atribuída aos proprietários principais com base nas regras de atribuição automática do Salesforce.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >O Salesforce exige que a pessoa tenha campos Empresa e Sobrenome preenchidos. Caso contrário, rejeitará o registro de cliente potencial.

1. Você pode definir um usuário ou fila de cliente potencial específica do Salesforce como proprietário do cliente potencial.

   ![](assets/sync-person-to-sfdc-2.png)

   Ao usar essa etapa de fluxo, a pessoa é sincronizada como um líder Salesforce imediatamente e não precisa aguardar a sincronização regular.

   >[!CAUTION]
   >
   >O Salesforce não permite que &quot;Contatos&quot; sejam atribuídos a filas de cliente potencial. Neste caso, Marketo criará um duplicado &quot;Lead&quot; no Salesforce.

