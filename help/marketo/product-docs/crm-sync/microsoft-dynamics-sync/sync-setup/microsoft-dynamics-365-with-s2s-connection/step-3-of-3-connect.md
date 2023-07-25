---
unique-page-id: 3571830
description: Etapa 3 de 3 - Conectar a solução da Marketo com conexão de servidor a servidor - Documentação da Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar a solução da Marketo com conexão de servidor a servidor
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# Etapa 3 de 3: Conectar a solução da Marketo com conexão de servidor a servidor {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

Esta é a última etapa da sincronização. Estamos quase lá!

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instalar a solução da Marketo com conexão de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [Etapa 2 de 3: Configurar a solução da Marketo com conexão de servidor a servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!IMPORTANT]
>
>Se estiver atualizando da Autenticação básica para o OAuth, você precisará entrar em contato com [Suporte ao Marketo](https://nation.marketo.com/t5/support/ct-p/Support) para obter ajuda com a atualização dos parâmetros adicionais. Habilitar este recurso interromperá temporariamente a sincronização até que novas credenciais sejam inseridas e a sincronização seja reabilitada. O recurso pode ser desativado (até abril de 2022) se você quiser reverter para o modo de autenticação antigo.

>[!NOTE]
>
>Antes de inserir novas credenciais, você pode [valide-os aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

## Inserir informações do Usuário da Sincronização Dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selecionar **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Clique em **Editar** in **Etapa 1: Inserir Credenciais**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Verifique se o URL da organização está correto, pois não é possível reverter as alterações subsequentes no esquema após o envio. Se um URL de organização incorreto for usado, será necessário obter uma nova assinatura do Marketo. Se você não souber o URL, [saiba como encontrá-lo aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. Insira as informações do usuário da sincronização dinâmica e clique em **Salvar** quando terminar.

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >O nome de usuário no Marketo deve corresponder ao [endereço de email](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) do usuário do aplicativo no CRM. O formato pode ser `user@domain.com` ou DOMAIN\user.

## Selecionar campos para a sincronização {#select-fields-to-sync}

1. Clique em **Editar** in **Etapa 2: Selecionar campos para sincronização**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazer isso com o [sincronização desabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando o [Selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, selecione os novos campos que serão sincronizados com o Marketo.

1. Acesse Administrador e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes da sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e marque-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer item. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** in **Etapa 3: Habilitar Sincronização**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >A Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou leads manualmente.

1. Leia tudo na janela pop-up, digite seu endereço de email e clique em **Iniciar sincronização**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. A primeira sincronização pode levar algumas horas. Depois de concluído, você receberá uma notificação por email.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Excelente trabalho!
