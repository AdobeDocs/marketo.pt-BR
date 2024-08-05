---
unique-page-id: 2950524
description: Implante Social no seu site - Documentos do Marketo - Documentação do produto
title: Implantar Social no seu site
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Implantar Social no seu site {#deploy-social-on-your-website}

Incorpore aplicativos sociais em suas páginas que não são do Marketo.

>[!IMPORTANT]
>
>Em 31 de julho de 2024, começamos o processo de descontinuação desse recurso. Você não poderá criar novas ativos. A ativos continuará a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nem todos os Marketo Engage usuários compraram esse funcionalidade. Entre em contato com a equipe de conta do Adobe Systems (seu gerente de conta) para obter detalhes.

Você pode implantar aplicativos sociais em seu próprio site para envolver seus público-alvo e trazer todos para a conversa maior nas redes sociais. À medida que as pessoas compartilham suas promoções e conteúdo com seus amigos nas redes sociais, você gera mais tráfego no seu site.

1. Selecione um aplicativo social aprovado, como um Vídeo do YouTube ou um Botão Social.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Selecione **Incorporar Code** em ações do Social aplicativo.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copie o código para o cabeçalho (`<head>`) e corpo do página do seu site.`<body>`

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Colar o primeiro snippet de código no cabeçalho de página do seu site.

   ![](assets/socialonsite-embedhead.png)

1. Colar o segundo snippet de código em cada página, em que você deseja que seu aplicativo social apareça no página.

   ![](assets/socialonsite-embedwidget.png)

1. Se for necessário definir o tamanho do aplicativo social para dimensões específicas no página, adicione as **opções outerHeight** e **outerWidth** ao segundo trecho de código. Por exemplo, você pode adicionar `options='{"outerHeight":400, "outerWidth":600}'`, como em:

   ![](assets/socialonsite-resizewidget2.png)

   Seu aplicativo social do Marketo agora adiciona conteúdo e interatividade ao seu site, convidando fãs, visitantes e clientes existentes a espalharem a notícia sobre você. Ao mesmo tempo, ele adiciona seus dados de perfil ao seu banco de dados e rastreia métricas de influência social.

   >[!MORELIKETHIS]
   >
   >* [Botão Personalizar Social aplicativo](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Definir Social requisito de compartilhamento](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publish Páginas de aterrissagem no Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
