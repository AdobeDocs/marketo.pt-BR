---
unique-page-id: 1147031
description: Excluir pessoa do SFDC - Documentos do Marketing - Documentação do produto
title: Excluir Pessoa do SFDC
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# Excluir Pessoa do SFDC {#delete-person-from-sfdc}

Se você precisar remover um conjunto específico de clientes potenciais do Salesforce, mas deixá-los como pessoas no Marketo, poderá usar a ação Excluir pessoa do fluxo SFDC.

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

1. No Banco de Dados, clique na pessoa que deseja remover do Salesforce. Em seguida, clique em **Ações da pessoa** e selecione **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Selecione **Excluir Pessoa do SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Verifique se a configuração **Excluir no Marketo** é **false** e clique em **Executar agora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Depois que a etapa de fluxo for executada, sua pessoa não será mais líder no Salesforce, mas permanecerá no Marketo.

   >[!CAUTION]
   >
   >Se você definir **Excluir no Marketo** como **true** e excluir as pessoas do Marketo e os clientes potenciais do Salesforce, elas desaparecerão para sempre. Isto não pode ser desfeito.
