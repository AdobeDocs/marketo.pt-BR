---
unique-page-id: 1147031
description: Excluir pessoa do SFDC - Documentação do Marketo - Documentação do produto
title: Excluir pessoa do SFDC
exl-id: 8245de35-f374-4241-946e-b4c4b87cc85e
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 6%

---

# Excluir pessoa do SFDC {#delete-person-from-sfdc}

Se precisar remover um conjunto específico de clientes potenciais do Salesforce, mas deixá-los como pessoas no Marketo Engage, você pode usar a ação de fluxo Excluir pessoa do SFDC.

>[!NOTE]
>
>Disponível somente quando integrado com [!DNL Salesforce].

1. No Banco de dados, clique na pessoa que você deseja remover do Salesforce. Em seguida, clique em **[!UICONTROL Ações da pessoa]** e selecione **[!DNL Salesforce]**.

   ![](assets/delete-person-from-sfdc-1.png)

1. Selecione **[!UICONTROL Excluir pessoa do SFDC]**.

   ![](assets/delete-person-from-sfdc-2.png)

1. Verifique se a configuração **[!UICONTROL Excluir no Marketo]** é **[!UICONTROL false]** e clique em **[!UICONTROL Executar Agora]**.

   ![](assets/delete-person-from-sfdc-3.png)

   Depois que a etapa de fluxo for executada, sua pessoa não será mais um cliente em potencial no [!DNL Salesforce], mas permanecerá no Marketo.

   >[!CAUTION]
   >
   >Se você definir **[!UICONTROL Excluir no Marketo]** como **[!UICONTROL true]** e excluir as pessoas do Marketo e os clientes em potencial do Salesforce, eles serão permanentemente excluídos. Essa ação não pode ser desfeita.
