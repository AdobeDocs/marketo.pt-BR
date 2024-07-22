---
description: Configurar a integração do ON24 com o Marketo - Documentação do Marketo - Documentação do produto
title: Configurar a integração do ON24 com o Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Configurar a integração do ON24 com o Marketo{#set-up-the-on24-integration-with-marketo}

Veja como configurar sua integração de eventos ON24.

## Criar uma função somente API {#create-an-api-only-role}

1. Em Meu Marketo, clique em **Admin**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. Em Segurança, clique em **Usuários e funções**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Clique na guia **Funções** e depois em **Nova Função**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Insira um Nome de Função. Abra o menu **Acessar API** e selecione &quot;Objeto Personalizado de Leitura-Gravação&quot; e &quot;Pessoa de Leitura-Gravação&quot;. Clique em **Criar**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Criar um novo usuário {#create-a-new-user}

1. Ainda em Usuários e funções, clique na guia **Usuários** e em **Convidar novo usuário**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Insira as informações do novo usuário e clique em **Avançar**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Selecione a função Somente API ON24 que você acabou de criar. Marque a caixa de seleção **Somente API**. Clique em **Avançar**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Clique em **Enviar**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Um convite não é necessário para usuários somente API.

## Configurar conexão ON24 {#set-up-on24-connection}

1. Ainda na seção Admin, clique em **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Clique em **Novo** e depois em **Novo serviço**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Escolha um nome para exibição. Clique no menu suspenso **Serviço** e selecione **Personalizado**. Insira uma descrição. Clique na lista suspensa Somente Usuário da API e selecione o usuário criado [nas etapas acima](#create-a-new-user). Clique em **Criar**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Encontre o serviço LaunchPoint personalizado que você acabou de criar e clique em Exibir detalhes.

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Realce, clique com o botão direito do mouse, copie e salve a ID do cliente (você precisará dela mais tarde). Repita o procedimento para o Segredo do cliente.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Na árvore à esquerda, clique em Serviços da Web.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. Em &quot;REST API&quot;, realce, clique com o botão direito do mouse, copie e salve a primeira parte da Identidade (até o &#39;m&#39; em .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Com a ID do cliente, o segredo do cliente e a identidade salvos, navegue até a conta do ON24. O restante das etapas são executadas lá e estão [descritas aqui](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target="_blank"}.
