---
description: Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 3 de 3 - Documentos do Marketo - Documentação do produto
title: Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 3 de 3
exl-id: ae801a59-8e29-479c-84c5-a18c7511f21f
source-git-commit: 44cc13361f6ff58d1be388fa0425a6daa63e4c7d
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 1%

---

# Etapa 3 de 3: Conecte O Marketo Dynamics (2016 No Local/Dynamics 365 No Local) {#step-of-connect-marketo-dynamics-on-premises-2016}

>[!PREREQUISITES]
>
>* [Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 1 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)
>* [Instale o Marketo para Microsoft Dynamics 2016/Dynamics 365 no local Etapa 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Inserir informações do usuário de sincronização dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Administrador**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Selecionar **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Clique em **Editar** em **Etapa 1: Inserir Credenciais**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Certifique-se de que suas credenciais estejam corretas, pois não podemos reverter as alterações subsequentes do schema após o envio. Se as credenciais incorretas forem salvas, você terá que obter uma nova assinatura do Marketo.

1. Insira o **Nome do usuário**, **Senha** a Microsoft Dynamics **URL** e um **Id/Segredo Do Cliente**. Clique em **Salvar** quando concluído.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Se sua Marketo foi provisionada antes de outubro de 2020, a ID do cliente e o Segredo são campos opcionais. Caso contrário, são obrigatórias. A obtenção dessas informações dependerá da versão do MSD que você estiver usando.
   >* O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.
   >* Se você não souber o URL, [saiba como encontrá-lo aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


   >[!TIP]
   >
   >Não sabe o URL? Mostraremos como encontrar seu [URL de Serviço de Organização Dinâmica](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aqui.

## Selecionar campos para a sincronização {#select-fields-to-sync}

1. Clique em **Editar** em **Etapa 2: Selecionar Campos para Sincronizar**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazer isso com a variável [sincronização desativada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando o [Selecionar Campos para Sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, acesse e selecione os novos campos a serem sincronizados com o Marketo.

1. Acesse Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Ativar Sincronização**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >O Marketo não deduplicará automaticamente em relação a uma sincronização do Microsoft Dynamics ou quando você insere pessoas manualmente.

1. Leia tudo no pop-up, insira seu email e clique em **Iniciar Sincronização**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de terminar, você receberá uma notificação por email.

   ![](assets/image2015-3-16-9-59-51.png)

Excelente trabalho!
