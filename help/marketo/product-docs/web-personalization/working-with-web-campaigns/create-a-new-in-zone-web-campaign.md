---
unique-page-id: 4719400
description: Criar uma nova campanha na Web na zona - Documentos do Marketo - Documentação do produto
title: Criar uma nova campanha na Web na zona
exl-id: 5cbe80a2-5e20-4e35-a722-b4cb479b4df7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 1%

---

# Criar uma nova campanha na Web na zona {#create-a-new-in-zone-web-campaign}

Uma campanha da Web é uma reação personalizada associada a um segmento específico e pode ser uma [caixa de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) em seu site, uma substituição de zona in, uma [recurso de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md) ou um alerta por email. Uma campanha da Web em Zona substitui um elemento de seu site baseado na ID da Zona por conteúdo ou banners gráficos.

## Criar uma campanha na Web na Zona {#create-an-in-zone-web-campaign}

1. Ir para **Campanhas da Web**.

   ![](assets/image2016-8-18-15-3a54-3a21.png)

1. Selecionar **Criar Nova Campanha da Web.**

   ![](assets/create-new-web-campaign-hand.png)

1. Selecione o **Na Zona** tipo de campanha. Personalize e adicione uma **ID da zona.** Defina a campanha como **Aderente** e adicione seu anúncio no editor. Adicione o URL da página para visualização e clique em **Visualizar** para ver como a campanha reagirá em seu site.

   ![](assets/new-3-1.png)

   >[!NOTE]
   >
   >**O que é uma ID de zona?**
   >
   >Uma ID de zona é onde você gostaria que sua campanha da Web &quot;Na zona&quot; estivesse localizada no site. Para localizar uma &quot;ID de zona&quot;, basta acessar seu site e selecionar a área que deseja substituir por uma campanha da Web e clicar com o botão direito do mouse. No Chrome, a opção é &quot;Elemento do Inspect&quot;, em outros navegadores pode variar.
   >
   >Em seguida, você deseja encontrar a &quot;id&quot; associada a esta seção do site, que é realçada porque você está inspecionando esse elemento. Por exemplo, se você clicar com o botão direito do mouse no Chrome, o texto destacado exibirá `<div id="featured-slider">` em seguida, &quot;controle deslizante em destaque&quot; é o que você deve digitar na seção &quot;id da zona&quot;. Normalmente, &quot;div id&quot; é usada, mas qualquer ID também pode ser usada, como h1 id, p id, etc.

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
   <td colspan="1" rowspan="1"><p>Insira o nome da id localizada no código do HTML do elemento do site que a campanha substitui.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Fixo
 </strong></p></td> 
   <td colspan="1" rowspan="1">A caixa de seleção Aderente é selecionada por padrão para a campanha Na zona e mantém a campanha Na zona em sua posição de identificação de zona durante toda a sessão do visitante no site. Recomenda-se sempre ter um Na zona definido como Aderente.</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong> Atenuação</strong> </p></td> 
   <td colspan="1" rowspan="1">Marcar a caixa de seleção Usar efeito e Esmaecer fornece um efeito esmaecido para a área de ID da Zona no site. Se In Zone for um banner gráfico, a página primeiro será carregada e a campanha será ativada com um efeito de esmaecimento.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Deslizamento</strong></td> 
   <td colspan="1">Marcar a caixa de seleção Usar efeito e a opção Deslizar fornecem um deslizamento em vigor para a área de ID da Zona no site. Se In Zone for um banner gráfico, a página primeiro será carregada e a campanha será ativada com um efeito deslizante da esquerda para a direita.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Editor de texto formatado  </strong></td> 
   <td colspan="1">O editor de rich text permite a formatação de texto, vinculação e inserção de imagem. <a href="/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md">Leia mais aqui</a> .</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong> Visualizar no site   </strong></td> 
   <td colspan="1">Visualize campanhas antes de serem iniciadas. <br> 
    <ul> 
     <li> URL - Insira um exemplo de URL onde a campanha seria executada para ver um exemplo de visualização de como a campanha seria ao vivo.</li> 
     <li>Dispositivo - Visualize como sua campanha será exibida por dispositivo: Desktop, Retrato Móvel, Paisagem Móvel, Retrato do Tablet, Paisagem Retrato.</li> 
     <li> Visualizar - Clique <strong>Visualizar</strong> para abrir uma nova janela do URL de exemplo e ver como a campanha reage.</li> 
     <li> Compartilhar - Use o botão Compartilhar para enviar um e-mail a um colega com um link para ver a campanha de proxy.</li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Acelere e simplifique o processo de criação de campanha usando nosso [modelos incorporados](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) ou [salvar sua campanha existente](/help/marketo/product-docs/web-personalization/using-templates/using-templates-to-create-web-campaigns.md) como modelo para reutilização.

>[!NOTE]
>
>**Deseja testar a/B suas campanhas da Web?** Uma ou mais campanhas da Web podem ser [Teste A/B para obter os melhores resultados](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/ab-test-your-web-campaign.md). Com o recurso de Ajuste automático, a plataforma reconhece automaticamente as campanhas com melhor desempenho, continua com as campanhas de conversão mais altas e pausa as outras.

## Editar uma campanha da Web {#edit-a-web-campaign}

No **Campanhas da Web** página, clique em **Editar** na Campanha.

![](assets/in-zone-web-campaign-edit.png)

>[!NOTE]
>
>Para facilitar a localização da campanha desejada, use o [recurso de filtro](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md).

## Visualizar uma campanha da Web {#preview-a-web-campaign}

1. Na página Campanhas da Web , clique em **Visualizar** na campanha da web que você deseja visualizar.

   ![](assets/in-zone-web-campaign-preview.png)

## Clonar uma campanha da Web {#clone-a-web-campaign}

Consulte [Clonar uma campanha da Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/clone-a-web-campaign.md).

## Excluir uma campanha da Web {#delete-a-web-campaign}

1. Na página Campanhas da Web , clique em **Excluir** na Campanha que deseja excluir.

   ![](assets/in-zone-web-campaign-delete.png)

1. Uma mensagem de confirmação é exibida para confirmar se você deseja excluir a Campanha.

>[!MORELIKETHIS]
>
>* [Criar uma nova campanha Web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
>* [Criar uma nova campanha Web de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)

