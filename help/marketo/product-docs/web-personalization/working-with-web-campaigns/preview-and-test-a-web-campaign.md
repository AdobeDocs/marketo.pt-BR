---
unique-page-id: 10092925
description: Pré-visualizar e testar uma campanha da Web - Documentação do Marketo - Documentação do produto
title: Pré-visualizar e testar uma campanha da web
exl-id: 6cc4ebd8-0d39-4a7d-bc3d-e8cd18157470
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 4%

---

# Pré-visualizar e testar uma campanha da web {#preview-and-test-a-web-campaign}

Este artigo mostra maneiras diferentes de visualizar uma campanha da Web e também como testá-la usando um segmento de sandbox em tempo real no seu site.

>[!NOTE]
>
>A visualização mostra apenas como a campanha será exibida no site escolhido. Links e widgets não funcionarão a fim de evitar cliques/exibições incorretos na análise.

## Pré-visualizar uma campanha da Web na página de criação {#preview-a-web-campaign-on-the-creation-page}

1. Vá para **[!UICONTROL Campanhas da Web]**.

   ![](assets/image2016-8-18-15-3a59-3a35.png)

1. Clique em **[!UICONTROL Criar nova campanha da Web]** ou no ícone para editar uma campanha existente.

   ![](assets/create-new-or-edit-web-campaign.png)

1. Em Visualizar no site, adicione a URL da página e clique em **[!UICONTROL Visualizar]**. Uma nova janela/guia é aberta mostrando a pré-visualização da campanha.

   ![](assets/three-1.png)

   >[!TIP]
   >
   >Clique em **[!UICONTROL Compartilhar]** para abrir um email com uma URL fixa da pré-visualização da campanha.

   >[!NOTE]
   >
   >Você também tem a opção de instalar um plug-in de navegador ([[!DNL Chrome]](https://chrome.google.com/webstore/detail/marketo-web-personalizati/ldiddonjplchallbngbccbfdfeldohkj) ou [[!DNL Firefox]](https://rtp-static.marketo.com/rtp/libs/mwp-0.0.0.8.xpi)) para obter a melhor experiência de visualização da sua campanha. Consulte a seção abaixo.

## Visualizar uma campanha da Web na página de criação usando o plug-in do navegador {#preview-a-web-campaign-on-the-creation-page-using-the-browser-plug-in}

1. Siga as etapas 1 e 2 da seção acima.

1. Clique no link para o plug-in do navegador (neste caso, estamos usando [!DNL Chrome]).

   ![](assets/4-1.png)

1. Uma nova janela/guia é aberta. Clique em **[!UICONTROL Adicionar ao Chrome]**.

   ![](assets/five.png)

1. Clique em **[!UICONTROL Adicionar extensão]**.

   ![](assets/six.png)

1. Volte para o Marketo. Adicione a URL da página e clique em **[!UICONTROL Visualizar]**.

   ![](assets/seven.png)

1. Uma nova janela/guia é aberta e permite pré-visualizar como sua campanha fica em um desktop, telefone ou tablet.

   ![](assets/campaign-preview.png)

## Pré-visualizar uma campanha da Web na página de campanhas da Web {#preview-a-web-campaign-on-the-web-campaigns-page}

1. Ao consultar a lista de suas campanhas da Web, basta escolher uma campanha e clicar no ícone **[!UICONTROL Visualizar]**.

   ![](assets/web-campaigns-1-preview-hand.png)

   Calma!

## Pré-visualizar uma campanha da Web no seu site {#preview-a-web-campaign-on-your-website}

Crie um segmento e uma campanha de sandbox.

1. Vá para **[!UICONTROL Segmentos]**.

   ![](assets/new-dropdown-segments-hand.jpg)

1. Clique em **[!UICONTROL Criar novo]**.

   ![](assets/image2015-9-10-10-3a42-3a39.png)

1. Nomeie o segmento.

1. Em [!UICONTROL Comportamento], arraste [!UICONTROL Incluir páginas] para a tela. Adicione o valor &#42;sandbox=1&#42;. Clique em **[!UICONTROL Salvar e definir a campanha]**.

   ![](assets/segment.png)

1. Na página Definir campanha da Web, altere o Segmento do Target para o segmento da sandbox, selecionando-o na lista.

   ![](assets/set-web-campaign-target-segment.jpg)

1. Conclua o criativo da campanha e clique em **[!UICONTROL Iniciar]**.

   ![](assets/click-launch.jpg)

1. Acesse seu site, adicione o parâmetro de URL &quot;?sandbox=1&quot; ao final do URL. Exemplo: `www.marketo.com?sandbox=1`.

1. Veja o resultado da campanha no seu site.

>[!NOTE]
>
>As campanhas reagem apenas uma vez durante uma sessão de visitante. Para ver a campanha novamente, limpe os cookies do navegador.

>[!NOTE]
>
>As campanhas de redirecionamento não podem ser visualizadas. A única maneira de testá-los é usando um segmento de sandbox (que é direcionado por páginas específicas - &#42;sandbox=redirect&#42;)
