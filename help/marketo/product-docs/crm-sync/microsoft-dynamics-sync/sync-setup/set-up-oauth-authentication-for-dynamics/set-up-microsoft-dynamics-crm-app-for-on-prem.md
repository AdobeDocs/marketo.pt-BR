---
description: Configurar o aplicativo Microsoft Dynamics CRM para On-loco - Documentos do Marketo - Documentação do produto
title: Configurar o aplicativo do Microsoft Dynamics CRM no local
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Configurar o aplicativo Microsoft Dynamics CRM para no local {#set-up-microsoft-dynamics-crm-app-for-on-prem}

A configuração baseada na ID do cliente/Segredo do cliente no Marketo pode ser feita no local com o AD FS (ver. 2016 ou posterior). Para versões mais antigas do No local, entre em contato com [Suporte do Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obter a alteração do método de autenticação, que será baseado apenas na ID de usuário e na Senha.

## Configurar o aplicativo Microsoft Dynamics CRM {#set-up-microsoft-dynamics-crm-app}

Siga as etapas em [este artigo da Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later).

Quando terminar, a próxima etapa é **Inserir a ID do cliente gerada pelo Dynamics CRM e o segredo no Marketo**.

## Insira a ID do cliente gerada pelo Dynamics CRM e o segredo no Marketo {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

As etapas a seguir são aplicáveis às versões online e no local.

1. No Marketo, clique em **Admin**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. Clique em **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. Clique em **Desativar Sincronização**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. Ao lado de credenciais, clique em **Editar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. Insira o **Client Id** e o **Client Secret** que você recuperou anteriormente e pressione **Save**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. Clique em **Validar Configuração de Sincronização**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. Clique em **Next**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. Você deve ver todas as marcas de seleção verdes. Clique em **Fechar**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >Se você vir um X vermelho entre suas marcas de seleção verdes, consulte [este artigo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para obter as opções de correção.

1. Clique em **Ativar Sincronização**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

E é isso!
