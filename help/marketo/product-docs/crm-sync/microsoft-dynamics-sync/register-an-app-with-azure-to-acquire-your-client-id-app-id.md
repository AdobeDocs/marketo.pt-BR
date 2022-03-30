---
unique-page-id: 12983390
description: Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo - Documentos do Marketo - Documentação do produto
title: Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
source-git-commit: 6ad418c8f4056b9a2fb31b0ac995692f0c618795
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Registre um aplicativo com o Azure para adquirir sua ID do cliente/ID do aplicativo {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

O Azure Ative Diretory estende seus diretórios locais na nuvem, fornecendo suporte para o MS Dynamics 365 CRM com autenticação ADFS local.

## Registro de um novo aplicativo {#registering-a-new-app}

1. [Fazer logon](https://azure.microsoft.com/en-us/account/) ao portal de gerenciamento do Microsoft Azure usando uma conta com permissões de administrador. Também é possível acessar o portal do Microsoft Azure por meio do Admin Center do Office 365 expandindo o **Administrador** no painel de navegação esquerdo e selecionando **Azure AD**.

   >[!CAUTION]
   >
   >Você deve usar uma conta na mesma assinatura do Office 365 que a conta com a qual pretende registrar o aplicativo.

   >[!NOTE]
   >
   >Se você não tiver uma conta do Azure, poderá [inscrever-se](https://azure.microsoft.com/en-us/free/) por um. Consulte a documentação da Microsoft ou entre em contato com o representante da Microsoft para obter mais informações. Depois de criar uma conta do Azure, você pode registrar um ou mais aplicativos usando o procedimento descrito abaixo.
   >
   >
   >Se você tiver uma conta do Azure, mas sua assinatura do Office 365 com o Microsoft Dynamics 365 não estiver disponível em sua assinatura do Azure, siga [estas instruções](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) associar as duas contas.

1. Localizar e clicar em **Ative Diretory do Azure** no painel de navegação esquerdo.

   ![](assets/two.png)

1. Em Gerenciar , clique em **Registros do aplicativo**.

   ![](assets/three.png)

1. Clique em **Novo registro** na parte superior da página.

   ![](assets/four.png)

1. Insira um nome para o aplicativo, escolha o tipo de conta aplicável e insira um URL de redirecionamento. Em seguida, clique em **Registrar** na parte inferior da página.

   ![](assets/five.png)

1. Agora você deve ver seu aplicativo no **Registros do aplicativo** guia .

   ![](assets/six.png)

## Configuração das permissões do aplicativo {#configuring-app-permissions}

1. Em **Registros do aplicativo** no Ative Diretory, clique no aplicativo para o qual deseja configurar permissões.

   ![](assets/seven.png)

1. Em Gerenciar , clique em **Permissões de API**.

   ![](assets/eight.png)

1. Clique no botão **Adicionar permissão** botão.

   ![](assets/nine.png)

1. Choose **Dynamics CRM**.

   ![](assets/ten.png)

1. Verifique a **Acesso ao Serviço de dados comum como usuário da organização***s** e, em seguida, clique em **Adicione permissões.**

   ![](assets/eleven.png)

1. Depois que as permissões forem adicionadas com êxito, aguarde pelo menos 10 segundos.

   ![](assets/twelve.png)

1. Clique no botão **Conceder consentimento administrativo** botão.

   ![](assets/thirteen.png)

1. Clique em **Sim** para confirmar.

   ![](assets/fourteen.png)

   E você acabou!

   ![](assets/fifteen.png)
