---
description: Etapa 2 de 4 - Configurar a solução da Marketo com a conexão de controle de senha de proprietário de recurso - Documentação da Marketo - Documentação do produto
title: Etapa 2 de 4 - Configurar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Etapa 2 de 4: Configurar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso {#step-2-of-4-set-up-the-marketo-solution-ropc}

Vamos começar criando uma conta de usuário.

>[!PREREQUISITES]
>
>[Etapa 1 de 4: Instalar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Criar um novo usuário {#create-a-new-user}

1. Faça logon em [!DNL Dynamics]. Clique no ícone [!UICONTROL Configurações] e selecione **[!UICONTROL Configurações Avançadas]**.

   ![](assets/one.png)

1. Clique em **[!UICONTROL Configurações]** e selecione **[!UICONTROL Segurança]**.

   ![](assets/two.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/three.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/four.png)

1. Clique em **[!UICONTROL Adicionar e licenciar usuários]** na nova janela.

   ![](assets/five.png)

1. Uma nova guia é aberta. Clique em **[!UICONTROL Administrador]** na parte superior da página.

   ![](assets/six.png)

1. Outra nova guia é aberta. Clique em **[!UICONTROL Adicionar um usuário]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >O usuário de sincronização deve ter permissão de leitura para a configuração do Marketo.

1. Insira todas as suas informações. Quando terminar, clique em **[!UICONTROL Adicionar]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Esse nome deve ser um usuário de sincronização dedicado e não uma conta existente de usuário do CRM. Não precisa ser um endereço de email real.

1. Insira o email para receber as novas credenciais de usuário e clique em **[!UICONTROL Enviar email e fechar]**.

   ![](assets/nine.png)

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função de Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Você não precisa atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica à versão 4.0.0.14 e posterior do Marketo. Para versões anteriores, todos os usuários devem ter a função de usuário sincronizar. Para atualizar o Marketo, consulte [Atualizar Solução Marketo para [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de Sincronização [ deve ser definida como Inglês](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Volte para a guia [!UICONTROL Usuários Habilitados] e atualize a lista de usuários.

   ![](assets/ten.png)

1. Passe o mouse ao lado do usuário recém-criado do Marketo Sync e uma caixa de seleção será exibida. Clique para selecioná-la.

   ![](assets/eleven.png)

1. Clique em **[!UICONTROL Gerenciar Funções]**.

   ![](assets/twelve.png)

1. Marque **[!UICONTROL Usuário da Sincronização do Marketo]** e clique em **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Quaisquer atualizações feitas em seu CRM pelo Usuário da Sincronização _não_ serão sincronizadas com o Marketo novamente.

## Configurar a solução da Marketo {#configure-marketo-solution}

Quase lá! Tudo o que resta é informar a solução Marketo sobre o novo usuário criado.

1. Volte para a seção [!UICONTROL Configurações Avançadas], clique no ícone ![](assets/image2015-5-13-15-3a49-3a19.png) ao lado de [!UICONTROL Configurações] e selecione **[!UICONTROL Configuração do Marketo]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se você não vir a **[!UICONTROL Configuração do Marketo]** no menu [!UICONTROL Configurações], atualize a página. Se isso não funcionar, tente [publicar a Solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) novamente ou sair e entrar novamente.

1. Clique em **[!UICONTROL Padrão]**.

   ![](assets/fifteen.png)

1. Clique no botão de pesquisa no campo **[!UICONTROL Usuário do Marketo]** e selecione o usuário de sincronização criado.

   ![](assets/sixteen.png)

1. Clique no ícone ![](assets/image2015-3-13-15-3a10-3a11.png) no canto inferior direito para salvar as alterações.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Clique no **X** no canto superior direito para fechar a tela.

   ![](assets/seventeen.png)

1. Clique no ícone ![](assets/image2015-5-13-15-3a49-3a19-1.png) ao lado de [!UICONTROL Configurações] e selecione **[!UICONTROL Soluções]**.

   ![](assets/eighteen.png)

1. Clique no botão **[!UICONTROL Publicar todas as personalizações]**.

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Etapa 3 de 4: Conectar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
