---
unique-page-id: 4720810
description: Remarketing personalizado no Google - Documentação do Marketo - Documentação do produto
title: Remarketing personalizado no Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Remarketing personalizado no Google {#personalized-remarketing-in-google}

O Remarketing personalizado permite que você se envolva novamente com seus usuários usando dados RTP e o poder dos Google Analytics com o alcance da rede de exibição da Google.

>[!PREREQUISITES]
>
>* Conclua o [Redirecionamento com dados de personalização da Web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configuração
>* Revisão [Remarketing com a ajuda do Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) documentação.

## Criação de um público de remarketing no Google {#creating-a-remarketing-audience-in-google}

1. Faça logon nos Google Analytics. Clique em **Admin**, **Conta**, **Propriedade**. Clique em **Definições de público** e **Públicos-alvo**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Clique em **+Novo público-alvo**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configuração do link**: Link para sua conta do Google Adwords. **Definir público-alvo**: Clique **Criar novo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. No Construtor de público-alvo, clique em **Sequências** e **Localizar os dados RTP** em Dimension personalizados, Variáveis personalizadas, Eventos.

>[!TIP]
>
>Como encontrar os dados RTP no Analytics para criar seu público-alvo?
>
>Em Google Analytics:
>
>* Variáveis personalizadas: organização, setor
>* Categoria do evento: Segmento, Insightera-CTA, RTP-Remarketing
>* Rótulo do evento: Nome do segmento, Nome da campanha, Nome do público segmentado
>
>No Google Universal Analytics:
>
>* Dimension personalizados: organização, setor, categoria (Fortune 500,1000, Global 2000), grupo (Enterprise, SMB), lista de ABM (lista de contas nomeadas)
>* Categoria do evento: RTP-Segmento, RTP-Campanha RTP-Remarketing
>* Rótulo do evento: Nome do segmento, Nome da campanha, Nome do público segmentado

**Exemplo de público-alvo de remarketing de dados de público-alvo segmentados RTP**

1. Clique em **Sequências.**
1. Selecionar **Rótulo do evento.**
1. Enter **Nome do público segmentado** (como aparece na RTP).
1. Clique em **Aplicar**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exemplo de público-alvo de dados do setor da RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Clique em **Sequências**.
1. Selecionar **RTP-Setor**.
1. Enter **Nome do setor** (p. ex. Serviços financeiros, educação...).
1. Clique em **Aplicar**.
1. Insira um **Nome do público**. Clique em **Salvar**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Criar uma campanha de anúncio de remarketing no Google AdWords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Fazer logon em **Google Adwords**. Clique em **Campanhas**, selecione **Exibir somente rede**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Enter **Nome da campanha**, Selecionar **Digite Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Enter **Nome do grupo de anúncios,** inserir **CPC aprimorado**, Selecionar **Lista de remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Clique em Salvar e continue.
1. Adicione uma Imagem ou Anúncio de texto e inicie a campanha de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Redirecionamento com dados de personalização da Web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado no Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
