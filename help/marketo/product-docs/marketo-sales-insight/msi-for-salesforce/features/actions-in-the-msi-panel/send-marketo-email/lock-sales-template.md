---
unique-page-id: 12981050
description: Bloquear modelo de vendas - Documentação do Marketo - Documentação do produto
title: Bloquear Modelo de Vendas
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---

# Bloquear Modelo de Vendas {#lock-sales-template}

Para impedir que usuários do CRM editem modelos de vendas, os administradores podem habilitar a capacidade de bloquear modelos, o que permite que os usuários bloqueiem modelos individualmente no editor de email.

>[!CAUTION]
>
>Este recurso funciona somente para [!DNL Salesforce] e não é compatível com [!DNL Microsoft Dynamics] ou outros CRMs. Os modelos acessados dos plug-ins do [!DNL Outlook] ou do Gmail não serão bloqueados, pois o editor não é controlado pela Marketo.

## Ativar o modelo de bloqueio {#enable-lock-template}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para **[!UICONTROL Admin]** e clique em **[!UICONTROL Sales Insight]**.

   ![](assets/1.png)

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Editar]**.

   ![](assets/2.png)

1. Verificar **[!UICONTROL Habilitar a capacidade de bloquear modelos]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Por padrão, essa caixa está marcada e a capacidade de bloquear modelos está ativada. Desmarcá-la desativará o recurso de modelo de bloqueio no editor de email.

>[!NOTE]
>
>Alterar essa configuração como administrador **não** afetará retroativamente os modelos existentes; ou seja, não os bloqueará automaticamente.

## Bloquear modelo no Editor de email {#lock-template-in-the-email-editor}

1. Selecione o email que deseja bloquear e clique em **[!UICONTROL Editar Rascunho]**.

   ![](assets/5.png)

1. No editor de email, clique em **[!UICONTROL Configurações de email]**.

   ![](assets/6.png)

1. Marque **[!UICONTROL Publicar no Marketo Sales Insight]** se ainda não estiver marcado. Agora você pode desmarcar **[!UICONTROL Permitir que o usuário do CRM edite o email]** para bloquear o modelo. Clique em **[!UICONTROL Salvar]**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Por padrão, essa caixa está marcada e os usuários do CRM têm permissão para editar emails.
