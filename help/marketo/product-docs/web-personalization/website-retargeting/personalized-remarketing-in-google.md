---
unique-page-id: 4720810
description: Remarketing personalizado no Google - Documentação do Marketo - Documentação do produto
title: Remarketing personalizado no Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Remarketing personalizado no Google {#personalized-remarketing-in-google}

O Remarketing personalizado permite que você se envolva novamente com seus usuários usando dados RTP e o poder do Google Analytics com o alcance da rede de exibição da Google.

>[!PREREQUISITES]
>
>* Concluir a configuração de [Redirecionamento com [!DNL Web Personalization] Dados](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Revise a documentação de [Remarketing com a Ajuda do Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645).

## Criação de um público de remarketing no Google {#creating-a-remarketing-audience-in-google}

1. Faça logon no Google Analytics. Clique em **[!UICONTROL Administrador]**, **[!UICONTROL Conta]**, **[!UICONTROL Propriedade]**. Clique em **[!UICONTROL Definições de público-alvo]** e **[!UICONTROL Públicos-alvo]**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Clique em **[!UICONTROL +Novo público-alvo]**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Configuração de Link]**: Link para sua conta [!DNL Google Adwords]. **[!UICONTROL Definir Público]**: Clique Em **[!UICONTROL Criar Novo]**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. No Construtor de público-alvo, clique em **[!UICONTROL Sequências]** e **[!UICONTROL Localize os dados RTP]** em [!UICONTROL Dimensões personalizadas], [!UICONTROL UICONTROL [ !]Variáveis Personalizadas &#x200B;], [!UICONTROL Eventos].

>[!TIP]
>
>Como encontrar os dados RTP no Analytics para criar seu público-alvo?
>
>No Google Analytics:
>
>* Variáveis personalizadas: organização, setor
>* Categoria do evento: Segmento, Insightera-CTA, RTP-Remarketing
>* Rótulo do evento: Nome do segmento, Nome da campanha, Nome do público segmentado
>
>No Google Universal Analytics:
>
>* Dimensões personalizadas: organização, setor, categoria (Fortune 500,1000, Global 2000), grupo (Enterprise, SMB), lista de ABM (lista de contas nomeadas)
>* Categoria do evento: RTP-Segmento, RTP-Campanha RTP-Remarketing
>* Rótulo do evento: Nome do segmento, Nome da campanha, Nome do público segmentado

**Exemplo de público-alvo de remarketing de dados de público-alvo segmentados RTP**

1. Clique em **[!UICONTROL Sequências].**
1. Selecione **[!UICONTROL Rótulo de Evento].**
1. Digite **[!UICONTROL Nome do Público-alvo Segmentado]** (como aparece no RTP).
1. Clique em **[!UICONTROL Aplicar]**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Exemplo de público-alvo de dados da indústria RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Clique em **[!UICONTROL Sequências]**.
1. Selecione **[!UICONTROL RTP-Industry]**.
1. Insira o **Nome do setor** (por exemplo, [!UICONTROL Serviços Financeiros], [!UICONTROL Educação]...).
1. Clique em **[!UICONTROL Aplicar]**.
1. Insira um **[!UICONTROL Nome do público-alvo]**. Clique em **[!UICONTROL Salvar]**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Criar uma campanha de anúncio de remarketing em [!DNL Google Adwords] {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Faça logon em **[!DNL Google Adwords]**. Clique em **[!UICONTROL Campanhas]**, selecione **[!UICONTROL Exibir somente rede]**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Insira O **[!UICONTROL Nome Da Campanha]** E Selecione **[!UICONTROL Digitar Remarketing].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Digite o **[!UICONTROL Nome do Grupo de Anúncios],** digite **[!UICONTROL CPC Aprimorado]**, selecione **[!UICONTROL Lista de Remarketing]**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Clique em **[!UICONTROL Salvar]** e continue.
1. Adicione uma Imagem ou Anúncio de texto e inicie a campanha de remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Redirecionamento com [!DNL Web Personalization] Dados](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizado em [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
