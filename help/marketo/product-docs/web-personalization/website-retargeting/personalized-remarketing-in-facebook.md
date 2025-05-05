---
unique-page-id: 4720917
description: Remarketing personalizado no Facebook - Documentação do Marketo - Documentação do produto
title: Remarketing personalizado no Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 8%

---

# Remarketing personalizado no Facebook {#personalized-remarketing-in-facebook}

O Remarketing personalizado permite que você se envolva novamente com seus usuários usando dados RTP e o poder do Remarketing do Facebook.

>[!PREREQUISITES]
>
>* Concluir a configuração de [Redirecionamento com Dados do Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Revise a documentação do [&#128279;](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook sobre Públicos-alvo personalizados](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) e Remarketing.

## Criação de um público-alvo no Facebook {#creating-an-audience-in-facebook}

1. No Facebook, acesse sua [guia Público-alvo](https://www.facebook.com/ads/audience_manager) do Ads Manager.

1. Clique em **Ferramentas** e selecione **Públicos**.

   ![](assets/one-1.png)

1. Clique em **Criar um público-alvo personalizado**.

   ![](assets/two-1.png)

1. Selecione **Tráfego de Site**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Na lista de tráfego do site, selecione **Combinação Personalizada**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Na lista Incluir, selecione **Evento**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Na lista Evento, selecione **RTP Remarketing** e selecione um parâmetro.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Neste exemplo, selecione o Setor para conter **Educação**. Insira **Educação** e edite **Nos Últimos** para ter 180 dias. Insira O Nome Do Público: **Setor De Educação**. Clique em **Criar Público**.

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
        <td colspan="1">Grupo</td> 
        <td colspan="1"><p>Empresarial</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Setor</td> 
        <td><p>Defesa</p><p>Educação</p><p>Serviços financeiros</p><p>Governo</p><p>Saúde, Farmácia, Biotecnologia</p><p>Software e Internet</p><p>etc... (de acordo com as opções do RTP Industry)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Público segmentado</td> 
        <td colspan="1">(Nome do público-alvo segmentado criado no RTP)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Direcione seu público com um anúncio {#target-your-audience-with-an-ad}

Para obter detalhes adicionais, consulte [a documentação da Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Vá para o Gerenciador de Anúncios, clique em **Criar Anúncio**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Selecione **Enviar pessoas para o seu site** como objetivo da campanha.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Insira o URL do site.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Crie seu conjunto de anúncios. Selecione um público-alvo personalizado na lista de públicos-alvo criada, por exemplo, Setor de educação.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Selecione todas as outras opções de conjunto de anúncios, defina seu orçamento e seus anúncios criativos.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Agora você tem uma campanha de remarketing personalizada no Facebook.

>[!MORELIKETHIS]
>
>* [Redirecionamento com dados do Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado no Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
