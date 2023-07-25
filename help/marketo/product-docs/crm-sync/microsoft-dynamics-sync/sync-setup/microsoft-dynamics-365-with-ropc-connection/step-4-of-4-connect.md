---
description: Etapa 4 de 4 - Conectar a solução da Marketo com a conexão de controle de senha de proprietário de recurso - Documentação da Marketo - Documentação do produto
title: Etapa 4 de 4 - Conectar a solução da Marketo com a conexão de controle de senha de proprietário de recurso
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 2%

---

# Etapa 4 de 4: Conectar a solução Marketo com a conexão de controle de senha de proprietário de recurso {#step-4-of-4-connect-the-marketo-solution-ropc}

Esta é a última etapa da sincronização. Você está quase lá!

>[!PREREQUISITES]
>
>* [Etapa 1 de 4: instalar a solução Marketo com a conexão de controle de senha de proprietário de recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Etapa 2 de 4: Configurar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Etapa 3 de 4: Configurar o Aplicativo Cliente no MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Se estiver atualizando da Autenticação básica para o OAuth, você pode usar [este artigo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) para reconfigurar sua autenticação.

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

   >[!NOTE]
   >
   >Antes de inserir novas credenciais, você pode [valide-os aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

1. Insira o **Nome de usuário**, **Senha**, Microsoft Dynamics **URL**, **ID do cliente**, e **Segredo do cliente**. Clique em **Salvar** quando terminar.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >O Nome de Usuário no Marketo deve corresponder ao Nome de Usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMAIN\user.

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

>[!MORELIKETHIS]
>
>[Reconfigurar Método de Autenticação do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)