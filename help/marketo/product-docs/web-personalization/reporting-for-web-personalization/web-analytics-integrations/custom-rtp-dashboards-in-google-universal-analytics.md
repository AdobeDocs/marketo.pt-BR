---
unique-page-id: 7504238
description: Painéis RTP personalizados no Google Universal Analytics - Documentos do Marketo - Documentação do produto
title: Painéis RTP personalizados no Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Painéis RTP personalizados no Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP ao Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Esta publicação explica como configurar painéis RTP no Google Universal Analytics (GUA). Os dados enviados de RTP para GUA podem ser configurados como dois painéis personalizados separados chamados de:

* RTP B2B
* Envolvimento RTP

## Configurar um painel personalizado {#setting-up-a-custom-dashboard}

1. Faça logon no Google Analytics. Clique em **Relatório** no menu superior. Clique em **Painéis** e **+Novo painel personalizado**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Selecionar **Tela em branco**, adicione um **Nome do painel** e clique em **Criar painel**.

1. Clique em **Adicionar Widget** para criar um novo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Painel B2B RTP {#rtp-b-b-dashboard}

Esse painel permite que os usuários analisem o desempenho de seus sites de uma perspectiva B2B.

Ele fornece informações como origem da visita e comportamento no site por setor, receita, tamanho, listas baseadas em conta e segmentos do target.

O painel consiste em 3 colunas

* Fonte de tráfego
* Segmentação
* Detalhamento de firmware

1. Criar um novo painel chamado **Painel B2B RTP** e defina os seguintes widgets:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Coluna 1 - Fontes de tráfego
    </div></th> 
   <th> 
    <div> <strong>Coluna 2 - Segmentação</strong> 
    </div></th> 
   <th> 
    <div> <strong>Coluna 3 - Detalhamento do firmware</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: Sessões por segmentos e canais</li> 
     <li>Tipo de widget: Barra<br></li> 
     <li>Crie um gráfico de barras mostrando: Sessão</li> 
     <li>Agrupado por: Rótulo do evento</li> 
     <li>Pivô por: Agrupamento de canal padrão</li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Nº de usuários segmentados RTP</li> 
     <li>Tipo: Métrica 2.1</li> 
     <li>Mostrar a seguinte métrica: Usuários<br></li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Sessões por setor</li> 
     <li>Tipo: Pizza<br></li> 
     <li>Crie um gráfico de pizza mostrando: Sessões</li> 
     <li>Agrupado por: RTP-Setor</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por setor e canais</strong></li> 
     <li><strong>Tipo de widget: Barra</strong></li> 
     <li><strong>Crie um gráfico de barras mostrando: Sessão</strong></li> 
     <li><strong>Agrupado por: RTP-Setor</strong></li> 
     <li><strong>Pivô por: Agrupamento de canal padrão</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões segmentadas por país</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Gráfico da métrica selecionada: País | Sessões</strong></li> 
     <li><strong>Selecione uma região: O mundo</strong></li> 
     <li><strong>Filtro: Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por Categoria RTP</strong></li> 
     <li><strong>Tipo: Pizza</strong></li> 
     <li><strong>Crie um gráfico de pizza mostrando: Sessões</strong></li> 
     <li><strong>Agrupado por: RTP-Categoria</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Principais segmentos do Target</li> 
     <li>Tipo: Barra</li> 
     <li>Crie um gráfico de barras mostrando: Usuários</li> 
     <li>Agrupado por: Ação do evento</li> 
     <li>Filtro: Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: Sessões por grupos de RTP</li> 
     <li>Tipo: Barra<br></li> 
     <li>Crie um gráfico de barras mostrando: Sessões</li> 
     <li>Agrupado por: Grupo RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Sessões e metas por principais segmentos</li> 
     <li>Tipo: Tabela<br></li> 
     <li>Exiba as seguintes colunas: <br>Rótulo do evento | Sessões | Taxa de conversão do objetivo</li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Painel de envolvimento RTP {#rtp-engagement-dashboard}

Esse painel permite que os usuários analisem o desempenho da campanha RTP e os envolvimentos do mecanismo de recomendação. Ele fornece a comparação da média. duração da sessão e páginas por sessão entre:

* Não Envolvido
* Envolvido (impressões e cliques em uma campanha personalizada)
* Cliques no Mecanismo de recomendação e no conteúdo recomendado principal

Criar um novo painel chamado **Painel de envolvimento RTP** e defina os seguintes widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Exposição de Campanhas da Coluna 1</strong> 
    </div></th> 
   <th> 
    <div> <strong>Click-through das campanhas da coluna 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Mecanismo de recomendação da coluna 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA total (envolvimento)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de eventos</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do Evento (contém): RTP-Campaigns</strong><br><strong>[show] Ação do evento (correspondência exata): Impressão</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CTA total (Click-through)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de eventos</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do Evento (contém): RTP-Campaigns</strong><br><strong>[show] Ação do evento (correspondência exata): Cliques</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Total de cliques</strong></li> 
     <li>Tipo: <strong>Métrica 2.1</strong><br></li> 
     <li>Mostrar a seguinte métrica: <strong>Pageviews</strong></li> 
     <li>Filtro: <strong>[mostrar somente] Página (contendo): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do evento (correspondência exata): RTP-Campaigns</strong><br><strong>[show] Ação do evento (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da sessão (Clickthrough)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do evento (correspondência exata): RTP-Campaigns</strong><br><strong>[show] Ação do evento (correspondência exata): cliques</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Conteúdo recomendado</strong></li> 
     <li>Tipo: <strong>Tabela</strong><br></li> 
     <li>Exiba as seguintes colunas: <br><strong>Título da página | Pageviews</strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[mostrar somente] Página (contendo): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas/Sessão</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do evento (correspondência exata): RTP-Campaigns</strong></li> 
     <li><strong>[show] Ação do evento (correspondência exata): impressão</strong></li> 
     <li><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Clickthrough)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas/Sessão</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do evento (correspondência exata): RTP-Campaigns</strong></li> 
     <li><strong>[show] Ação do evento (correspondência exata): cliques</strong></li> 
     <li><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impressões do CTA</strong></li> 
     <li>Tipo: <strong>Tabela</strong></li> 
     <li>Exiba as seguintes colunas: <strong>Rótulo do evento | Total de eventos | Usuários</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do evento (correspondência exata): RTP-Campaigns</strong><br><strong>[show] Ação do evento (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Click-through do CTA</strong></li> 
     <li>Tipo: <strong>Tabela</strong></li> 
     <li>Exiba as seguintes colunas: <strong>Rótulo do evento | Total de eventos | Usuários</strong></li> 
     <li>Filtros:<br><strong>[show] Categoria do evento (correspondência exata): RTP-Campaigns</strong><br><strong>[show] Ação do evento (correspondência exata): cliques</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integrar RTP ao Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Relatórios RTP personalizados no Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
