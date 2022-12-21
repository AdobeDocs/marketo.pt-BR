---
unique-page-id: 4720810
description: Remarketing personalizado no Google - Documentos do Marketo - Documentação do produto
title: Remarketing personalizado no Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Remarketing personalizado no Google {#personalized-remarketing-in-google}

O Remarketing personalizado permite reengajamento com seus usuários usando dados RTP e o poder do Google Analytics com o alcance da Google Display Network.

>[!PREREQUISITES]
>
>* Complete o [Redirecionamento com dados de personalização da Web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configuração
>* Revisão [Remarketing com a ajuda do Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) documentação.


## Criação de um público-alvo de remarketing no Google {#creating-a-remarketing-audience-in-google}

1. Faça logon no Google Analytics. Clique em **Administrador**, **Conta**, **Propriedade**. Clique em **Definições de público-alvo** e **Públicos-alvo**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Clique em **+Novo público-alvo**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configuração de link**: Vincule à sua conta do Google AdWords. **Definir público-alvo**: Clique em **Criar novo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. No Construtor de público-alvo, clique em **Sequências** e **Localizar os dados RTP** em Custom Dimension, Custom Variables, Events.

>[!TIP]
>
>Como encontrar os dados da RTP no Analytics para criar seu público-alvo?
>
>No Google Analytics:
>
>* Variáveis personalizadas: Organização, Indústria
>* Categoria do evento: Segmento, Insightera-CTA, RTP-Remarketing
>* Rótulo do evento: Nome do segmento, Nome da campanha, Nome do público-alvo segmentado
>
>No Google Universal Analytics:
>
>* Dimension personalizado: Organização, Setor, Categoria (Fortune 500,1000, Global 2000), Grupo (Empresa, SMB), Lista de ABM (Lista de Contas Nomeadas)
>* Categoria do evento: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Rótulo do evento: Nome do segmento, Nome da campanha, Nome do público-alvo segmentado


**Exemplo de remarketing de público-alvo de dados de público-alvo segmentado RTP**

1. Clique em **Sequências.**
1. Selecionar **Rótulo do evento.**
1. Enter **Nome do público-alvo segmentado** (como aparece na RTP).
1. Clique em **Aplicar**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exemplo de público-alvo dos dados do setor RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Clique em **Sequências**.
1. Selecionar **RTP-Setor**.
1. Enter **Nome da indústria** (por exemplo, Financial Services, Education...).
1. Clique em **Aplicar**.
1. Insira um **Nome do público-alvo**. Clique em **Salvar**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Criar uma campanha publicitária de remarketing no Google AdWords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Faça logon em **Google Adwords**. Clique em **Campanhas**, selecione **Exibir somente rede**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Enter **Nome da campanha**, Selecione **Digite Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Enter **Nome do grupo de anúncios,** enter **CPC aprimorado**, Selecione **Lista de remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Clique em Salvar e continue.
1. Adicione sua Imagem ou Publicidade em texto e inicie sua campanha de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Redirecionamento com dados de personalização da Web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado no Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

