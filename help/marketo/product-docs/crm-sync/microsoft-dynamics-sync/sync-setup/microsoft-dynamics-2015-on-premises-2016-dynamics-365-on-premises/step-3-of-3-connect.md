---
unique-page-id: 7504744
description: Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 de 3 - Marketing to Docs - Documentação do produto
title: Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Etapa 3 de 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Instale o Marketo para Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 de 3 {#install-marketo-for-dynamics-on-prem-and-on-prem-step-of}

>[!PREREQUISITES]
>
>* [Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Etapa 1 de 3](step-1-of-3-install.md)
>* [Instale o Marketo para o Dynamics 2015 On-Prem e 2016 365 On-Prem Etapa 2 de 3](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Permissões de administrador necessárias**

## Digite as informações do usuário do Dynamics Sync {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Selecione **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Clique em **Editar** em **Etapa 1: Insira Credenciais**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no schema após o envio. Se as credenciais incorretas forem salvas, será necessário obter uma nova subscrição de marketing.

1. Digite o **Nome de usuário**, **Senha** um Microsoft Dynamics **URL** e um **ID de cliente opcional**. Clique em **Salvar** quando terminar.

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#8cf9ffe9fecce8e3e1ede5e2a2efe3e1) ou DOMÍNIO\usuário.

   >[!TIP]
   >
   >Não sabe o URL? Mostraremos como localizar seu [URL do Serviço de Organização Dinâmica](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) aqui.

## Selecionar campos para sincronizar {#select-fields-to-sync}

1. Clique em **Editar** em **Etapa 2: Selecione Campos para sincronização**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Selecione os campos que deseja sincronizar com o Marketo, de modo que eles sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, certifique-se de entrar e selecionar os novos campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Habilitar Sincronização**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >O Marketo não eliminará a duplicação automaticamente em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas manualmente.

1. Leia tudo no pop-up, digite seu email e clique em **Sincronização de Start**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A primeira sincronização pode levar algumas horas. Depois de terminar, você receberá uma notificação por email.

   ![](assets/image2015-3-16-9-59-51.png)

Excelente trabalho!
