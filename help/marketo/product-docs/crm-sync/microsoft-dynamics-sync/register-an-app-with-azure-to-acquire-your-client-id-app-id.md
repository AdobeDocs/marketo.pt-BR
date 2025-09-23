---
unique-page-id: 12983390
description: Registre um aplicativo com o Azure para adquirir a ID do cliente/ID do aplicativo - Documentação do Marketo - Documentação do produto
title: Registrar um aplicativo com o Azure para adquirir a ID do cliente/ID do aplicativo
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 7%

---

# Registrar um aplicativo com o Azure para adquirir a ID do cliente/ID do aplicativo {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

O Ative Diretory do Azure estende seus diretórios locais na nuvem, fornecendo suporte ao CRM do [!DNL MS Dynamics 365] com autenticação ADFS local.

## Registrando um novo aplicativo {#registering-a-new-app}

1. [Faça logon](https://login.microsoftonline.com/){target="_blank"} no portal de gerenciamento do Microsoft Azure usando uma conta com permissões de administrador. Você também pode acessar o portal do Microsoft Azure por meio do Centro de Administração do Office 365, expandindo o item **[!UICONTROL Administrador]** no painel de navegação esquerdo e selecionando **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >Você deve usar uma conta na mesma assinatura do [!DNL Office 365] que a conta com a qual pretende registrar o aplicativo.

   >[!NOTE]
   >
   >Se você não tiver uma conta do Azure, poderá [inscrever-se](https://azure.microsoft.com/en-us/free/){target="_blank"} para uma conta. Consulte a documentação da Microsoft ou entre em contato com o representante da Microsoft para obter mais informações. Depois de criar uma conta do Azure, você pode registrar um ou mais aplicativos usando o procedimento descrito abaixo.
   >
   >
   >Se você tiver uma conta do Azure, mas sua assinatura do [!DNL Office 365] com [!DNL Microsoft Dynamics 365] não estiver disponível em sua assinatura do Azure, siga [estas instruções](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} para associar as duas contas.

1. Localize e clique em **[!UICONTROL Azure Ative Diretory]** no painel de navegação esquerdo.

   ![](assets/two.png)

1. Em [!UICONTROL Gerenciar], clique em **[!UICONTROL Registros de aplicativo]**.

   ![](assets/three.png)

1. Clique em **[!UICONTROL Novo registro]** na parte superior da página.

   ![](assets/four.png)

1. Insira um nome para o aplicativo, escolha o tipo de conta aplicável e insira um URL de redirecionamento. Em seguida, clique em **[!UICONTROL Registrar]** na parte inferior da página.

   ![](assets/five.png)

1. Agora você deve ver seu aplicativo na guia **[!UICONTROL Registros de aplicativo]**.

   ![](assets/six.png)

## Configuração de permissões do aplicativo {#configuring-app-permissions}

1. Na guia **[!UICONTROL Registros de aplicativo]** do Ative Diretory, clique no aplicativo para o qual deseja configurar permissões.

   ![](assets/seven.png)

1. Em [!UICONTROL Gerenciar], clique em **[!UICONTROL Permissões de API]**.

   ![](assets/eight.png)

1. Clique no botão **[!UICONTROL Adicionar uma permissão]**.

   ![](assets/nine.png)

1. Escolha o **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Marque a caixa **[!UICONTROL Acessar o Common Data Service como usuários da organização]** e clique em **[!UICONTROL Adicionar permissões].**

   ![](assets/eleven.png)

1. Depois que as permissões forem adicionadas com êxito, aguarde pelo menos 10 segundos.

   ![](assets/twelve.png)

1. Clique no botão **[!UICONTROL Dar consentimento administrativo]**.

   ![](assets/thirteen.png)

1. Clique em **[!UICONTROL Sim]** para confirmar.

   ![](assets/fourteen.png)

   E pronto!

   ![](assets/fifteen.png)
