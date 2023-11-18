---
description: Etapa 3 de 4 - Configurar o aplicativo do cliente no MS Dynamics - Documentação do Marketo - Documentação do produto
title: Etapa 3 de 4 - Configurar o Aplicativo do Cliente no MS Dynamics
exl-id: e7897174-3303-4c3b-8832-3e10f34fca96
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Etapa 3 de 4: Configurar o Aplicativo Cliente no MS Dynamics {#step-3-of-4-set-up-client-app-ms-dynamics-ropc}

>[!PREREQUISITES]
>
>* [Etapa 1 de 4: instalar a solução Marketo com a conexão de controle de senha de proprietário de recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}
>* [Etapa 2 de 4: Configurar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}

1. Navegue até este [Artigo do Microsoft](https://docs.microsoft.com/en-us/powerapps/developer/common-data-service/walkthrough-register-app-azure-active-directory#create-an-application-registration){target="_blank"}.

1. Siga todas as etapas. Para a Etapa 3, insira um nome de aplicativo relevante (por exemplo, &quot;Integração do Marketo&quot;). Em Tipos de conta compatíveis, selecione Conta somente neste diretório organizacional.

1. Anote a ID do aplicativo (ClientId). Você precisará inseri-lo no Marketo mais tarde.

1. Conceda consentimento do administrador seguindo as etapas em [este artigo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md){target="_blank"}.

1. Gere um Segredo do cliente no Admin Center clicando em **[!UICONTROL Certificados e segredos]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-1.png)

1. Clique em **[!UICONTROL Novo segredo do cliente]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-2.png)

1. Adicione uma descrição Segredo do cliente e clique em **[!UICONTROL Adicionar]**.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-3.png)

   >[!CAUTION]
   >
   >Anote o valor do Segredo do cliente (visto na captura de tela abaixo), como você precisará dele posteriormente. É exibido apenas uma vez e não será possível recuperá-lo novamente.

   ![](assets/step-3-of-4-set-up-client-app-ms-dynamics-ropc-4.png)

## Azure AD Federado com AD FS no local {#azure-ad-federated-with-ad-fs-on-prem}

O Federated Azure AD para ADFS no Local precisa da criação de uma política de Descoberta de Domínio Doméstico para o aplicativo específico. Com esta política, o Azure AD redirecionará a solicitação de autenticação para o serviço de federação. A sincronização de hash de senha deve ser habilitada no AD Connect para isso. Para obter mais informações, consulte [OAuth com ROPC](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc){target="_blank"} and [Set an hrd policy for an application](https://docs.microsoft.com/en-us/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#example-set-an-hrd-policy-for-an-application){target="_blank"}.

Referências adicionais [pode ser encontrado aqui](https://docs.microsoft.com/en-us/azure/active-directory/reports-monitoring/concept-all-sign-ins#:~:text=Interactive%20user%20sign%2Dins%20are,as%20the%20Microsoft%20Authenticator%20app.&amp;text=This%20report%20also%20includes%20federated, are%20federated%20to%20Azure%20AD.){target="_blank"}.

## Antes de prosseguir para a Etapa 4 {#before-proceeding-to-step-4}

* Se quiser restringir o número de registros sincronizados, [configurar um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md){target="_blank"} agora.
* Execute o [Validar a sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"} processo. Ele verifica se as configurações iniciais foram feitas corretamente.
* Faça logon no Usuário do Marketo Sync no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>* [Etapa 4 de 4: Conectar a solução Marketo com a conexão de controle de senha de proprietário de recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md){target="_blank"}
