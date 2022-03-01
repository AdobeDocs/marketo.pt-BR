---
unique-page-id: 10095429
description: Corrigir problemas de sincronização de validação do Dynamics - Documentos do Marketo - Documentação do produto
title: Corrigir problemas de sincronização de validação do Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
source-git-commit: 48b8289994e000eafd72982ac1b4a0a809b10bab
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 6%

---

# Corrigir problemas de sincronização de validação do Dynamics {#fix-dynamics-validation-sync-issues}

## Validar os resultados da ferramenta de sincronização {#validate-sync-tool-results}

When you run the Dynamics Validate Sync, it generates a report. Se houver um ![x](assets/delete.png) ao lado de uma etapa, consulte as opções abaixo para identificar e corrigir o problema. Then, rerun the sync validation steps until the result shows nothing but green checkmarks.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL válido {#url-is-valid}

If you have an ![x](assets/delete.png) here, verify that the URL is valid. Localize-o aqui em Recursos do desenvolvedor e veja o Serviço de organização. O URL pode ser inválido por vários motivos.

1. Faça logon no Dynamics. Click the Settings icon and select **Advanced Settings**.

   ![](assets/one.png)

1. Clique em Configurações e selecione **Personalizações**.

   ![](assets/two.png)

1. Clique em **Recursos do desenvolvedor**.

   ![](assets/three.png)

1. O URL do Serviço de Organização pode ser encontrado em Endpoints de Serviço.

   ![](assets/four.png)

## Nome de usuário e senha válidos {#username-and-password-are-valid}

Se você tiver uma ![x](assets/delete.png) aqui, verifique se suas credenciais do Microsoft Dynamics são válidas. Para autenticação S2S da API da Web, o nome de usuário no Marketo deve corresponder ao nome da API da Web [endereço de email](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) do Usuário do aplicativo no CRM. Para outros tipos, deve corresponder ao nome de usuário para o Usuário de sincronização.

## O usuário de sincronização é atribuído à função Usuário de sincronização do Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se você tiver uma ![x](assets/delete.png) aqui, pode ser um dos três problemas abaixo.

**Opção 1 - Verifique se a função de usuário de sincronização Marketo está marcada no Microsoft Dynamics**:

1. No Dynamics, clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Click **Settings** and select **Security**.

   ![](assets/six.png)

1. Clique em **Usuários.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Clique no link para o usuário de sincronização.

   ![](assets/seven.png)

1. Clique em **Gerenciar funções**.

   ![](assets/eight.png)

1. Verifique se a função Usuário de sincronização do Marketo está marcada. Caso contrário, marque-a e clique em **Ok.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Opção 2 - Confirmar o consentimento da concessão**:

1. Revise o [Conceder consentimento para ID do cliente e registro de aplicativo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) para confirmar que o aplicativo tem consentimento administrativo para chamar APIs.

**Opção 3 - Sincronizar usuário**:

1. Verifique se o usuário de sincronização foi adicionado à Configuração do Marketo.

## A solução Marketo foi devidamente instalada {#marketo-solution-is-properly-installed}

If you have an ![x](assets/delete.png) here, Go to Microsoft Dynamics to verify the Marketo installation is there. Consulte a Etapa 1 da documentação de configuração do Microsoft Dynamics.

1. No Dynamics, clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Soluções.**

   ![](assets/eleven.png)

1. Verifique se a solução está listada.

   ![](assets/twelve.png)

## Todas as etapas da solução estão ativadas {#all-steps-in-the-solution-are-enabled}

If you have an ![x](assets/delete.png) here, verify that none of the default steps have been deactivated. All steps are automatically enabled at installation, but they could be deactivated during a customization.

## Atribui-se o usuário de sincronização à solução Marketo {#sync-user-is-assigned-to-the-marketo-solution}

If you have an ![x](assets/delete.png) here, make sure the Sync user is assigned on the Marketo Default page in Microsoft Dynamics.

1. In Dynamics, click the Settings icon and select **Advanced Settings**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Configuração do Marketo**.

   ![](assets/thirteen.png)

1. Verifique se o usuário de sincronização está atribuído como padrão.

   ![](assets/fourteen.png)

## O usuário de sincronização corresponde ao nome de usuário e à senha {#sync-user-matches-username-and-password}

Se você tiver uma ![x](assets/delete.png) aqui, atribua o usuário de sincronização adequado no campo Usuário do Marketo na etapa de configuração Padrão da configuração do Marketo no Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Validar a sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
