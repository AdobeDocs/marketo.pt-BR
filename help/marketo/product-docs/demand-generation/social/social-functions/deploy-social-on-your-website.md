---
unique-page-id: 2950524
description: Implante o Social em seu site - Documentação do Marketo - Documentação do produto
title: Implantar o Social no seu site
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Implantar o Social no seu site {#deploy-social-on-your-website}

Incorpore aplicativos sociais em suas páginas que não sejam do Marketo.

>[!IMPORTANT]
>
>Em 31 de julho de 2024, iniciamos o processo de desativação desse recurso. Não é mais possível criar novos ativos. Os ativos existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

Você pode implantar aplicativos sociais em seu próprio site para engajar seu público e trazer todos para uma conversa maior nas redes sociais. À medida que as pessoas compartilham suas promoções e conteúdo com os amigos nas redes sociais, você gera mais tráfego no site.

1. Selecione um aplicativo social aprovado, como um Vídeo do YouTube ou o Botão Social.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Selecione **Incorporar código** em Ações do aplicativo social.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copie o código do cabeçalho (`<head>`) e do corpo da página do site (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Cole o primeiro trecho de código no cabeçalho da página do site.

   ![](assets/socialonsite-embedhead.png)

1. Cole o segundo trecho de código em cada página, onde você deseja que o aplicativo social apareça na página.

   ![](assets/socialonsite-embedwidget.png)

1. Se você precisar definir o tamanho do aplicativo social para dimensões específicas na sua página, adicione as opções **outerHeight** e **outerWidth** ao segundo trecho de código. Por exemplo, você pode adicionar `options='{"outerHeight":400, "outerWidth":600}'`, como em:

   ![](assets/socialonsite-resizewidget2.png)

   Seu aplicativo social do Marketo agora adiciona conteúdo e interatividade ao seu site, convidando fãs, visitantes e clientes existentes para espalhar a notícia sobre você. Ao mesmo tempo, adiciona os dados do perfil ao banco de dados e rastreia as métricas de influência social.

   >[!MORELIKETHIS]
   >
   >* [Botão Personalizar Aplicativo Social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Definir Requisito de Compartilhamento Social](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Páginas de aterrissagem do Publish para o Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
