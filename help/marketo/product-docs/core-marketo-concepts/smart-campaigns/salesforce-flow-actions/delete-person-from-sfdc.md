---
unique-page-id: 1147031
description: Excluir pessoa do SFDC - Documentação do Marketo - Documentação do produto
title: Excluir pessoa da SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 5%

---

# Excluir pessoa da SFDC {#delete-person-from-sfdc}

Se você precisar remover um conjunto específico de clientes potenciais do Salesforce, mas deixá-los como pessoas no Marketo Engage, poderá usar a ação de fluxo Excluir pessoa do SFDC.

>[!NOTE]
>
>Disponível somente quando integrado ao Salesforce.

1. No Banco de dados, clique na pessoa que deseja remover do Salesforce. Em seguida, clique em **[!UICONTROL Ações da pessoa]** e selecione **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Selecione **[!UICONTROL Excluir pessoa do SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Verifique se a configuração **[!UICONTROL Excluir no Marketo]** é **[!UICONTROL false]** e clique em **[!UICONTROL Executar Agora]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Depois que a etapa de fluxo for executada, sua pessoa não será mais a líder no Salesforce, mas permanecerá no Marketo.

   >[!CAUTION]
   >
   >Se você definir **[!UICONTROL Excluir no Marketo]** como **[!UICONTROL true]** e excluir as pessoas do Marketo e os clientes em potencial do Salesforce, eles serão permanentemente excluídos. Essa ação não pode ser desfeita.
