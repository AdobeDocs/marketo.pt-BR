---
unique-page-id: 7504238
description: Painéis RTP personalizados no Google Universal Analytics - Documentação do Marketo - Documentação do produto
title: Painéis RTP personalizados no Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '758'
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

1. Faça logon no Google Analytics. Clique em **[!UICONTROL Relatórios]** no menu superior. Clique em **[!UICONTROL Painéis]** e **[!UICONTROL Novo Painel]**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Selecione **Tela em Branco**, adicione um **Nome do Painel** e clique em **[!UICONTROL Criar Painel]**.

1. Clique em **[!UICONTROL Adicionar widget]** para criar um novo widget.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## Painel B2B RTP {#rtp-b-b-dashboard}

Esse painel permite que os usuários analisem o desempenho do site a partir de uma perspectiva B2B.

Ela fornece informações como origem de visitas e comportamento no local por setor, receita, tamanho, listas baseadas em conta e segmentos de destino.

O painel consiste em 3 colunas

* Traffic source
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
     <li>Tipo de widget: <span class="uicontrol">Barra</span><br></li> 
     <li><span class="uicontrol">Criar um gráfico de barras que mostre</span>: <span class="uicontrol">Sessão</span></li> 
     <li><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">Rótulo de evento</span></li> 
     <li><span class="uicontrol">Deslocar por</span>: <span class="uicontrol">Agrupamento de Canais Padrão</span></li> 
     <li>Filtro: <br><span class="uicontrol">Somente Mostrar</span> | <span class="uicontrol">Categoria de Eventos</span> (<span class="uicontrol">contendo</span>) RTP-Segmentos</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: nº de usuários segmentados RTP</li> 
     <li>Tipo: <span class="uicontrol">2.1 Métrica</span></li> 
     <li><span class="uicontrol">Mostrar a seguinte métrica</span>: <span class="uicontrol">Usuários</span><br></li> 
     <li>Filtro: <br><span class="uicontrol">Somente Mostrar</span> | <span class="uicontrol">Categoria de eventos</span> (contendo) segmentos RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Sessões por setor</li> 
     <li>Tipo: <span class="uicontrol">Pizza</span><br></li> 
     <li><span class="uicontrol">Criar um gráfico de pizza mostrando</span>: <span class="uicontrol">Sessões</span></li> 
     <li><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">RTP-Indústria</span></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por setor e canais</strong></li> 
     <li><strong>Tipo de widget: <span class="uicontrol">Barra</span></strong></li> 
     <li><strong><span class="uicontrol">Criar um gráfico de barras que mostre</span>: <span class="uicontrol">Sessão</span></strong></li> 
     <li><strong><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">RTP-Indústria</span></strong></li> 
     <li><strong><span class="uicontrol">Deslocar por</span>: <span class="uicontrol">Agrupamento de Canais Padrão</span></strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões segmentadas por país</strong></li> 
     <li><strong>Tipo: <span class="uicontrol">Geomap</span></strong></li> 
     <li><strong><span class="uicontrol">Plotar métrica selecionada</span>: <span class="uicontrol">País</span> | <span class="uicontrol">Sessões</span></strong></li> 
     <li><strong><span class="uicontrol">Selecione uma região</span>: <span class="uicontrol">O Mundo</span></strong></li> 
     <li><strong>Filtro: <span class="uicontrol">Somente Mostrar</span> | <span class="uicontrol">Categoria de eventos</span> (contendo) segmentos RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por Categoria RTP</strong></li> 
     <li><strong>Tipo: <span class="uicontrol">Pizza</span></strong></li> 
     <li><strong><span class="uicontrol">Criar um gráfico de pizza mostrando</span>: <span class="uicontrol">Sessões</span></strong></li> 
     <li><strong><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">Categoria-RTP</span></strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Principais Segmentos do Target</li> 
     <li>Tipo: <span class="uicontrol">Barra</span></li> 
     <li><span class="uicontrol">Criar um gráfico de barras que mostre</span>: <span class="uicontrol">Usuários</span></li> 
     <li><span class="uicontrol">Agrupado por</span>: <span class="uicontrol">Ação de Evento</span></li> 
     <li>Filtro: <span class="uicontrol">Somente Mostrar</span> | <span class="uicontrol">Categoria de eventos</span> (contendo) segmentos RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: Sessões por Grupos RTP</li> 
     <li>Tipo: Barra<br></li> 
     <li>Criar um gráfico de barras que mostra: Sessões</li> 
     <li>Agrupado por: RTP-Group</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Sessões e Metas por Segmentos Principais</li> 
     <li>Tipo: Tabela<br></li> 
     <li>Exibir as seguintes colunas: <br>Rótulo de Evento | Sessões | Índice de conversão de meta</li> 
     <li>Filtro: <br>Mostrar apenas | Categoria de evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
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
     <li>Nome: <strong>Total de CTA (Envolvimento)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de eventos</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (contém): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de Evento (exatamente correspondente): Impressão</strong>[não mostrar] Rótulo de Evento (contendo): #</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Total de CTA (ClickThrough)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de eventos</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (contém): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de Evento (correspondência exata): Cliques</strong><strong>[não mostrar] Rótulo de Evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Total de Cliques</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">2.1 Métrica</span></strong><br></li> 
     <li><span class="uicontrol">Mostrar a seguinte métrica</span>: <strong><span class="uicontrol">Pageviews</span></strong></li> 
     <li>Filtro: <strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Página</span> (<span class="uicontrol">contendo</span>): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da Sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de evento (correspondência exata): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de evento (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da Sessão (Clickthrough)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de evento (correspondência exata): RTP-Campanhas</strong><br><strong>[mostrar apenas] Ação de evento (correspondência exata): cliques</strong><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Principal Conteúdo Recomendado</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabela</span></strong><br></li> 
     <li><span class="uicontrol">Exibir as seguintes colunas</span>: <br><strong><span class="uicontrol">Título da Página</span> | <span class="uicontrol">Exibições de página</span></strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Página</span> (<span class="uicontrol">contendo</span>): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">2.1 Métrica</span> </strong></li> 
     <li><span class="uicontrol">Mostrar a seguinte métrica</span>: <strong><span class="uicontrol">Páginas/Sessão</span></strong></li> 
     <li>Filtros:<br><strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Categoria de Eventos</span> (<span class="uicontrol">correspondência exata</span>): RTP-Campanhas</strong></li> 
     <li><strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Ação de Evento</span> (<span class="uicontrol">correspondência exata</span>): impressão</strong></li> 
     <li><strong>[<span class="uicontrol">não mostrar</span>] <span class="uicontrol">Rótulo de Evento</span> (<span class="uicontrol">contendo</span>): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Click-through)</strong></li> 
     <li>Tipo: <strong>2.1 Métrica </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas/Sessão</strong></li> 
     <li>Filtros:<br><strong>[mostrar apenas] Categoria de Evento (correspondência exata): RTP-Campanhas</strong></li> 
     <li><strong>[mostrar apenas] Ação do evento (correspondência exata): cliques</strong></li> 
     <li><strong>[não mostrar] Rótulo de evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impressões por CTA</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabela</span></strong></li> 
     <li><span class="uicontrol">Exibir as seguintes colunas</span>: <strong><span class="uicontrol">Rótulo do Evento</span> | <span class="uicontrol">Total de eventos</span> | <span class="uicontrol">Usuários</span></strong></li> 
     <li>Filtros:<br><strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Categoria de eventos</span> (<span class="uicontrol">exatamente correspondentes</span>): RTP-Campanhas</strong><br><strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Ação de eventos</span> (<span class="uicontrol">exatamente correspondentes</span>): impressão</strong><strong>[<span class="uicontrol">não mostrar</span>] <span class="uicontrol">Rótulo de Eventos</span> (<span class="uicontrol">contendo</span>): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Clickthrough de CTA</strong></li> 
     <li>Tipo: <strong><span class="uicontrol">Tabela</span></strong></li> 
     <li><span class="uicontrol">Exibir as seguintes colunas</span>: <strong><span class="uicontrol">Rótulo do Evento</span> | <span class="uicontrol">Total de eventos</span> | <span class="uicontrol">Usuários</span></strong></li> 
     <li>Filtros:<br><strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Categoria de Evento</span> (<span class="uicontrol">exatamente correspondentes</span>): RTP-Campanhas</strong><br><strong>[<span class="uicontrol">mostrar somente</span>] <span class="uicontrol">Ação de Evento</span> (<span class="uicontrol">exatamente correspondentes</span>): cliques</strong></li> 
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
