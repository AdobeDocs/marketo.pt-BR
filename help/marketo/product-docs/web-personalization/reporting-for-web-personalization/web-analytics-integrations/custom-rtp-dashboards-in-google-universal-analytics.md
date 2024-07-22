---
unique-page-id: 7504238
description: Painéis RTP personalizados no Google Universal Analytics - Documentação do Marketo - Documentação do produto
title: Painéis RTP personalizados no Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Painéis RTP personalizados no Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP com o Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Esta publicação explica como configurar painéis RTP no Google Universal Analytics (GUA). Os dados enviados do RTP para o GUA podem ser configurados como dois painéis personalizados separados chamados:

* RTP B2B
* Envolvimento com RTP

## Configurar um painel personalizado {#setting-up-a-custom-dashboard}

1. Faça logon no Google Analytics. Clique em **Relatórios** no menu superior. Clique em **Painéis** e **+Novo Painel Personalizado**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Selecione **Tela em Branco**, adicione um **Nome do Painel** e clique em **Criar Painel**.

1. Clique em **Adicionar widget** para criar um novo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Painel B2B RTP {#rtp-b-b-dashboard}

Esse painel permite que os usuários analisem o desempenho do site a partir de uma perspectiva B2B.

Ela fornece informações como origem de visitas e comportamento no local por setor, receita, tamanho, listas baseadas em conta e segmentos de destino.

O painel consiste em 3 colunas

* Fonte de tráfego
* Segmentação
* Perfuração firme

1. Crie um novo painel chamado **Painel B2B RTP** e defina os seguintes widgets:

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
    <div> <strong>Coluna 3 - Detalhamento Firmográfico</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: Sessões por segmentos e canais</li> 
     <li>Tipo de dispositivo: barra<br></li> 
     <li>Criar um gráfico de barras que mostre: Sessão</li> 
     <li>Agrupado por: Rótulo do evento</li> 
     <li>Deslocar por: Agrupamento de canal padrão</li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: nº de usuários segmentados RTP</li> 
     <li>Tipo: 2.1 métrica</li> 
     <li>Mostrar a seguinte métrica: Usuários<br></li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Sessões por setor</li> 
     <li>Tipo: Pizza<br></li> 
     <li>Criar um gráfico de pizza mostrando: Sessões</li> 
     <li>Agrupado por: RTP-Industry</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por setor e canais</strong></li> 
     <li><strong>Tipo de dispositivo: barra</strong></li> 
     <li><strong>Criar um gráfico de barras que mostre: Sessão</strong></li> 
     <li><strong>Agrupado por: RTP-Industry</strong></li> 
     <li><strong>Deslocar por: Agrupamento de canal padrão</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões segmentadas por país</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Plotar métrica selecionada: País | Sessões</strong></li> 
     <li><strong>Selecione uma região: O mundo</strong></li> 
     <li><strong>Filtro: Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por Categoria RTP</strong></li> 
     <li><strong>Tipo: Pizza</strong></li> 
     <li><strong>Criar um gráfico de pizza mostrando: Sessões</strong></li> 
     <li><strong>Agrupado por: RTP-Category</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Principais Segmentos do Target</li> 
     <li>Tipo: Barra</li> 
     <li>Criar um gráfico de barras que mostre: Usuários</li> 
     <li>Agrupado por: Ação de evento</li> 
     <li>Filtro: Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: Sessões por Grupos RTP</li> 
     <li>Tipo: Barra<br></li> 
     <li>Criar um gráfico de barras que mostra: Sessões</li> 
     <li>Agrupado por: RTP-Group</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Sessões e Metas por Segmentos Principais</li> 
     <li>Tipo: Tabela<br></li> 
     <li>Exibir as seguintes colunas: <br>Rótulo de Evento | Sessões | Índice de conversão de meta</li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## Painel de Envolvimento RTP {#rtp-engagement-dashboard}

Esse painel permite que os usuários analisem o desempenho da campanha RTP e os engajamentos do mecanismo de recomendação. Ela fornece a comparação da média duração da sessão e páginas por sessão entre:

* Não engajado
* Engajado (impressões e cliques em uma campanha personalizada)
* Cliques no Mecanismo de recomendação e principais conteúdos recomendados

Crie um novo painel chamado **Painel de Envolvimento RTP** e defina os seguintes widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Coluna 1 - Exposição de Campanhas</strong> 
    </div></th> 
   <th> 
    <div> <strong>Clickthrough de Campanhas da Coluna 2</strong> 
    </div></th> 
   <th> 
    <div> <strong>Mecanismo de Recomendação da Coluna 3</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Total de CTA (Compromisso)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de eventos</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (contém): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de Evento (exatamente correspondente): Impressão</strong><strong>[não mostrar] Rótulo de Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Total de CTA (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de eventos</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (contém): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de Evento (correspondência exata): Cliques</strong><strong>[não mostrar] Rótulo de Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Total de Cliques</strong></li> 
     <li>Tipo: <strong>2.1 Métrica</strong><br></li> 
     <li>Mostrar a seguinte métrica: <strong>Pageviews</strong></li> 
     <li>Filtro: <strong>[mostrar apenas] Página (contendo): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da Sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de evento (correspondência exata): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de evento (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da Sessão (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de evento (correspondência exata): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de evento (correspondência exata): cliques</strong><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Principal Conteúdo Recomendado</strong></li> 
     <li>Tipo: <strong>Tabela</strong><br></li> 
     <li>Exibir as seguintes colunas: <br><strong>Título da Página | Exibições de página</strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[mostrar apenas] Página (contendo): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas/Sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (correspondência exata): RTP-Campanhas</strong></li> 
     <li><strong>[mostrar apenas] Ação do evento (correspondência exata): impressão</strong></li> 
     <li><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Click-through)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas/Sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (correspondência exata): RTP-Campanhas</strong></li> 
     <li><strong>[mostrar apenas] Ação do evento (correspondência exata): cliques</strong></li> 
     <li><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impressões por CTA</strong></li> 
     <li>Tipo: <strong>Tabela</strong></li> 
     <li>Exibir as seguintes colunas: <strong>Rótulo de Evento | Total de eventos | Usuários</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de evento (correspondência exata): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de evento (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Clickthrough de CTA</strong></li> 
     <li>Tipo: <strong>Tabela</strong></li> 
     <li>Exibir as seguintes colunas: <strong>Rótulo de Evento | Total de eventos | Usuários</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de evento (correspondência exata): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de evento (correspondência exata): cliques</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integrar RTP com o Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Relatórios RTP personalizados no Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
