---
description: Conceder consentimento para ID do cliente e registro do aplicativo - Documentos do Marketo - Documentação do produto
title: Conceder consentimento para ID do cliente e registro de aplicativo
translation-type: tm+mt
source-git-commit: 3a6d9987e214aa8606b9f5abdc780a81355b1001
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# Conceder Consentimento para Id de Cliente e Registro de Aplicativo {#grant-consent-for-client-id-and-app-registration}

## Conceder permissões de usuário delegado para o usuário de sincronização {#grant-delegated-user-permissions-for-the-sync-user}

1. Use um programa de texto limpo (Bloco de notas para Windows, Edição de texto para Mac) para criar um URI (Uniform Resource Identifier) para autorização colando o texto abaixo e substituindo os valores client_id, redirect_uri e state .

   ```
   https://login.microsoftonline.com/common/oauth2/authorize?
   client_id='xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx'
   &response_type='code'
   &redirect_uri='https://www.<ourdomain>.com'
   &response_mode='query'
   &state='SOME_UNIQUE_UID'
   client_id value should be the client_id generated in App Registration process
   redirect_uri value should be same as value entered at the time of App registration-> Redirect URIs
   state value can be any ID (e.g.,12345)
   ```

   <table> 
    <colgroup> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>valor client_id</strong></td> 
      <td>deve ser a client_id gerada no processo de registro do aplicativo</td> 
     </tr> 
     <tr> 
      <td><strong>valor de redirect_uri</strong></td> 
      <td>deve ser igual ao valor inserido no momento do registro do aplicativo &gt; URIs de redirecionamento</td> 
     </tr> 
     <tr> 
      <td><strong>valor do estado</strong></td> 
      <td>pode ser qualquer ID (por exemplo, 12345)</td> 
     </tr> 
    </tbody> 
   </table>

   O URL final deve ser semelhante a: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Abra o URI criado em qualquer navegador.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Faça logon como o Usuário de sincronização para o qual você está concedendo permissões.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Se você já estiver conectado ao Azure como administrador em outra guia, precisará usar um navegador ou modo Incógnito diferente para fazer logon como o usuário de sincronização.

1. Clique em **Aceitar**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Conceder consentimento para todos os usuários {#grant-consent-for-all-users}

Como administrador, você também pode consentir com as permissões delegadas de um aplicativo em nome de todos os usuários do seu locatário. O consentimento administrativo impede que a caixa de diálogo de consentimento seja exibida para cada usuário no locatário e pode ser feita no portal do Azure por usuários com a função de administrador. Saiba quais funções de administrador podem [consentir com permissões delegadas aqui](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. No portal do Azure, navegue até a página inicial do aplicativo.

1. Em Gerenciar, clique em **Permissões de API**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Clique no botão **Conceder consentimento do administrador** (para locatário).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Clique em **Sim** para confirmar.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)

>[!MORELIKETHIS]
>
>[Configurar o aplicativo do Microsoft Dynamics CRM no local](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/set-up-oauth-authentication-for-dynamics/set-up-microsoft-dynamics-crm-app-for-on-prem.md)
