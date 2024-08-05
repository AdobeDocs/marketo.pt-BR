---
unique-page-id: 2950561
description: Script de conversão para eventos personalizados - Documentação do Marketo - Documentação do produto
title: Script de conversão para eventos personalizados
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# Script de conversão para eventos personalizados {#conversion-script-for-custom-events}

Você define a meta de preenchimento ao criar uma oferta de referência. Se a ação que conta para a meta for um evento específico em sua própria página da Web, você poderá usar um script de conversão para chamar nossa API do JavaScript.

>[!IMPORTANT]
>
>Em 31 de julho de 2024, iniciamos o processo de desativação desse recurso. Não é mais possível criar novos ativos. Os ativos existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

## Recuperar o script de conversão {#retrieve-the-conversion-script}

1. No editor de oferta de referência, clique em **Detalhes da oferta** e selecione **Evento do JavaScript para cliente** na lista suspensa de meta de preenchimento.

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. Copie o script superior na caixa cinza e coloque-o em sua página da Web nas marcas `<body>`. O script inferior é colocado dentro das marcas `<header>`.

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Lembre-se de copiar e colar ambos os scripts se eles estiverem em um site que não seja da Marketo.

## Recuperar o script de carregamento {#retrieve-the-loader-script}

1. Selecione a oferta de referência da árvore e clique em **Ações da Oferta de Referência** e **Incorporar Código**.

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. Clique com o botão direito do mouse no **Código do cabeçalho** e insira-o no cabeçalho da sua página da Web. Em seguida, faça o mesmo para o **Código do corpo**.

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Colar os scripts na sua página da Web {#pasting-the-scripts-onto-your-webpage}

Cole os scripts de conversão no HTML para o corpo e o cabeçalho. Em seguida, coloque os scripts de carregamento no HTML do corpo e cabeçalho.

![](assets/image2015-4-20-21-3a0-3a16.png)

## Conectar o script de conversão {#connecting-the-conversion-script}

Aqui você escreverá uma função JavaScript que usa a ID de HTML específica de qualquer elemento de página que você deseja acionar a conclusão da meta. Por exemplo:

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

Neste exemplo, há um botão na página da Web com uma ID de &quot;#myButtonId&quot;. Quando esse botão for clicado, a pessoa será registrada como tendo concluído a meta.

Fantástico! Seu site agora está capturando metas personalizadas de promoção social com o Marketo.

>[!MORELIKETHIS]
>
>* [Especificar Meta para Oferta de Indicação](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [Criar uma Oferta de Indicação](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Implantar o Social no seu site](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)
