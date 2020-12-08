---
unique-page-id: 10092925
description: Pré-visualização e teste uma Campanha da Web - Documentos do Marketing - Documentação do produto
title: Pré-visualização e teste uma Campanha da Web
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Pré-visualização e teste uma Campanha da Web {#preview-and-test-a-web-campaign}

Este artigo mostra diferentes maneiras de pré-visualização de uma campanha da Web e também como testá-la usando um segmento de caixa de proteção ao vivo em seu site.

## Pré-visualização de uma Campanha da Web na página de criação {#preview-a-web-campaign-on-the-creation-page}

1. Vá para **Web** **Campanha**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Clique em** Criar nova Campanha da Web**** ** ou no ícone para editar uma campanha existente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Na Pré-visualização do site, adicione o URL da página e clique em **Pré-visualização**. Uma nova janela/guia é aberta mostrando a pré-visualização da campanha.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Clique em **Compartilhar** para abrir um email com um URL fixo da pré-visualização da campanha.

   >[!NOTE]
   >
   >Você também tem a opção de instalar um plug-in do navegador ( [Chrome](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) ou [Firefox](http://docs.marketo.com/display/docs/assets/mwp-0.0.0.8.xpi)) para obter a melhor experiência em visualizar sua campanha. Consulte a seção abaixo.

## Pré-visualização de uma Campanha da Web na página de criação usando o plug-in do navegador {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Siga as etapas 1 e 2 do `section above`.
1. Clique no link para o plug-in do navegador (neste caso, estamos usando o Chrome).

   ![](assets/4-1.png)

1. Uma nova janela/guia é aberta. Clique em **Adicionar ao Chrome**.

   ![](assets/five.png)

1. Clique em **Adicionar extensão**.

   ![](assets/six.png)

1. Volte para Marketo. Adicione o URL da página e clique em **Pré-visualização**.

   ![](assets/seven.png)

1. Uma nova janela/guia é aberta, permitindo que você pré-visualização a aparência da sua campanha em um desktop, telefone ou tablet.

   ![](assets/campaign-preview.png)

## Pré-visualização de uma Campanha da Web na página do Web Campanha {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Ao olhar para a lista de suas campanhas da Web, basta escolher uma campanha e clicar no ícone de **Pré-visualização** .

   ![](assets/web-campaigns-1-preview-hand.png)

   Calma!

## Pré-visualização de uma Campanha da Web em seu site {#preview-a-web-campaign-on-your-website}

Crie um segmento e uma campanha de sandbox.

1. Ir para **Segmentos**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Clique em **Criar novo**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Nomeie o segmento.
1. Em Comportamento, arraste Incluir páginas até a tela. Adicione o valor *sandbox=1*. Clique em Salvar e definir Campanha.

   ![](assets/segment.png)

1. Na página Definir Campanha da Web, altere o segmento do Público alvo para o segmento da caixa de proteção selecionando-o na lista.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Conclua o anúncio da campanha e clique em **Iniciar**.\
   ![](assets/click-launch.jpg)

1. Vá para seu site, adicione o parâmetro de URL &quot;?sandbox=1&quot; no final do URL. Exemplo: [www.marketo.com?sandbox=1](http://www.marketo.com/?sandbox=1)
1. Veja a campanha reagir em seu site.

>[!NOTE]
>
>O Campanha reage somente uma vez durante uma sessão de visitante. Para ver a campanha novamente, limpe os cookies do navegador.

>[!NOTE]
>
>Campanhas de redirecionamento não podem ser visualizadas. A única maneira de testá-los é usando um segmento de caixa de proteção (que público alvo por páginas específicas - *sandbox=redirect* )

