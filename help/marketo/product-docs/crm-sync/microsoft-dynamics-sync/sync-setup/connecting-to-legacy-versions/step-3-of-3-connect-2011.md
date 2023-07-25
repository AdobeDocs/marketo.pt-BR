---
unique-page-id: 3571809
description: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (2011 no local) - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (2011 no local)
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# Etapa 3 de 3: Conectar o Microsoft Dynamics com o Marketo (2011 no local) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Tudo bem! Instalamos a solução e configuramos o usuário de sincronização. Em seguida, precisamos conectar o Marketo e o Dynamics.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: instalar a solução da Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [Etapa 2 de 3: Configurar o usuário do Marketo Sync no Dynamics (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Inserir Informações de Usuário da Sincronização Dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Clique em **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **Editar** in **Etapa 1: Inserir credenciais.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no esquema após o envio. Se credenciais incorretas forem salvas, será necessário obter uma nova assinatura do Marketo.

1. Insira o **Nome de usuário**, **Senha** e CRM **URL** e clique em **Salvar**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* O Nome de Usuário no Marketo deve corresponder ao Nome de Usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMAIN\user.
   >* Se você não souber o URL, [saiba como encontrá-lo aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## Selecionar campos para a sincronização {#select-fields-to-sync}

Agora precisamos selecionar os campos que queremos sincronizar.

1. Clique em **Editar** in **Etapa 2: Selecionar campos para sincronização.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Há campos pré-selecionados que serão sincronizados. Adicione mais se desejar e clique em **Salvar**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

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

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** in **Etapa 3: Habilitar Sincronização**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >A Marketo não eliminará automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou leads manualmente.

1. Leia tudo na janela pop-up, insira seu email e clique em **Iniciar sincronização**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de concluído, você receberá uma notificação por email.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Excelente trabalho!
