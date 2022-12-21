---
unique-page-id: 12981050
description: Bloquear modelo de vendas - Documentos do Marketo - Documentação do produto
title: Bloquear Modelo de Vendas
exl-id: 005dde5d-ed60-444b-b7a3-b91be72a0151
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Bloquear Modelo de Vendas {#lock-sales-template}

Para impedir que usuários do CRM editem modelos de vendas, os administradores podem ativar a capacidade de bloquear modelos, o que permite que os usuários bloqueiem modelos individualmente do editor de email.

>[!CAUTION]
>
>Esse recurso funciona somente para o Salesforce e não é compatível com o Microsoft Dynamics ou outros CRMs. Os modelos acessados nos plug-ins do Outlook ou do Gmail não serão bloqueados, pois o editor não é controlado pela Marketo.

## Habilitar modelo de bloqueio {#enable-lock-template}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Ir para **Administrador**, depois clique em **Insight de vendas**.

   ![](assets/1.png)

1. Em **Configurações**, clique em **Editar**.

   ![](assets/2.png)

1. Verificar **Habilitar a capacidade de bloquear modelos**. Clique em **Salvar**.

   ![](assets/image2017-10-9-8-3a19-3a45.png)

>[!NOTE]
>
>Por padrão, esta caixa está marcada e a capacidade de bloquear modelos está ativada. Ao desmarcá-lo, o recurso de modelo de bloqueio será desativado no editor de email.

>[!NOTE]
>
>A alteração dessa configuração como administrador irá **not** afetam retroativamente modelos existentes; ou seja, não os bloqueia automaticamente.

## Bloquear modelo no editor de email {#lock-template-in-the-email-editor}

1. Selecione o email que deseja bloquear e clique em **Editar rascunho**.

   ![](assets/5.png)

1. No editor de email, clique em **Configurações de email**.

   ![](assets/6.png)

1. Verificar **Publicar no Marketo Sales Insight** se ainda não estiver marcado. Agora você pode desmarcar **Permitir que o usuário do CRM edite o email** para bloquear o template. Clique em **Salvar**.

   ![](assets/7.png)

   >[!NOTE]
   >
   >Por padrão, essa caixa está marcada e os usuários do CRM têm permissão para editar emails.
