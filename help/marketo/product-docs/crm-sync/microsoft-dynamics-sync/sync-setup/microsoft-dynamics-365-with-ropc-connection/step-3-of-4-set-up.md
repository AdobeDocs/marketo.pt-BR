---
description: Etapa 3 de 4 - Configurar o aplicativo cliente no MS Dynamics - Documentos do Marketo - Documentação do produto
title: Etapa 3 de 4 - Configurar o aplicativo cliente no MS Dynamics
source-git-commit: 9ee27e22fec4e0ab85c193be2ea99d3c8b40568b
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Etapa 3 de 4: Configurar o aplicativo cliente no MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Etapa 1 de 4: Instale a solução Marketo com a conexão de controle de senha do proprietário de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Etapa 2 de 4: Configurar a solução Marketo com a conexão de controle de senha do proprietário de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. Navegue até https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration.

1. Siga todas as etapas. Para a Etapa 3, insira um nome de aplicativo relevante (por exemplo, &quot;Integração do Marketo&quot;). Em Tipos de conta suportados, selecione Conta somente neste diretório organizacional.

1. Anote a ID do aplicativo (ClientId). Você precisará inseri-lo no Marketo posteriormente.

1. Conceda consentimento ao administrador seguindo as etapas em [este artigo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md).

1. Gere um segredo do cliente no Admin Center clicando em **Certificados e segredos**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Clique em **Novo segredo de cliente**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Adicione uma descrição de Segredo do cliente e clique em **Adicionar**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Certifique-se de anotar o valor Segredo do cliente (visto na captura de tela abaixo), pois ele será necessário posteriormente. Ela só é exibida uma vez e você não poderá recuperá-la novamente.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federated com AD FS no local {#azure-ad-federated-with-ad-fs-on-prem}

O Federated Azure AD para o ADFS Onlocal precisa da criação de uma política de Descoberta de Domínio para o aplicativo específico. Com esta política, o Azure AD redirecionará a solicitação de autenticação para o serviço de federação. Para isso, a sincronização de hash de senha deve ser ativada no AD Connect. Para obter mais informações, consulte [OAuth com ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) e [Definir uma política de hardware para um aplicativo](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application).

Referências adicionais [pode ser encontrada aqui](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=Este%20report%20also%20inclui%20federado, são%20federado%20a%20Azure%20AD.).

>[!MORELIKETHIS]
>
>* [Etapa 4 de 4: Conecte a solução Marketo com a conexão de controle de senha do proprietário de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md)

