---
unique-page-id: 12983390
description: Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo - Documentos do marketing - Documentação do produto
title: Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

O Azure Ative Diretory estende seus diretórios locais para a nuvem, fornecendo suporte para o MS Dynamics 365 CRM com autenticação ADFS local.

## Registrando um novo aplicativo {#registering-a-new-app}

1. [Efetue logon ](http://manage.windowsazure.com/) no portal de gerenciamento do Microsoft Azure usando uma conta com permissões de administrador. Você também pode acessar o portal do Microsoft Azure pelo Centro de Administração do Office 365 expandindo o item **Admin** no painel de navegação esquerdo e selecionando **Azure AD**.

   >[!CAUTION]
   >
   >Você deve usar uma conta na mesma subscrição do Office 365 que aquela com a qual você pretende registrar o aplicativo.

   >[!NOTE]
   >
   >Se você não tiver uma conta do Azure, poderá [inscrever-se](https://azure.microsoft.com/en-us/free/) para uma. Consulte a documentação da Microsoft ou entre em contato com seu representante da Microsoft para obter mais informações. Depois de criar uma conta do Azure, você pode registrar um ou mais aplicativos usando o procedimento descrito abaixo.
   >
   >
   >Se você tiver uma conta do Azure, mas sua subscrição do Office 365 com o Microsoft Dynamics 365 não estiver disponível na subscrição do Azure, siga [estas instruções](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) para associar as duas contas.

1. Localize e clique em **Azure Ative Diretory** no painel de navegação esquerdo.

   ![](assets/two.png)

1. Em Gerenciar, clique em **Registros do aplicativo**.

   ![](assets/three.png)

1. Clique em **Novo registro** na parte superior da página.

   ![](assets/four.png)

1. Insira um nome para o aplicativo, escolha o tipo de conta aplicável e insira um URL de redirecionamento. Em seguida, clique em **Register** na parte inferior da página.

   ![](assets/five.png)

1. Agora você deve ver seu aplicativo na guia **Registros do aplicativo**.

   ![](assets/six.png)

## Configuração das permissões do aplicativo {#configuring-app-permissions}

1. Na guia **Registros do aplicativo** no Ative Diretory, clique no aplicativo para o qual deseja configurar permissões.

   ![](assets/seven.png)

1. Em Gerenciar, clique em **permissões da API**.

   ![](assets/eight.png)

1. Clique no botão **Adicionar uma permissão**.

   ![](assets/nine.png)

1. Escolha **Dynamics CRM**.

   ![](assets/ten.png)

1. Marque a caixa **Acessar o Serviço de Dados Comuns como usuário da organização****s** e clique em **Adicionar permissões.**

   ![](assets/eleven.png)

1. Depois que as permissões forem adicionadas com êxito, aguarde pelo menos 10 segundos.

   ![](assets/twelve.png)

1. Clique no botão **Conceder consentimento admin**.

   ![](assets/thirteen.png)

1. Clique em **Yes** para confirmar.

   ![](assets/fourteen.png)

   E você terminou!

   ![](assets/fifteen.png)

