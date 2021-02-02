---
unique-page-id: 3571827
description: Etapa 2 de 3 - Configurar usuário de sincronização de marketing no Dynamics - Documentos de marketing - Documentação do produto
title: Etapa 2 de 3 - Configurar usuário de sincronização de marketing no Dynamics
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---


# Etapa 2 de 3: Configurar usuário de sincronização de marketing no Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Vamos começar criando uma conta de usuário.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Instalar a solução Marketing (Online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)

## Criar um novo usuário {#create-a-new-user}

1. Faça logon no Dynamics. Clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Segurança**.

   ![](assets/two.png)

1. Clique em **Usuários**.

   ![](assets/three.png)

1. Clique em **Novo.**

   ![](assets/four.png)

1. Clique em **Adicionar e licenciar usuários** na nova janela.

   ![](assets/five.png)

1. Uma nova guia é aberta. Clique em **Admin** na parte superior da página.

   ![](assets/six.png)

1. Uma nova guia é aberta. Clique em **Adicionar um usuário**.

   ![](assets/seven.png)

1. Insira todas as suas informações. Quando terminar, clique em **Adicionar**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Esse nome deve ser um usuário de sincronização dedicado e não uma conta de usuário do CRM existente. Não precisa ser um endereço de email real.

1. Digite o email para receber as novas credenciais do usuário e clique em **Enviar email e fechar**.

   ![](assets/nine.png)

## Atribuir função de usuário de sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização de marketing somente ao usuário de sincronização de marketing. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica à versão 4.0.0.14 e posterior do Marketo. Para versões anteriores, todos os usuários devem ter a função de usuário de sincronização. Para atualizar o Marketo, consulte [Upgrade Marketing Solution for Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Volte para a guia Usuários habilitados e atualize a lista de usuários.

   ![](assets/ten.png)

1. Passe o mouse ao lado do usuário recém-criado da Sincronização de marketing e uma caixa de seleção será exibida. Clique para selecioná-lo.

   ![](assets/eleven.png)

1. Clique em **Gerenciar funções**.

   ![](assets/twelve.png)

1. Marque **Usuário de sincronização de marketing** e clique em **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Todas as atualizações feitas em seu CRM pelo Usuário de sincronização serão **e não** sincronizadas de volta ao Marketo.

## Configurar a solução de marketing {#configure-marketo-solution}

Quase lá! Tudo o que nos resta é informar a Solução de marketing sobre o novo usuário criado.

1. Volte para a seção Configurações avançadas e clique no ícone ![](assets/image2015-5-13-15-3a49-3a19.png) ao lado de Configurações e selecione **Configuração do marketing**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se você não vir **Configuração do Marketing** no menu Configurações, atualize a página. Se isso não funcionar, tente [publicar novamente a solução Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) ou faça logout e volte a fazer logon.

1. Clique em **Padrão**.

   ![](assets/fifteen.png)

1. Clique no botão de pesquisa no campo **Usuário do Marketing** e selecione o usuário de sincronização que você criou.

   ![](assets/sixteen.png)

1. Clique no ícone ![](assets/image2015-3-13-15-3a10-3a11.png) no canto inferior direito para salvar as alterações.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Clique no **X** no canto superior direito para fechar a tela.

   ![](assets/seventeen.png)

1. Clique no ícone ![](assets/image2015-5-13-15-3a49-3a19-1.png) ao lado de Configurações e selecione **Soluções**.

   ![](assets/eighteen.png)

1. Clique no botão **Publicar todas as personalizações**.

   ![](assets/nineteen.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

    * Se você quiser restringir o número de registros que sincronizar, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
    * Execute o processo [Validar Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
    * Faça logon no usuário de sincronização de marketing no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conectar o Microsoft Dynamics com o Marketing (Online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
