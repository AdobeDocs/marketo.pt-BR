---
unique-page-id: 2950549
description: Configurar Fluxo Social Recomendado - Documentação Do Marketo - Documentação Do Produto
title: Configurar fluxo social recomendado
exl-id: 01b54215-4a0c-4639-80d2-ec30603b3695
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Configurar fluxo social recomendado {#configure-social-recommend-flow}

Ao criar um aplicativo social, você pode configurar as opções de rede social e os prompts que um usuário encontra ao se inscrever.

>[!IMPORTANT]
>
>Em 31 de julho de 2024, iniciamos o processo de desativação desse recurso. Você não poderá criar novos ativos. Os ativos existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Selecionar redes para compartilhamento {#select-networks-for-sharing}

>[!NOTE]
>
>Isso é muito semelhante a [configurar o fluxo de compartilhamento/inscrição social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/configure-social-sign-up-share-flow.md), mas isso é para os links de compartilhamento _em_ no aplicativo social.

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione o aplicativo e clique em **Editar rascunho**.

   ![](assets/image2014-9-22-11-3a51-3a6.png)

1. No editor de aplicativo social, vá para **Fluxo recomendado** > **Redes sociais**.

   ![](assets/recommendedflow.png)

1. Selecione as redes para as quais um usuário pode compartilhar.

   ![](assets/socialnetworkschoose.png)

## Configurar a mensagem do Facebook {#configure-the-facebook-message}

1. Configure a mensagem que aparecerá nas publicações do Facebook.

   ![](assets/image2014-9-22-11-3a53-3a21.png)

   >[!NOTE]
   >
   >Em um compartilhamento de vídeo, a miniatura é gerada automaticamente.

   Se você escolher **Adicionar conteúdo dinâmico**, os valores das marcas OpenGraph da página (og:title, og:caption e og:description) e a miniatura serão adicionados automaticamente às postagens do Facebook. Consulte a próxima etapa.

   Se você escolher **Adicionar conteúdo estático**, insira o título, a legenda e a descrição e carregue uma imagem. Consulte as próximas duas etapas.

1. Na janela Exibir e editar, clique em **Mostrar edições** para personalizar o prompt de compartilhamento e a mensagem que aparecerão nas publicações do Facebook.

   >[!TIP]
   >
   >Para obter mais informações, consulte [Editar configurações de postagem avançada do Facebook](/help/marketo/product-docs/demand-generation/facebook/edit-facebook-rich-post-settings.md).

   ![](assets/image2014-9-22-11-3a54-3a36.png)

   >[!NOTE]
   >
   >A [URL de compartilhamento](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) é adicionada automaticamente a todas as mensagens de compartilhamento.

1. Se você escolheu **Adicionar conteúdo estático** acima, edite o título, a legenda e a descrição e carregue uma imagem personalizada (das Imagens e Arquivos do Marketo).

   ![](assets/image2014-9-22-11-3a55-3a14.png)

   Consulte [Adicionar imagens e arquivos ao Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Ao carregar uma imagem, você não a verá aqui até fechar e reabrir o editor do aplicativo social.

1. Clique em **Avançar**.

Se você escolher , os valores das tags OpenGraph da página (og:title, og:caption e og:description) e a miniatura serão adicionados automaticamente às publicações do Facebook. Consulte a próxima etapa.

## Configurar a mensagem de Twitter {#configure-the-twitter-message}

1. Clique em para editar o prompt de compartilhamento e a mensagem que aparecerá nos tweets do Twitter.

   ![](assets/image2014-9-22-12-3a2-3a40.png)

   >[!TIP]
   >
   >Use {html_title} no texto do tweet para exibir o título da página automaticamente.

1. Clique em **Avançar**.

## Configurar a mensagem do LinkedIn {#configure-the-linkedin-message}

1. Configure a mensagem que aparecerá nas publicações do LinkedIn.

   ![](assets/image2014-9-22-12-3a3-3a21.png)

   Se você escolher **Adicionar conteúdo dinâmico**, os valores das marcas de página (título e descrição) e a miniatura serão adicionados automaticamente às postagens do LinkedIn. Consulte a próxima etapa.

   Se você escolher **Adicionar estático**, insira o título, a legenda e a descrição e carregue uma imagem. Consulte as próximas duas etapas.

1. Na janela **Exibir e editar**, clique em **Mostrar edições** e edite o prompt de compartilhamento e a mensagem que aparecerão nas publicações do LinkedIn.

   ![](assets/image2014-9-22-12-3a3-3a38.png)

   >[!TIP]
   >
   >Use {html_title} no texto da postagem para exibir o título da página automaticamente.

1. Se você escolheu **Adicionar estático** conteúdo acima, edite o título e a descrição e carregue uma imagem personalizada (das imagens e arquivos do Marketo).

   ![](assets/image2014-9-22-12-3a4-3a43.png)

   Consulte [Adicionar imagens e arquivos ao Marketo](/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md).

   >[!NOTE]
   >
   >Ao carregar uma imagem, você não a verá aqui até fechar e reabrir o editor do aplicativo social.

1. Clique em **Avançar**.

## Configurar a mensagem de confirmação {#configure-the-confirmation-message}

1. Editar o texto da confirmação do compartilhamento.

   ![](assets/image2014-9-22-12-3a5-3a30.png)

1. Clique em **Concluir** > **Aprovar** e **Fechar**.

   ![](assets/image2014-9-22-12-3a5-3a45.png)

>[!MORELIKETHIS]
>
>A próxima etapa é [adicionar o compartilhamento de vídeo](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-video-share-flow.md) ou a [votação](/help/marketo/product-docs/demand-generation/social/creating-a-poll/create-a-poll.md) a uma página de aterrissagem, Facebook ou a seu próprio site.
