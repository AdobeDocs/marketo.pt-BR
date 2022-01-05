---
unique-page-id: 3571827
description: Etapa 2 de 3 - Configurar a solução da Marketo com a conexão S2S - Documentos da Marketo - Documentação do produto
title: Etapa 2 de 3 - Configurar a solução Marketo com a conexão S2S
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 8b4d86f2dd5f19abb56451403cd2638b1a852d79
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Etapa 2 de 3: Configurar o usuário do Marketo Sync no Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Vamos começar criando uma conta de usuário.

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Instalar a solução Marketo com a conexão S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)

## Criar um novo usuário {#create-a-new-user}

1. Faça logon no Dynamics. Clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Segurança**.

   ![](assets/two.png)

1. Clique em **Usuários**.

   ![](assets/three.png)

1. Clique em **Novo.**

   ![](assets/four.png)

1. Clique em **Adicionar e Licenciar Usuários** na nova janela.

   ![](assets/five.png)

1. Uma nova guia é aberta. Clique em **Administrador** na parte superior da página.

   ![](assets/six.png)

1. Outra nova guia é aberta. Clique em **Adicionar um usuário**.

   ![](assets/seven.png)

1. Insira todas as suas informações. Quando terminar, clique em **Adicionar**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Esse nome deve ser um usuário de sincronização dedicado e não uma conta de usuário do CRM existente. Não precisa ser um endereço de email real.

1. Digite o email para receber as novas credenciais do usuário e clique em **Enviar e-mail e fechar**.

   ![](assets/nine.png)

## Atribuir Função de Usuário de Sincronização {#assign-sync-user-role}

Atribua a função Usuário de sincronização do Marketo somente ao usuário de sincronização do Marketo. Não é necessário atribuí-lo a nenhum outro usuário.

>[!NOTE]
>
>Isso se aplica ao Marketo versão 4.0.0.14 e posterior. Para versões anteriores, todos os usuários devem ter a função de sincronização do usuário. Para atualizar o Marketo, consulte [Atualizar a solução Marketo para o Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>A configuração de idioma do Usuário de sincronização [deve ser definido como inglês](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Volte para a guia Usuários ativados e atualize a lista de usuários.

   ![](assets/ten.png)

1. Passe o mouse sobre o usuário recém-criado do Marketo Sync , e uma caixa de seleção será exibida. Clique em para selecioná-lo.

   ![](assets/eleven.png)

1. Clique em **Gerenciar funções**.

   ![](assets/twelve.png)

1. Verificar **Usuário do Marketo Sync** e clique em **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Qualquer atualização feita em seu CRM pelo Usuário de sincronização **not** ser sincronizado de volta ao Marketo.

## Configurar a solução Marketo {#configure-marketo-solution}

Quase lá! Resta informar a Marketo Solution sobre o novo usuário criado.

1. Volte para a seção Configurações avançadas e clique no botão ![](assets/image2015-5-13-15-3a49-3a19.png) ícone ao lado de Configurações e selecione **Configuração do Marketo**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Se você não vir **Configuração do Marketo** no menu Configurações , atualize a página. Se isso não funcionar, tente [publicar a solução Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md) novamente ou faça logoff e volte.

1. Clique em **Padrão**.

   ![](assets/fifteen.png)

1. Clique no botão de pesquisa na **Usuário do Marketo** e selecione o usuário de sincronização que você criou.

   ![](assets/sixteen.png)

1. Clique no botão ![](assets/image2015-3-13-15-3a10-3a11.png) no canto inferior direito para salvar as alterações.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Clique no botão **X** no canto superior direito para fechar a tela.

   ![](assets/seventeen.png)

1. Clique no botão ![](assets/image2015-5-13-15-3a49-3a19-1.png) ícone ao lado de Configurações e selecione **Soluções**.

   ![](assets/eighteen.png)

1. Clique no botão **Publicar todas as personalizações** botão.

   ![](assets/nineteen.png)

## Antes de prosseguir para a Etapa 3 {#before-proceeding-to-step}

    * Se quiser restringir o número de registros sincronizados, [configure um filtro de sincronização personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) agora.
    * Execute o processo [Validar o Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md). Ele verifica se as configurações iniciais foram feitas corretamente.
    * Efetue logon no usuário de sincronização do Marketo no Microsoft Dynamics CRM.

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Conecte a solução Marketo com a conexão S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)
