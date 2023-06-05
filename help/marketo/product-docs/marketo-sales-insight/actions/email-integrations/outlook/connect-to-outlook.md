---
description: Conectar-se ao Outlook - Documentação do Marketo - Documentação do produto
title: Conectar ao Outlook
source-git-commit: 2538bd5973eb3372352c3ddbada6521911f9fc33
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

# Conectar ao Outlook {#connect-to-outlook}

Saiba como conectar sua conta de Ações do Sales Insight ao Outlook.

>[!NOTE]
>
>Cada usuário precisa se conectar ao Outlook a partir de sua conta do Marketo Sales.

## Conectando ao Outlook Online {#connecting-to-outlook-online}

Conectar-se ao Outlook significa que você receberá rastreamento de resposta, acesso ao canal de entrega do Outlook, a capacidade de agendar emails no Outlook e enviar conformidade.

1. No Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/connect-to-outlook-1.png)

1. Em Minha conta, selecione **Configurações de email**.

   ![](assets/connect-to-outlook-2.png)

1. Clique em **Conexão de email** guia.

   ![](assets/connect-to-outlook-3.png)

1. Clique em **Introdução**.

   ![](assets/connect-to-outlook-4.png)

1. Selecionar **Eu uso o Outlook para enviar emails** e clique em **Próxima**.

   ![](assets/connect-to-outlook-5.png)

1. Selecione a versão do Outlook que você está usando e clique em **Próxima**. Neste exemplo, estamos escolhendo Outlook Online.

   ![](assets/connect-to-outlook-6.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>Também conhecido como Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange no local</strong></td> 
      <td>Inclui o Exchange 2013 e 2016</td> 
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >No momento, a Marketo não oferece suporte a contas híbridas do Exchange.

1. Clique em **OK**.

   ![](assets/connect-to-outlook-7.png)

1. Se você não estiver conectado ao Outlook, insira suas informações de logon e clique em **Próxima**. Se estiver, escolha a conta à qual deseja se conectar e clique em **Próxima**. Neste exemplo, já estamos conectados.

   ![](assets/connect-to-outlook-8.png)

1. Clique em **Aceitar**.

   ![](assets/connect-to-outlook-9.png)

   Você pode usar essa conexão para rastrear emails e também como um canal de delivery.

   >[!NOTE]
   >
   >O Outlook Online (Office365) impõe seus próprios limites de envio. [Saiba mais aqui](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md#email-provider-limits).

## Conectando-se ao Exchange no local {#connecting-to-exchange-on-premise}

Conectar-se ao Exchange no local significa que você receberá rastreamento de resposta, acesso ao canal de entrega do Outlook, a capacidade de agendar emails no Outlook e enviar conformidade.

1. No Marketo Sales, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/connect-to-outlook-10.png)

1. Em Minha conta, selecione **Configurações de email**.

   ![](assets/connect-to-outlook-11.png)

1. Clique em **Conexão de email** guia.

   ![](assets/connect-to-outlook-12.png)

1. Clique em **Introdução**.

   ![](assets/connect-to-outlook-13.png)

1. Selecionar **Eu uso o Outlook para enviar emails** e clique em **Próxima**.

   ![](assets/connect-to-outlook-14.png)

1. Selecione a versão do Outlook que você está usando e clique em **Próxima**. Neste exemplo, estamos escolhendo Exchange no local.

   ![](assets/connect-to-outlook-15.png)

   <table> 
    <tbody>
     <tr>
      <td><strong>Outlook Online</strong></td> 
      <td>Também conhecido como Exchange Online</td> 
     </tr>
     <tr>
      <td><strong>Exchange no local</strong></td> 
      <td>Inclui o Exchange 2013 e 2016</td> 
     </tr>
    </tbody>
   </table>

1. Insira suas credenciais e clique em **Conectar**.

   ![](assets/connect-to-outlook-16.png)

   >[!NOTE]
   >
   >Se você desativar a Descoberta Automática no menu suspenso Versão do Exchange, será necessário solicitar ao departamento de TI a URL do Exchange.

   Você pode usar essa conexão para rastrear emails e também como um canal de delivery.

   >[!NOTE]
   >
   >Ao usar o Exchange no local, sua equipe de TI estabelecerá seu limite de envio de email.

## Obtendo Permissão para Conectar-se ao Outlook Online {#getting-permission-to-connect-to-outlook-online}

Talvez seja necessário trabalhar com sua equipe de TI para obter permissão para permitir que o Marketo Sales se conecte à sua conta do Outlook Online (Microsoft 365).

>[!NOTE]
>
>Informe à equipe de TI que gerencia sua conta do Microsoft 365 que o aplicativo que precisa de acesso é o &quot;Marketo Sales Connect&quot;.

Dependendo das preferências da equipe de TI e da configuração atual, é melhor consultar essa equipe sobre como conceder acesso. Abaixo estão alguns artigos que podem ajudar a orientar a conversa.

* Consentimento global: [Aplicativos integrados e Azure AD para administradores do Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/enterprise/integrated-apps-and-azure-ads?view=o365-worldwide){target="_blank"}
* Consentimento do usuário: [Configure como os usuários consentem com os aplicativos](https://learn.microsoft.com/en-us/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal&amp;pivots=portal){target="_blank"}
* Consentimento do administrador: [Configurar o fluxo de trabalho de consentimento administrativo](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Ativar ou desativar o consentimento do usuário: [Gerenciamento do consentimento do usuário para aplicativos no Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365/admin/misc/user-consent?source=recommendations&amp;view=o365-worldwide){target="_blank"}
* Gerenciamento com o Microsoft Defender: [Gerenciar aplicativos OAuth](https://learn.microsoft.com/en-us/defender-cloud-apps/manage-app-permissions){target="_blank"}
