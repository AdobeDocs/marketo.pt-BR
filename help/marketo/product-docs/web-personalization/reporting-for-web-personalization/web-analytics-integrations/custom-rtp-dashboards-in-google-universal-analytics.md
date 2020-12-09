---
unique-page-id: 7504238
description: Painéis RTP personalizados no Google Universal Analytics - Documentos do Marketing - Documentação do produto
title: Painéis RTP personalizados no Google Universal Analytics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---


# Painéis RTP personalizados no Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP ao Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

Esta publicação explica como configurar painéis RTP no Google Universal Analytics (GUA).  Os dados enviados de RTP para GUA podem ser configurados como dois painéis personalizados chamados:

* RTP B2B
* Participação no RTP

## Configuração de um Painel personalizado {#setting-up-a-custom-dashboard}

1. Faça logon em Google Analytics. Clique em **Relatórios **no menu superior. Clique em **Painéis **e **+Novo Painel personalizado.**

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Selecione Tela de desenho em **branco**, adicione um nome **de** Painel e clique em **Criar Painel**.

1. Clique em **Adicionar widget** para criar um novo widget.\
   ![](assets/image2015-3-22-16-3a46-3a48.png)

## PAINEL RTP B2B {#rtp-b-b-dashboard}

Este painel permite que os usuários analisem o desempenho de seu site da perspectiva B2B.

Ele fornece informações como origem da visita e comportamento no local por segmento do setor, receita, tamanho, listas baseadas em conta e segmentos de público alvo.

O painel consiste de 3 colunas

* Fonte de tráfego
* Segmentação
* Detalhamento de firmware

1. Crie um novo painel chamado **Painel RTP B2B **e defina os seguintes widgets:

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
     <li>Nome: Sessões por segmentos e Canais</li> 
     <li>Tipo de widget: Barra<br></li> 
     <li>Crie um gráfico de barras mostrando: Sessão</li> 
     <li>Agrupado por: Etiqueta do evento</li> 
     <li>Tabela dinâmica por: Agrupamento de Canais padrão</li> 
     <li>Filtro: <br>Mostrar somente | Categoria do Evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Nº de usuários segmentados RTP</li> 
     <li>Tipo: Métrica 2.1</li> 
     <li>Mostrar a seguinte métrica: Usuários<br></li> 
     <li>Filtro: <br>Mostrar somente | Categoria do Evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: Sessões por setor</li> 
     <li>Tipo: Pizza<br></li> 
     <li>Crie um gráfico de pizza mostrando: Sessões</li> 
     <li>Agrupado por: RTP-Indústria</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por setor e Canais</strong></li> 
     <li><strong>Tipo de widget: Barra</strong></li> 
     <li><strong>Crie um gráfico de barras mostrando: Sessão</strong></li> 
     <li><strong>Agrupado por: RTP-Indústria</strong></li> 
     <li><strong>Tabela dinâmica por: Agrupamento de Canais padrão</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões segmentadas por país</strong></li> 
     <li><strong>Tipo: Geomap</strong></li> 
     <li><strong>Gráfico da métrica selecionada: País | Sessões</strong></li> 
     <li><strong>Selecione uma região: O mundo</strong></li> 
     <li><strong>Filtro: Mostrar somente | Categoria do Evento (contendo) Segmentos RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Nome: Sessões por Categoria RTP</strong></li> 
     <li><strong>Tipo: Pizza</strong></li> 
     <li><strong>Crie um gráfico de pizza mostrando: Sessões</strong></li> 
     <li><strong>Agrupado por: CATEGORIA RTP</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Principais segmentos do Público alvo</li> 
     <li>Tipo: Barra</li> 
     <li>Crie um gráfico de barras mostrando: Usuários</li> 
     <li>Agrupado por: Ação do evento</li> 
     <li>Filtro: Mostrar somente | Categoria do Evento (contendo) Segmentos RTP</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Nome: Sessões por grupos RTP</li> 
     <li>Tipo: Barra<br></li> 
     <li>Crie um gráfico de barras mostrando: Sessões</li> 
     <li>Agrupado por: Grupo RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Nome: Sessões e metas pelos principais segmentos</li> 
     <li>Tipo: Tabela<br></li> 
     <li>Exiba as seguintes colunas: <br>Etiqueta do evento | Sessões | Taxa de conversão de objetivos</li> 
     <li>Filtro: <br>Mostrar somente | Categoria do Evento (contendo) Segmentos RTP</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## PAINEL de envolvimento RTP {#rtp-engagement-dashboard}

Este painel permite que os usuários analisem o desempenho da campanha RTP e os envolvimentos do mecanismo de recomendação. Ele fornece comparação de média. duração da sessão e páginas por sessão entre:

* 

   * Desengajado
   * Envolvido (impressões e cliques em uma campanha personalizada)
   * Cliques no mecanismo de recomendação e no conteúdo recomendado superior

Crie um novo painel chamado Painel **de envolvimento** RTP e defina os seguintes widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Coluna 1 Exposição Campanha</strong> 
    </div></th> 
   <th> 
    <div> <strong>Click-through de Campanhas da Coluna 2</strong> 
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
     <li>Nome: <strong>Total de CTA (Envolvimento)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de Eventos</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (contém): Ação do Evento RTP-Campanha</strong><br><strong>[só show] (correspondência exata): Rótulo do Evento de impressão</strong><strong>[não mostrar] (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Total de CTA (click-through)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Total de Eventos</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (contém): Ação do Evento RTP-Campanha</strong><br><strong>[só show] (correspondência exata): Cliques</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>CRE - Total de cliques</strong></li> 
     <li>Tipo: <strong>Métrica 2.1</strong><br></li> 
     <li>Mostrar a seguinte métrica: <strong>Pageviews</strong></li> 
     <li>Filtro: <strong>[só mostrar] Página (contendo): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (correspondência exata): Ação do Evento RTP-Campanha</strong><br><strong>[só show] (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>Média Duração da sessão (click-through)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Média Duração da sessão</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (correspondência exata): Ação do Evento RTP-Campanha</strong><br><strong>[só show] (correspondência exata): clica</strong><strong>em Rótulo do Evento [não mostrar] (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Nome: <strong>CRE - Conteúdo recomendado superior</strong></li> 
     <li>Tipo: <strong>Tabela</strong><br></li> 
     <li>Exiba as seguintes colunas: <br><strong>Título da página | Pageviews</strong><br></li> 
     <li>Filtros:<br>Filtro: <strong>[só mostrar] Página (contendo): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas/Sessão (Envolvimento)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas / Sessão</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (correspondência exata): CAMPANHAS RTP</strong></li> 
     <li><strong>[show] Ação do Evento (correspondência exata): impressão</strong></li> 
     <li><strong>Rótulo do Evento [não mostrar] (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Páginas / Sessão (Clickthrough)</strong></li> 
     <li>Tipo: <strong>Métrica 2.1 </strong></li> 
     <li>Mostrar a seguinte métrica: <strong>Páginas / Sessão</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (correspondência exata): CAMPANHAS RTP</strong></li> 
     <li><strong>[show] Ação do Evento (correspondência exata): cliques</strong></li> 
     <li><strong>Rótulo do Evento [não mostrar] (contendo): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Nome: <strong>Impressões do CTA</strong></li> 
     <li>Tipo: <strong>Tabela</strong></li> 
     <li>Exiba as seguintes colunas: <strong>Etiqueta do evento | Total de Eventos | Utilizadores</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (correspondência exata): Ação do Evento RTP-Campanha</strong><br><strong>[só show] (correspondência exata): impressão</strong><strong>[não mostrar] Rótulo do Evento (contendo): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Nome: <strong>Click-through do CTA</strong></li> 
     <li>Tipo: <strong>Tabela</strong></li> 
     <li>Exiba as seguintes colunas: <strong>Etiqueta do evento | Total de Eventos | Utilizadores</strong></li> 
     <li>Filtros:<br><strong>[só mostrar] Categoria do Evento (correspondência exata): Ação do Evento RTP-Campanha</strong><br><strong>[só show] (correspondência exata): cliques</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Artigos relacionados**
>
>[Integrar RTP ao Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)
>
>[Relatórios RTP personalizados no Google Universal Analytics](custom-rtp-reports-in-google-universal-analytics.md)

