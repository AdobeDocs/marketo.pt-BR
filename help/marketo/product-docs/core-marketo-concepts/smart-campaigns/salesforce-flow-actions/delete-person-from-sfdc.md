---
unique-page-id: 1147031
description: Excluir pessoa do SFDC - Documentos do Marketo - Documentação do produto
title: Excluir pessoa da SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Excluir pessoa da SFDC {#delete-person-from-sfdc}

Se você precisar remover um conjunto específico de leads do Salesforce, mas deixá-los como pessoas no Marketo, poderá usar a ação Excluir pessoa do SFDC em fluxo.

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

1. No Banco de Dados, clique na pessoa que deseja remover do Salesforce. Em seguida, clique em **Ações da pessoa** e selecione **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Selecionar **Excluir pessoa do SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Certifique-se de que o **Excluir no Marketo** é **false**, depois clique em **Executar agora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Depois que a etapa do fluxo for executada, sua pessoa não será mais líder no Salesforce, mas permanecerá no Marketo.

   >[!CAUTION]
   >
   >Se você definir **Excluir no Marketo** para **true** e exclua as pessoas do Marketo e os leads do Salesforce, elas foram para sempre. Isso não pode ser desfeito.
