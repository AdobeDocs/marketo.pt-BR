---
unique-page-id: 3571819
description: Etapa 3 de 3 - Connect Marketing and Dynamics (2013 On-Premise) - Marketing to Docs - Documentação do produto
title: Etapa 3 de 3 - Conectar marcas e dinâmicas (locais 2013)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Etapa 3 de 3: Connect Marketing and Dynamics (On-Premise 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

Tudo bem! Instalamos a solução e configuramos o usuário de sincronização. Em seguida, precisamos conectar o Marketing e o Dynamics.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instalar a solução Marketo no Dynamics (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-1-of-3-install.md)
>* [Etapa 2 de 3: Configurar usuário de sincronização para o Marketing (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Digite as informações do usuário do Dynamics Sync {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Selecione **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **Editar** em **Etapa 1: Insira Credenciais**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no schema após o envio. Se as credenciais incorretas forem salvas, será necessário obter uma nova subscrição de marketing.

1. Digite **Nome de usuário**, **Senha** e Microsoft Dynamics **URL** e clique em **Salvar**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser user@domain.com ou DOMAIN\user.

   >[!TIP]
   >
   >Não sabe o URL? Mostraremos como localizar o [URL do Serviço de Organização Dinâmica](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aqui.

## Selecionar campos para sincronizar {#select-fields-to-sync}

Agora precisamos selecionar os campos nos quais queremos sincronizar.

1. Clique em **Editar** em **Etapa 2: Selecione Campos para sincronização**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo, de modo que eles sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, certifique-se de entrar e selecionar os novos campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Habilitar Sincronização**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >O Marketo não eliminará a duplicação automaticamente em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou clientes em potencial manualmente.

1. Leia tudo no pop-up, digite seu email e clique em **Sincronização de Start**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de terminar, você receberá uma notificação por email.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Excelente trabalho! Você acabou de desencadear o poder da sincronização bidirecional entre o Marketo e o Microsoft Dynamics. Se você adquiriu o Marketing Cloud Sales Insight, é mais divertido:

>[!MORELIKETHIS]
>
>[Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)
