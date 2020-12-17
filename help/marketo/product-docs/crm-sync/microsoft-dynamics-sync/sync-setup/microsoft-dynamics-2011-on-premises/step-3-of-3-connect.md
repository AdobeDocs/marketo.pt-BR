---
unique-page-id: 3571809
description: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (2011 On-Premise) - Documentação do produto
title: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketo (On-Premise 2011)
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Etapa 3 de 3: Conecte o Microsoft Dynamics com o Marketing (On-Premise 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Tudo bem! Instalamos a solução e configuramos o usuário de sincronização. Em seguida, precisamos conectar o Marketing e o Dynamics.

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instale a solução Marketo (2011 On-Premise)](step-1-of-3-install.md)
>* [Etapa 2 de 3: Configurar usuário de sincronização de marketing no Dynamics (2011 no local)](step-2-of-3-set-up.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Digite as informações do usuário do Dynamics Sync {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Clique em **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Clique em **Editar** em **Etapa 1: Introduza as credenciais.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no schema após o envio. Se as credenciais incorretas forem salvas, será necessário obter uma nova subscrição de marketing.

1. Digite **Nome de usuário**, **Senha** e CRM **URL** e clique em **Salvar**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) ou DOMÍNIO\usuário.

   >[!TIP]
   >
   >Não sabe o URL? Mostraremos como localizar o [URL do Serviço de Organização Dinâmica](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aqui.

## Selecionar campos para sincronizar {#select-fields-to-sync}

Agora precisamos selecionar os campos nos quais queremos sincronizar.

1. Clique em **Editar** em **Etapa 2: Selecionar campos para sincronização.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Há campos pré-selecionados que serão sincronizados. Adicione mais se desejar e clique em **Salvar**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, certifique-se de entrar e selecionar os novos campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Habilitar Sincronização**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >O Marketo não eliminará a duplicação automaticamente em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou clientes em potencial manualmente.

1. Leia tudo no pop-up, digite seu email e clique em **Sincronização de Start**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de terminar, você receberá uma notificação por email.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Excelente trabalho!
