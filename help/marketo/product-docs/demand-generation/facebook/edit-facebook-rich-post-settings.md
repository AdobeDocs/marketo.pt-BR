---
unique-page-id: 2950555
description: Editar configurações avançadas de publicação do Facebook - Documentação do Marketo - Documentação do produto
title: Editar configurações de publicação avançada do Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
feature: Integrations
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# Editar configurações de publicação avançada do Facebook {#edit-facebook-rich-post-settings}

Personalize publicações quando as pessoas compartilharem você no Facebook.

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

Marketo [aplicativos sociais](/help/marketo/product-docs/demand-generation/social/social-functions/add-a-social-button-on-a-landing-page.md) permitir que seus clientes em potencial compartilhem suas páginas de aterrissagem com as conexões deles em redes sociais, como Facebook, Twitter etc. As tags do facebook OpenGraph (tags OG) permitem especificar quais informações da página de aterrissagem são incluídas em publicações do Facebook.

## Selecionar opções de publicação avançadas {#select-rich-post-options}

Você pode especificar os tipos de informações de página a serem usados nas publicações avançadas do Facebook geradas por compartilhamentos da sua página de aterrissagem.

1. Selecionar **Mensagem do facebook** no editor do seu **YouTube** vídeo ou botão social.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Selecione entre as seguintes opções para a mensagem do Facebook.

   * Adicionar conteúdo estático: selecione essa opção para inserir o título, a legenda e a descrição manualmente.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Adicionar conteúdo dinâmico: seu aplicativo social pode usar a da sua landing page `<TITLE>`, `<CAPTION>`, e `<DESCRIPTION>` para preencher sua publicação avançada.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Eles já devem existir na fonte da página, mas, para obter mais controle, é possível adicionar tags OG da Facebook específicas à página de aterrissagem.

   * Não adicionar conteúdo avançado: limita as publicações do Facebook da página de aterrissagem somente à mensagem e ao link principais.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Adicionar tags OG da Facebook a uma página de aterrissagem {#add-facebook-og-tags-to-a-landing-page}

Para controlar os elementos de página que serão incluídos nos compartilhamentos da Facebook a partir da página de aterrissagem, é possível adicionar tags OG (Open Graph) da Facebook para título, legenda e descrição à página de aterrissagem.

1. Abra a landing page que contém seu **Vídeo do YouTube** ou social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   A variável **Designer de landing page** abre em uma nova janela.

1. Selecionar **Ações da landing page** > **Editar metatags de página**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Adicione o HTML que define og:title, og:caption e og:description. Copie e cole essas linhas e substitua o texto do espaço reservado:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenha cuidado para usar a sintaxe de HTML adequada ao adicionar as tags OG.
