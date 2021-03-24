---
unique-page-id: 3571809
description: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (2011 no local) - Documentos do Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (2011 no local)
translation-type: tm+mt
source-git-commit: 20eb3389b267101fb277152f150c2119a5be65a8
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Etapa 3 de 3: Conecte o Microsoft Dynamics com o Marketo (2011 no local) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Tudo bem! Instalamos a solução e configuramos o usuário de sincronização. Em seguida, precisamos conectar o Marketo e o Dynamics.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instalar a solução Marketo (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)
>* [Etapa 2 de 3: Configurar usuário de sincronização do Marketo no Dynamics (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Inserir Informações do Usuário de Sincronização Dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Clique em **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **Editar** em **Etapa 1: Insira as credenciais.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Certifique-se de que suas credenciais estejam corretas, pois não podemos reverter as alterações subsequentes do schema após o envio. Se as credenciais incorretas forem salvas, você terá que obter uma nova assinatura do Marketo.

1. Insira o **Nome de usuário**, **Senha** e CRM **URL** e clique em **Salvar**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.
   >* Se você não souber o URL, [saiba como encontrá-lo aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Selecionar Campos para Sincronizar {#select-fields-to-sync}

Agora, precisamos selecionar os campos que deseja sincronizar.

1. Clique em **Editar** em **Etapa 2: Selecionar Campos para Sincronizar.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Há campos pré-selecionados que serão sincronizados. Adicione mais se desejar e clique em **Salvar**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazer isso com o [sync disabled](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando o [Selecionar Campos para Sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, acesse e selecione os novos campos a serem sincronizados com o Marketo.

1. Acesse Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Habilitar Sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Habilite Sync**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >O Marketo não desduplica automaticamente em relação a uma sincronização do Microsoft Dynamics ou quando você insere manualmente pessoas ou leads.

1. Leia tudo na janela pop-up , insira seu email e clique em **Iniciar Sincronização**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de terminar, você receberá uma notificação por email.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Excelente trabalho!
