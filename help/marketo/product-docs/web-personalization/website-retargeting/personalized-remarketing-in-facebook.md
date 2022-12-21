---
unique-page-id: 4720917
description: Remarketing personalizado no Facebook - Documentos do Marketo - Documentação do produto
title: Remarketing personalizado no Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 6%

---

# Remarketing personalizado no Facebook {#personalized-remarketing-in-facebook}

O Remarketing personalizado permite reengajamento com seus usuários usando dados RTP e o poder do Remarketing da Facebook.

>[!PREREQUISITES]
>
>* Complete o [Redirecionamento com dados de personalização da Web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configuração
>* Revise o [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Documentação do facebook sobre públicos-alvo personalizados](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) e Remarketing.


## Criação de um público-alvo no Facebook {#creating-an-audience-in-facebook}

1. No Facebook, acesse seu [Guia Público](https://www.facebook.com/ads/audience_manager) no Gerenciador de anúncios.

1. Clique em **Ferramentas** e selecione **Públicos-alvo**.

   ![](assets/one-1.png)

1. Clique em **Criar um público-alvo personalizado**.

   ![](assets/two-1.png)

1. Selecionar **Tráfego do site**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Na lista de tráfego do site, selecione **Combinação personalizada**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Na lista Incluir, selecione **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Na lista Evento , selecione **Remarketing RTP** e selecione um parâmetro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Para este exemplo, selecione Setor para conter **Educação**. Enter **Educação** e editar **No último** para ser 180 dias. Insira o nome do público-alvo: **Setor da Educação**. Clique em **Criar público-alvo**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Agora você criou um novo público-alvo personalizado usando dados RTP no Facebook.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## Pontos de dados RTP no Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Nome do evento</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>Remarketing RTP</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parâmetro</th> 
        <th>Valor</th> 
       </tr> 
       <tr> 
        <td>Lista ABM</td> 
        <td>(Nome da lista baseada em conta)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Categoria</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Agrupar</td> 
        <td colspan="1"><p>Empresarial</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Setor</td> 
        <td><p>Defesa</p><p>Educação</p><p>Serviços financeiros</p><p>Governo</p><p>Saúde, Pharma, Biotech</p><p>Software e Internet</p><p>etc... (de acordo com as opções do setor RTP)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Público segmentado</td> 
        <td colspan="1">(Nome do público-alvo segmentado criado na RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Direcione seu público-alvo com um anúncio {#target-your-audience-with-an-ad}

Para obter mais detalhes, consulte [Documentação do facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vá para o Gerenciador de anúncios e clique em **Criar anúncio**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Selecionar **Enviar pessoas para o seu site** como o objetivo de sua campanha.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Insira o URL do site.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Crie seu conjunto de anúncios. Selecione um público-alvo personalizado na lista de Públicos-alvo que você criou, por exemplo, Setor de Educação.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Selecione todas as outras opções de conjunto de anúncios, defina o orçamento e defina os anúncios.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Agora, todos os usuários estão configurados com uma campanha de remarketing personalizada no Facebook.

>[!MORELIKETHIS]
>
>* [Redirecionamento com dados de personalização da Web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado no Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

