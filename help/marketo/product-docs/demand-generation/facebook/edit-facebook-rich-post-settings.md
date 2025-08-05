---
unique-page-id: 2950555
description: Editar configurações de publicação avançada do Facebook - Documentação do Marketo - Documentação do produto
title: Editar configurações de publicação avançada do Facebook
exl-id: f72bfb03-9bc7-46c4-bfb8-b377b2d23fc9
hide: true
hidefromtoc: true
feature: Integrations
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Editar configurações de publicação avançada [!DNL Facebook] {#edit-facebook-rich-post-settings}

Personalize postagens quando as pessoas compartilharem com você no [!DNL Facebook].

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

Os _aplicativos sociais_ do Marketo permitem que seus clientes potenciais compartilhem suas páginas de aterrissagem com suas conexões em redes sociais, como Facebook, Twitter etc. As tags do Facebook OpenGraph (tags OG) permitem especificar quais informações da página de aterrissagem são incluídas em publicações do Facebook.

## Selecionar opções de publicação avançadas {#select-rich-post-options}

Você pode especificar os tipos de informações de página a serem usadas nas postagens avançadas do [!DNL Facebook] geradas por compartilhamentos da sua página de aterrissagem.

1. Selecione **[!UICONTROL Mensagem do Facebook]** no editor do vídeo ou do botão de redes sociais __[!DNL YouTube_]_.

   ![](assets/image2014-9-22-16-3a47-3a21.png)

1. Selecione entre as opções a seguir para a mensagem [!DNL Facebook].

   * Adicionar conteúdo estático: selecione essa opção para inserir o título, a legenda e a descrição manualmente.

   ![](assets/image2014-9-22-16-3a48-3a0.png)

   * Adicionar conteúdo dinâmico: seu aplicativo social pode usar as marcas `<TITLE>`, `<CAPTION>` e `<DESCRIPTION>` da página de aterrissagem para preencher sua publicação avançada.

   ![](assets/image2014-9-22-16-3a48-3a9.png)

   >[!NOTE]
   >
   >Eles já devem existir na origem da página, mas, para obter mais controle, é possível adicionar marcas OG [!DNL Facebook] específicas à página de aterrissagem.

   * Não adicionar conteúdo avançado: limita as postagens de [!DNL Facebook] da sua página de aterrissagem somente à mensagem e ao link principais.

   ![](assets/image2014-9-22-16-3a48-3a18.png)

## Adicionar [!DNL Facebook] marcas OG a uma página de aterrissagem {#add-facebook-og-tags-to-a-landing-page}

Para controlar os elementos de página que serão incluídos nos compartilhamentos [!DNL Facebook] da página de aterrissagem, você pode adicionar [!DNL Facebook] marcas OG (Open Graph) para título, legenda e descrição à página de aterrissagem.

1. Abra a página de aterrissagem que contém seu **[!DNL YouTube]vídeo** ou botão de rede social.

   ![](assets/image2014-9-22-16-3a51-3a28.png)

   A **[!UICONTROL Designer da Página de Aterrissagem]** abre em uma nova janela.

1. Selecione **[!UICONTROL Ações Da Página De Aterrissagem]** > **[!UICONTROL Editar Metatags De Página]**.

   ![](assets/image2014-9-22-16-3a51-3a36.png)

1. Adicione a HTML que define log:title, og:caption e og:description. Copie e cole essas linhas e substitua o texto do espaço reservado:

   `<meta property="og:title" content="My Post Title"/>`

   `<meta property="og:caption" content="My Post Caption"/>`

   `<meta property="og:description" content="This text appears in the post description"/>`

   ![](assets/image2014-9-22-16-3a52-3a8.png)

>[!NOTE]
>
>Tenha cuidado para usar a sintaxe apropriada do HTML ao adicionar as tags OG.
