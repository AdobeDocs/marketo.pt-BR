---
unique-page-id: 2950555
description: Editar configurações de rich post do Facebook - Documentos do Marketo - Documentação do produto
title: Editar configurações de publicação avançada do Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 1%

---

# Editar configurações de publicação avançada do Facebook {#edit-facebook-rich-post-settings}

Personalize publicações quando as pessoas compartilharem você no Facebook.

>[!AVAILABILITY]
>
>Nem todos os clientes compraram essa funcionalidade. Confira os detalhes com seu representante de vendas.

Marketo [aplicativos sociais](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) permita que seus leads compartilhem suas landing pages com suas conexões em redes sociais, como Facebook, Twitter etc. Tags do facebook OpenGraph (tags OG) permitem especificar quais informações da sua página inicial estão incluídas em publicações do Facebook.

## Selecionar opções de publicação avançadas {#select-rich-post-options}

Você pode especificar os tipos de informações de página a serem usadas nas postagens avançadas do Facebook geradas por compartilhamentos de sua página de aterrissagem.

1. Selecionar **Mensagem facebook** no editor do **YouTube** vídeo ou botão social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Selecione uma das opções a seguir para sua mensagem do Facebook.

   * Adicionar conteúdo estático: Selecione essa opção para inserir o título, a legenda e a descrição manualmente.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Adicionar conteúdo dinâmico: Seu aplicativo social pode usar o `<TITLE>`, `<CAPTION>`e `<DESCRIPTION>` tags para preencher sua publicação avançada.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Eles já devem existir na origem da página, mas para ter mais controle, você pode adicionar tags OG específicas da Facebook à página inicial.

   * Não adicione conteúdo rico: Limita as publicações do Facebook da página de aterrissagem a apenas a mensagem principal e o link.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Adicionar tags OG da Facebook a uma página de aterrissagem {#add-facebook-og-tags-to-a-landing-page}

Para controlar os elementos da página que serão incluídos nos compartilhamentos da Facebook de sua página inicial, você pode adicionar tags OG (Gráfico aberto) da Facebook para título, legenda e descrição para sua página inicial.

1. Abra a landing page que contém a **Vídeo YouTube** ou social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   O **Designer de página de aterrissagem** abre em uma nova janela.

1. Selecionar **Ações da página de aterrissagem** > **Editar Meta Tags De Página**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Adicione o HTML que define og:title, og:caption e og:description. Copie e cole essas linhas e substitua o texto do espaço reservado:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenha cuidado para usar a sintaxe de HTML adequada ao adicionar as tags OG.
