---
unique-page-id: 7504218
description: Relatórios RTP personalizados no Google Universal Analytics - Documentos do Marketo - Documentação do produto
title: Relatórios RTP personalizados no Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 5%

---

# Relatórios RTP personalizados no Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP ao Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

Este artigo explica como configurar relatórios personalizados RTP para o Google Universal Analytics (GUA).  Os dados enviados de RTP para GUA podem ser configurados como dois relatórios personalizados separados chamados de:

* RTP B2B
* Envolvimento RTP

## Configuração de um relatório personalizado {#setting-up-a-custom-report}

1. Faça logon no Google Analytics.

1. Clique em **Personalização** no menu superior.

1. Clique em **+Novo relatório personalizado**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## Relatório RTP B2B {#rtp-b-b-report}

1. Dê um nome ao relatório **Relatório RTP B2B**.

1. Nomeie a primeira guia **Setor**.

>[!NOTE]
>
>Você irá **Duplicar esta guia** e criar outros semelhantes - etapa 5)

1. Selecione o **Explorer** tipo de relatório.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. No **Grupos de métricas** selecione as métricas relevantes para sua empresa.

   a. Recomendamos o seguinte:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplique esta guia 4 vezes e nomeie-a:

   1. **Setor**
   1. **Agrupar**
   1. **Categoria**
   1. **ABM**
   1. **Organizações**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. No **Detalhamentos do Dimension** defina as dimensões relevantes para cada guia conforme abaixo.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nome da guia 
    </div></th> 
   <th> 
    <div>
      Detalhamentos do Dimension
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Setor</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Agrupar</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Categoria</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Organizações</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Não defina nenhum filtro e defina este relatório como disponível para **Todos os dados do site** (ou alterar se for relevante para uma conta específica do Analytics).

1. Clique em **Salvar**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Relatório de envolvimento RTP {#rtp-engagement-report}

1. Dê um nome ao relatório **Relatório de envolvimento RTP**.

1. Defina o nome da primeira guia como **Todos os Envolvimentos**.

>[!NOTE]
>
>Você duplicará essa guia e criará outras semelhantes - etapa 5)

1. Selecione o **Explorer** tipo de relatório.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Na seção Grupos de métricas , selecione as métricas relevantes para sua empresa. Aqui está uma recomendação:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplique esta guia 4 vezes e nomeie-a:

   1. **Todos os Envolvimentos**
   1. **Envolvimento do setor**
   1. **Participação por grupo**
   1. **Envolvimento por categoria**
   1. **Envolvimento do ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. No **Detalhamentos do Dimension** seção defina as dimensões relevantes para cada guia conforme abaixo:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Nome da guia 
    </div></th> 
   <th> 
    <div>
      Detalhamentos do Dimension 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Todos os Envolvimentos</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Envolvimento do ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Envolvimento por categoria</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participação por grupo</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Envolvimento do setor</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Defina os seguintes filtros:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Campo 
    </div></th> 
   <th> 
    <div>
      Tipo de correspondência 
    </div></th> 
   <th> 
    <div>
      Valores 
    </div></th> 
   <th colspan="1"> 
    <div>
      Comentários 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>Incluir</p></td> 
   <td><p>Categoria de eventos</p></td> 
   <td>Expressão regular</td> 
   <td>RTP-Campaigns|RTP-Recommendations|RTP-Segments</td> 
   <td colspan="1">Filtrará todos os outros eventos personalizados que não estão relacionados ao RTP</td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>Rótulo do evento</td> 
   <td>Expressão regular</td> 
   <td>#</td> 
   <td colspan="1">Permite que você filtre de sua campanha de relatórios usando # no nome da campanha</td> 
  </tr> 
 </tbody> 
</table>

1. Configure este relatório para estar disponível para **Todos os dados do site** (ou alterar, se necessário).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Clique em **Salvar**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrar RTP ao Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Painéis RTP personalizados no Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
