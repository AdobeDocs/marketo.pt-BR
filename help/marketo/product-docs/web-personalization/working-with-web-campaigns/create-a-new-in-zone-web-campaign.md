---
unique-page-id: 4719400
description: Criar uma nova Campanha na Web da Zona - Documentos do Marketing - Documentação do produto
title: Criar uma nova Campanha da Web na zona
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---


# Criar uma nova Campanha da Web na Zona {#create-a-new-in-zone-web-campaign}

Uma campanha da Web é uma reação personalizada associada a um segmento específico e pode ser uma [caixa de diálogo](create-a-new-dialog-web-campaign.md) em seu site, uma substituição de zona interna, um [recurso de widget](create-a-new-widget-web-campaign.md) ou um alerta de email. Uma campanha da Web In Zone substitui um elemento do seu site com base na ID da Zona pelo conteúdo ou banners gráficos.

## Criar uma Campanha da Web In Zone {#create-an-in-zone-web-campaign}

1. Vá para **Campanha**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Selecione **Criar Nova Campanha Web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Selecione o tipo de campanha **Na Zona**. Personalize e adicione uma **ID de zona.** Defina a campanha como  **** Stickyy e adicione seu anúncio no editor. Adicione o URL da página à pré-visualização e clique em **Pré-visualização** para ver como a campanha reagirá ao site.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >
   >**O que é uma ID de zona?**
   >
   >
   >Uma ID de zona é onde você deseja que sua campanha &quot;Na zona&quot; esteja localizada no site. Para localizar uma &quot;ID de zona&quot;, vá para o seu site e selecione a área que deseja substituir por uma campanha da Web e clique com o botão direito do mouse. No Chrome, a opção é &quot;Elemento Inspect&quot;, em outros navegadores ela pode variar.
   >
   >
   >Em seguida, você deseja encontrar a &quot;id&quot; associada a esta seção do site, que é realçada porque você está inspecionando esse elemento. Por exemplo, se você clicar com o botão direito do mouse no Chrome o texto realçado indicar `<div id="featured-slider">`, então &quot;controle deslizante em destaque&quot; é o que você deve digitar na seção &quot;ID da zona&quot;. Normalmente, &quot;div id&quot; é usado, mas qualquer ID também pode ser usada, como h1 id, p id etc.

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nome</th> 
   <th colspan="1" rowspan="1">Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong> ID da zona </strong></td> 
   <td colspan="1" rowspan="1"><p>Insira o nome da ID encontrada no código HTML do elemento do site que a campanha substitui.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Aderente </strong></p></td> 
   <td colspan="1" rowspan="1">A caixa de seleção Aderente é selecionada por padrão para a campanha da zona interna e mantém a campanha da zona em sua posição de ID da zona durante toda a sessão do visitante no site. É recomendável ter sempre um In Zone definido como Sticky.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Desaparecimento</strong> </p></td> 
   <td colspan="1" rowspan="1">Marcar a caixa de seleção Usar efeito e Esmaecer fornece um efeito de esmaecimento para a área de ID da Zona no site. Se a Zona de entrada for um banner gráfico, a página primeiro será carregada e, em seguida, a campanha será ativada com um efeito de sombreamento.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Deslizamento</strong></td> 
   <td colspan="1">Marcar a caixa de seleção Usar efeito e a opção Deslizar fornecem um deslocamento para a área de ID da Zona no site. Se a Zona de entrada for um banner gráfico, a página primeiro será carregada e, em seguida, a campanha será ativada com um efeito deslizante da esquerda para a direita.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editor de Rich Text  </strong></td> 
   <td colspan="1">O editor de Rich Text permite a formatação de texto, vinculação e inserção de imagem. <a href="using-the-web-personalization-rich-text-editor.md">Leia mais aqui</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Pré-visualização no local   </strong></td> 
   <td colspan="1">Campanhas de pré-visualização antes de serem iniciadas. <br> 
    <ul> 
     <li> URL - Insira um URL de exemplo onde a campanha seria executada para ver um exemplo pré-visualização de como a campanha seria exibida.</li> 
     <li>Dispositivo - Pré-visualização como sua campanha será exibida por dispositivo: Desktop, Retrato Móvel, Paisagem Móvel, Retrato Tablet, Paisagem Retrato.</li> 
     <li> Pré-visualização - Clique em <strong>Pré-visualização</strong> para abrir uma nova janela do URL de exemplo para ver como a campanha reage.</li> 
     <li> Compartilhar - Use o botão Compartilhar para enviar um email para um colega com um link para ver a campanha proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Acelere e simplifique seu processo de criação de campanhas usando nossos [modelos incorporados](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) ou [salvando sua campanha existente](../../../product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) como modelo para reutilização.

>[!NOTE]
>
>**Deseja testar a A/B suas campanhas da Web?** Uma ou mais campanhas da Web podem ser  [A/B testadas para obter resultados](ab-test-your-web-campaign.md) ideais. Com o recurso Ajuste automático, a plataforma reconhece automaticamente as campanhas de melhor desempenho, continua com as campanhas de conversão mais altas e pausa as outras.

## Editar uma Campanha da Web {#edit-a-web-campaign}

Na página **Campanha**, clique em **Editar** na Campanha.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Para facilitar a localização da campanha desejada, use o recurso [filter](filter-web-campaigns.md).

## Pré-visualização de uma Campanha da Web {#preview-a-web-campaign}

1. Na página Campanhas da Web, clique em **Pré-visualização **na campanha da Web que deseja visualização.

   ![](assets/in-zone-web-campaign-preview.png)

## Clonar uma Campanha da Web {#clone-a-web-campaign}

Consulte [Clonar uma Campanha da Web](clone-a-web-campaign.md).

## Excluir uma Campanha da Web {#delete-a-web-campaign}

1. Na página Campanhas da Web, clique em **Excluir **na Campanha que deseja excluir.

   ![](assets/in-zone-web-campaign-delete.png)

1. Uma mensagem de confirmação é exibida para confirmar se você deseja excluir a Campanha.

>[!MORELIKETHIS]
>
>* [Criar uma nova Campanha Web de widget](create-a-new-widget-web-campaign.md)
>* [Criar uma nova Campanha da Web de caixa de diálogo](create-a-new-dialog-web-campaign.md)

