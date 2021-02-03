---
unique-page-id: 2950555
description: Editar configurações de postagens avançadas do Facebook - Documentos de marketing - Documentação do produto
title: Editar configurações de postagens avançadas do Facebook
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---


# Editar configurações de postagens avançadas do Facebook {#edit-facebook-rich-post-settings}

Personalize publicações quando as pessoas compartilham você no Facebook.

>[!AVAILABILITY]
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com seu representante de vendas para obter detalhes.

Marketo [aplicativos sociais](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) permite que seus clientes potenciais compartilhem suas landings page com suas conexões em redes sociais, como Facebook, Twitter etc. As tags OpenGraph do Facebook (tags OG) permitem que você especifique quais informações de sua landing page estão incluídas nas publicações do Facebook.

## Selecionar opções avançadas de publicação {#select-rich-post-options}

Você pode especificar os tipos de informações de página a serem usadas nas publicações avançadas do Facebook geradas por compartilhamentos de sua landing page.

1. Selecione **Mensagem do Facebook** no editor para o seu **YouTube** vídeo ou botão social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Selecione uma das seguintes opções para sua Mensagem do Facebook.

   * Adicionar conteúdo estático: Selecione essa opção para inserir o título, a legenda e a descrição manualmente.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Adicionar conteúdo dinâmico: Seu aplicativo social pode usar as tags `<TITLE>`, `<CAPTION>` e `<DESCRIPTION>` do landing page para preencher sua publicação avançada.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Eles já devem existir na fonte da página, mas para ter mais controle, você pode adicionar tags OG específicas do Facebook à sua landing page.

   * Não adicione conteúdo rico: Limita as publicações do Facebook da sua landing page apenas à mensagem principal e ao link.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Adicionar tags OG do Facebook a uma Landing page {#add-facebook-og-tags-to-a-landing-page}

Para controlar os elementos da página que serão incluídos nos compartilhamentos do Facebook de sua landing page, você pode adicionar tags OG (Gráfico aberto) do Facebook para título, legenda e descrição à sua landing page.

1. Abra a landing page que contém seu **vídeo do YouTube** ou botão social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   O **Designer de Landing page** é aberto em uma nova janela.

1. Selecione **Ações de Landing page** > **Editar marcas meta de página**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Adicione o HTML que define og:title, og:caption e og:description. Copie e cole essas linhas e substitua o texto do espaço reservado:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenha cuidado para usar a sintaxe HTML adequada ao adicionar as tags OG.
