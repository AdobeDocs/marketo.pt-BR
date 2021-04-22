---
unique-page-id: 12983390
description: Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo - Documentos do Marketo - Documentação do produto
title: Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

O Azure Ative Diretory estende seus diretórios locais na nuvem, fornecendo suporte para o MS Dynamics 365 CRM com autenticação ADFS local.

## Registrar um novo aplicativo {#registering-a-new-app}

1. [Faça logon ](https://manage.windowsazure.com/) no portal de gerenciamento do Microsoft Azure usando uma conta com permissões de administrador. Também é possível acessar o portal do Microsoft Azure por meio do Admin Center do Office 365 expandindo o item **Admin** no painel de navegação esquerdo e selecionando **Azure AD**.

   >[!CAUTION]
   >
   >Você deve usar uma conta na mesma assinatura do Office 365 que a conta com a qual pretende registrar o aplicativo.

   >[!NOTE]
   >
   >Se você não tiver uma conta do Azure, poderá [inscrever-se](https://azure.microsoft.com/en-us/free/) para uma. Consulte a documentação da Microsoft ou entre em contato com seu representante da Microsoft para obter mais informações. Depois de criar uma conta do Azure, você pode registrar um ou mais aplicativos usando o procedimento descrito abaixo.
   >
   >
   >Se você tiver uma conta do Azure, mas sua assinatura do Office 365 com o Microsoft Dynamics 365 não estiver disponível em sua assinatura do Azure, siga [estas instruções](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) para associar as duas contas.

1. Localize e clique em **Azure Ative Diretory** no painel de navegação esquerdo.

   ![](assets/two.png)

1. Em Gerenciar, clique em **Registros do aplicativo**.

   ![](assets/three.png)

1. Clique em **New registration** na parte superior da página.

   ![](assets/four.png)

1. Insira um nome para o aplicativo, escolha o tipo de conta aplicável e insira um URL de redirecionamento. Em seguida, clique em **Register** na parte inferior da página.

   ![](assets/five.png)

1. Agora você deve ver seu aplicativo na guia **Registros do aplicativo**.

   ![](assets/six.png)

## Configurar permissões do aplicativo {#configuring-app-permissions}

1. Na guia **Registros de aplicativos** no Ative Diretory, clique no aplicativo para o qual deseja configurar permissões.

   ![](assets/seven.png)

1. Em Gerenciar, clique em **Permissões de API**.

   ![](assets/eight.png)

1. Clique no botão **Adicionar uma permissão**.

   ![](assets/nine.png)

1. Escolha **Dynamics CRM**.

   ![](assets/ten.png)

1. Marque a caixa **Acessar o Serviço de Dados Comum como usuário da organização***s** e clique em **Adicionar permissões.**

   ![](assets/eleven.png)

1. Depois que as permissões forem adicionadas com êxito, aguarde pelo menos 10 segundos.

   ![](assets/twelve.png)

1. Clique no botão **Conceder consentimento do administrador**.

   ![](assets/thirteen.png)

1. Clique em **Sim** para confirmar.

   ![](assets/fourteen.png)

   E você acabou!

   ![](assets/fifteen.png)
