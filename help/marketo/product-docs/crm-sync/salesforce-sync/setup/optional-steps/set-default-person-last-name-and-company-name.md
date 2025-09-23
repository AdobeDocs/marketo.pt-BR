---
unique-page-id: 4719291
description: Definir sobrenome da pessoa padrão e nome da empresa - Documentação do Marketo - Documentação do produto
title: Definir sobrenome da pessoa e nome da empresa padrão
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 11%

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

E é isso! Toda vez que uma pessoa não tiver um sobrenome e/ou nome da empresa, o Marketo adicionará o valor padrão à medida que sincroniza o registro.
