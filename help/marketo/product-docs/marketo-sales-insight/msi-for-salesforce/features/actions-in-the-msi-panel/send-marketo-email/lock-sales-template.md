---
unique-page-id: 12981050
description: Bloquear modelo de vendas - Documentos do marketing - Documentação do produto
title: Bloquear modelo de vendas
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Bloquear Modelo de Vendas {#lock-sales-template}

Para impedir que usuários do CRM editem modelos de vendas, os administradores podem habilitar a capacidade de bloquear modelos, o que permite que os usuários bloqueiem modelos individualmente do editor de email.

>[!CAUTION]
>
>Este recurso funciona somente para o Salesforce e não é compatível com o Microsoft Dynamics ou outros CRMs. Os modelos acessados pelo Outlook ou pelos plug-ins do Gmail não serão bloqueados, pois o editor não é controlado pelo Marketo.

## Ativar Bloquear Modelo {#enable-lock-template}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para **Admin** e clique em **Sales Insight**.

   ![](assets/1.png)

1. Em **Configurações**, clique em **Editar**.

   ![](assets/2.png)

1. Marque **Habilite a capacidade de bloquear modelos**. Clique em **Salvar**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Por padrão, essa caixa está marcada e a capacidade de bloquear modelos está ativada. Desmarcá-lo desativará o recurso de modelo de bloqueio no editor de email.

>[!NOTE]
>
>Alterar essa configuração como um administrador **não** afetará retroativamente os modelos existentes; ou seja, não os bloqueia automaticamente.

## Bloquear modelo no editor de email {#lock-template-in-the-email-editor}

1. Selecione o email que deseja bloquear e clique em **Editar rascunho**.

   ![](assets/5.png)

1. No editor de email, clique em **Configurações de email**.

   ![](assets/6.png)

1. Marque **Publicar no Marketing Insight de Vendas** se ainda não estiver marcado. Agora você pode desmarcar **Permitir que o usuário do CRM edite email** para bloquear o modelo. Clique em **Salvar**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Por padrão, essa caixa está marcada e os usuários do CRM podem editar emails.

