---
unique-page-id: 2950561
description: Script de conversão para eventos personalizados - Documentos do Marketo - Documentação do produto
title: Script de conversão para eventos personalizados
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Script de conversão para eventos personalizados {#conversion-script-for-custom-events}

Você define a meta de realização ao criar uma oferta de referência. Se a ação que conta para a meta for um evento específico em sua própria página da Web, você pode usar um script de conversão para chamar nossa API JavaScript.

## Recuperar o script de conversão {#retrieve-the-conversion-script}

1. No editor de ofertas de referência, clique em **Detalhes da oferta** e depois selecione **Evento JavaScript do cliente** no menu suspenso meta de realização.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie o script superior na caixa cinza e coloque-o em sua página da Web no `<body>` tags. O script inferior é colocado dentro da variável `<header>` tags.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Lembre-se de copiar e colar ambos os scripts se eles estiverem em um site que não seja da Marketo.

## Recuperar o script do carregador {#retrieve-the-loader-script}

1. Selecione a oferta de referência da árvore e clique em **Ações de oferta de referência** e **Código incorporado**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Clique com o botão direito do mouse no **Código do cabeçalho** e insira-o no cabeçalho da página da Web. Em seguida, faça o mesmo para o **Código do corpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Colar os scripts na sua página da Web {#pasting-the-scripts-onto-your-webpage}

Cole os scripts de conversão no HTML para o corpo e o cabeçalho. Em seguida, coloque os scripts de carregamento no HTML do corpo e do cabeçalho.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conexão do script de conversão {#connecting-the-conversion-script}

Aqui é onde você escreverá uma função JavaScript que usa o HTML específico de qualquer elemento de página em que deseja acionar a conclusão da meta. Por exemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

Neste exemplo, há um botão na página da Web com uma ID de &quot;#myButtonId&quot;. Ao clicar nesse botão, a pessoa será registrada como tendo concluído a meta.

Ótimo! Seu site agora está capturando metas personalizadas de promoção social com o Marketo.

>[!MORELIKETHIS]
>
>* [Especificar meta para oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Criar uma oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implantar o Social em seu site](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

