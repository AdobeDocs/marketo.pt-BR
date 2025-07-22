---
description: Conceder consentimento para registro da ID do cliente e do aplicativo - Documentação do Marketo - Documentação do produto
title: Conceder consentimento para a ID do cliente e o registro do aplicativo
exl-id: d0c851d7-24a1-4b17-9daa-f0ceed39d040
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Conceder consentimento para a ID do cliente e o registro do aplicativo {#grant-consent-for-client-id-and-app-registration}

Siga as etapas abaixo para saber como conceder o consentimento/as permissões necessárias.

## Conceder permissões de usuário delegado para o usuário de sincronização {#grant-delegated-user-permissions-for-the-sync-user}

1. Use um programa de texto limpo (Bloco de Notas para Windows, Edição de Texto para Mac) para criar um URI (Uniform Resource Identifier) de autorização, colando o texto abaixo e substituindo os valores `client_id`, `redirect_uri` e `state`.

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
      <td><strong>valor redirect_uri</strong></td> 
      <td>deve ser o mesmo que o valor inserido no momento do registro do aplicativo &gt; Redirecionar URIs</td> 
     </tr> 
     <tr> 
      <td><strong>valor do estado</strong></td> 
      <td>pode ser qualquer ID (por exemplo, 12345)</td> 
     </tr> 
    </tbody> 
   </table>

   A URL final deve ser mais ou menos assim: `https://login.microsoftonline.com/common/oauth2/authorize?client_id=xxxxxx-xxxx-xxxx-xxxx-xxxxxxxx&response_type=code&redirect_uri=https://www.marketo.com&response_mode=query&state=12345`

1. Abra o URI que você criou em qualquer navegador.

   ![](assets/grant-consent-for-client-id-app-registration-1.png)

1. Faça logon como o Usuário de sincronização para o qual você está concedendo permissões.

   ![](assets/grant-consent-for-client-id-app-registration-2.png)

   >[!NOTE]
   >
   >Se você já estiver conectado ao Azure como um Administrador em outra guia, precisará usar um navegador diferente ou modo Incógnito para fazer logon como o Usuário da sincronização.

1. Clique em **[!UICONTROL Aceitar]**.

   ![](assets/grant-consent-for-client-id-app-registration-3.png)

## Conceder consentimento a todos os usuários {#grant-consent-for-all-users}

Como administrador, você também pode consentir com as permissões delegadas de um aplicativo em nome de todos os usuários em seu locatário. O consentimento administrativo impede que a caixa de diálogo de consentimento apareça para cada usuário no locatário e pode ser feito no portal do Azure por usuários com a função de administrador. Saiba quais funções de administrador podem [consentir com permissões delegadas aqui](https://docs.microsoft.com/en-us/azure/active-directory/roles/permissions-reference).

1. No portal do Azure, navegue até a página inicial do aplicativo.

1. Em [!UICONTROL Gerenciar], clique em **[!UICONTROL Permissões de API]**.

   ![](assets/grant-consent-for-client-id-app-registration-4.png)

1. Clique no botão **[!UICONTROL Dar consentimento administrativo]** (para locatário).

   ![](assets/grant-consent-for-client-id-app-registration-5.png)

1. Clique em **[!UICONTROL Sim]** para confirmar.

   ![](assets/grant-consent-for-client-id-app-registration-6.png)
