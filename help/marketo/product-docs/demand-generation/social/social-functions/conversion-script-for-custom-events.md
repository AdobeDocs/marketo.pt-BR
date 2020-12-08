---
unique-page-id: 2950561
description: Script de conversão para Eventos personalizados - Documentos de marketing - Documentação do produto
title: Script de conversão para Eventos personalizados
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Script de conversão para Eventos personalizados {#conversion-script-for-custom-events}

Você define a meta de realização ao criar uma oferta de referência. Se a ação que conta para a meta for um evento específico em sua própria página da Web, você pode usar um script de conversão para chamar nossa API JavaScript.

## Recuperar o script de conversão {#retrieve-the-conversion-script}

1. No editor de oferta de referência, clique em Detalhes **da** Oferta e selecione Evento **JavaScript do** cliente no menu suspenso de meta de realização.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie o script superior na caixa cinza e coloque-o em sua página da Web dentro das `<body>` tags. O script inferior é colocado dentro das `<header>` tags.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Lembre-se de copiar e colar ambos os scripts se eles estiverem em um site que não seja de marketing.

## Recuperar o script do loader {#retrieve-the-loader-script}

1. Selecione a oferta de referência na árvore e clique em Ações **de Oferta de** referência e **Incorporar código**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Clique com o botão direito do mouse no Código **do** cabeçalho e insira-o no cabeçalho da página da Web. Em seguida, faça o mesmo com o Código **do** Corpo.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Colar os scripts na sua página da Web {#pasting-the-scripts-onto-your-webpage}

Cole os scripts de conversão no HTML para o corpo e cabeçalho. Em seguida, coloque os scripts loader no HTML para o corpo e o cabeçalho.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conexão do script de conversão {#connecting-the-conversion-script}

Aqui é onde você escreverá uma função JavaScript que usa a ID HTML específica de qualquer elemento de página no qual você deseja acionar a conclusão da meta. Por exemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

Neste exemplo, há um botão na página da Web com uma ID de &quot;#myButtonId&quot;. Quando esse botão for clicado, a pessoa será registrada como tendo completado a meta.

Incrível! Seu site agora está capturando metas personalizadas de promoção social com o Marketo.

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Especificar meta para a Oferta de referência](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Criar uma Oferta de referência](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implantar o Social em seu site](deploy-social-on-your-website.md)

