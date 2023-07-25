---
unique-page-id: 12983390
description: Registre um aplicativo com o Azure para adquirir a ID do cliente/ID do aplicativo - Documentação do Marketo - Documentação do produto
title: Registrar um aplicativo com o Azure para adquirir a ID do cliente/ID do aplicativo
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Registrar um aplicativo com o Azure para adquirir a ID do cliente/ID do aplicativo {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

O Azure Ative Diretory estende seus diretórios locais na nuvem, fornecendo suporte ao MS Dynamics 365 CRM com autenticação ADFS local.

## Registrando um novo aplicativo {#registering-a-new-app}

1. [Fazer logon](https://login.microsoftonline.com/){target="_blank"} ao portal de gerenciamento do Microsoft Azure usando uma conta com permissões de administrador. Você também pode acessar o portal do Microsoft Azure por meio do Centro de Administração do Office 365 expandindo o **Admin** no painel de navegação esquerdo e selecionando **Azure AD**.

   >[!CAUTION]
   >
   >Você deve usar uma conta na mesma assinatura do Office 365 que aquela com a qual pretende registrar o aplicativo.

   >[!NOTE]
   >
   >Se você não tiver uma conta do Azure, poderá [inscrever-se](https://azure.microsoft.com/en-us/free/){target="_blank"} por um. Consulte a documentação da Microsoft ou entre em contato com o representante da Microsoft para obter mais informações. Depois de criar uma conta do Azure, você pode registrar um ou mais aplicativos usando o procedimento descrito abaixo.
   >
   >
   >Se você tiver uma conta do Azure, mas sua assinatura do Office 365 com o Microsoft Dynamics 365 não estiver disponível em sua assinatura do Azure, siga [estas instruções](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} para associar as duas contas.

1. Localize e clique em **Azure Ative Diretory** no painel de navegação esquerdo.

   ![](assets/two.png)

1. Em Gerenciar, clique em **Registros do aplicativo**.

   ![](assets/three.png)

1. Clique em **Novo registro** na parte superior da página.

   ![](assets/four.png)

1. Insira um nome para o aplicativo, escolha o tipo de conta aplicável e insira um URL de redirecionamento. Clique em **Registrar** na parte inferior da página.

   ![](assets/five.png)

1. Agora você deve ver seu aplicativo no **Registros do aplicativo** guia.

   ![](assets/six.png)

## Configuração de permissões do aplicativo {#configuring-app-permissions}

1. No **Registros do aplicativo** no Ative Diretory, clique no aplicativo para o qual deseja configurar permissões.

   ![](assets/seven.png)

1. Em Gerenciar, clique em **Permissões de API**.

   ![](assets/eight.png)

1. Clique em **Adicionar uma permissão** botão.

   ![](assets/nine.png)

1. Escolher **Dynamics CRM**.

   ![](assets/ten.png)

1. Verifique a **Acessar o Serviço de dados comum como usuário da organização***s** e clique em **Adicionar permissões.**

   ![](assets/eleven.png)

1. Depois que as permissões forem adicionadas com êxito, aguarde pelo menos 10 segundos.

   ![](assets/twelve.png)

1. Clique em **Dar consentimento administrativo** botão.

   ![](assets/thirteen.png)

1. Clique em **Sim** para confirmar.

   ![](assets/fourteen.png)

   E pronto!

   ![](assets/fifteen.png)
