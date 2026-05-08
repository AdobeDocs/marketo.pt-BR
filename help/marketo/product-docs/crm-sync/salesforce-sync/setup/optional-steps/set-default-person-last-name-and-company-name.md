---
unique-page-id: 4719291
description: Saiba como definir o sobrenome da pessoa padrão e o nome da empresa para a sincronização do Salesforce. Use as Opções de Administração e Sincronização para que os registros parciais sejam sincronizados com os valores padrão.
title: Definir sobrenome da pessoa e nome da empresa padrão
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 10%

---

# Definir sobrenome da pessoa e nome da empresa padrão {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] requer (mínimo) sobrenome e nome da empresa para seus clientes em potencial e contatos. Registros incompletos não serão sincronizados com [!DNL Salesforce]. Se quiser sincronizar registros parciais, defina valores padrão para o Marketo a serem usados com [!DNL Salesforce].

1. Vá para **[!UICONTROL Admin]** e clique em **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Clique em **[!UICONTROL Editar opções de sincronização]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Insira um **[!UICONTROL Sobrenome da pessoa padrão]** e uma **[!UICONTROL Empresa da pessoa padrão]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >O Marketo Engage só atribui um valor padrão quando o registro é sincronizado inicialmente com o Salesforce e somente se qualquer um dos campos obrigatórios estiver vazio.

Toda vez que uma pessoa não tiver um sobrenome ou nome da empresa, o Marketo adicionará o valor padrão à medida que sincroniza o registro.
