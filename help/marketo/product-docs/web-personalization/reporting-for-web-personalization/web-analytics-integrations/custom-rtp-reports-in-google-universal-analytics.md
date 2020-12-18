---
unique-page-id: 7504218
description: Relatórios RTP personalizados no Google Universal Analytics - Documentos do Marketing - Documentação do produto
title: Relatórios RTP personalizados no Google Universal Analytics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---


# Relatórios RTP personalizados no Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrar RTP ao Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

Esta publicação explica como configurar relatórios personalizados RTP para o Google Universal Analytics (GUA).  Os dados enviados de RTP para GUA podem ser configurados como dois relatórios personalizados separados chamados:

* RTP B2B
* Participação no RTP

## Configuração de um Relatório Personalizado {#setting-up-a-custom-report}

1. Efetue login em Google Analytics.
1. Clique em **Personalização **no menu superior.
1. Clique em **+Novo Relatório Personalizado.**

** ![](assets/image2015-3-22-16-3a10-3a48.png)

**

## Relatório RTP B2B {#rtp-b-b-report}

1. Nomeie o relatório **Relatório RTP B2B**.
1. Nomear a 1ª guia **Indústria **

   1. (Observação: você **Duplicado essa guia** e cria outros semelhantes - etapa 5)

1. Selecione o tipo de relatório** Explorer**.\
   ** ![](assets/image2015-3-22-16-3a15-3a25.png)

   **

1. Na seção **Grupos de métricas**, selecione as métricas relevantes para seu negócio.

   1. Recomendamos o seguinte:\
      ** ![](assets/image2015-3-22-16-3a16-3a40.png)

      **

1. Duplicado esta guia 4 vezes e nomeie-as:

   1. **Indústria**
   1. **Grupo**
   1. **Categoria**
   1. **ABM**
   1. **Organizações**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Na seção **Detalhamentos do Dimension** defina as dimensões relevantes para cada guia, como abaixo.

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
   <td>Indústria</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Grupo</td> 
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

1. Não defina nenhum filtros e defina este relatório como disponível para **Todos os dados do site da Web **(ou altere se relevante para uma conta específica do Analytics).
1. Clique em **Salvar**.\
   ![](assets/image2015-3-22-16-3a21-3a23.png)

## Relatório de envolvimento RTP {#rtp-engagement-report}

1. Nomeie o relatório **Relatório de Envolvimento RTP.**
1. Defina o nome da primeira guia como **Todo o envolvimento**

   1. (Observação: você vai Duplicado essa guia e criar outras semelhantes - etapa 5)

1. Selecione o tipo de relatório **Explorer**.\
   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Na seção Grupos de métricas, selecione as métricas relevantes para seu negócio. Esta é uma recomendação:\
   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplicado esta guia 4 vezes e nomeie-as:

   1. **Todos os envolvimentos**
   1. **Envolvimento por setor**
   1. **Participação por grupo**
   1. **Participação por Categoria**
   1. **Participação por ABM**

   ** ![](assets/image2015-3-22-16-3a26-3a21.png)\**

1. Na seção **Detalhamentos do Dimension** defina as dimensões relevantes para cada guia, como a seguir:

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
   <td>Todos os envolvimentos</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participação por ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participação por Categoria</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Participação por grupo</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Envolvimento por setor</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Defina os seguintes filtros:
1. 

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
   <td><p>Categoria evento</p></td> 
   <td>Regex</td> 
   <td>RTP-Campanhas|RTP-Recommendations|RTP-Segmentos</td> 
   <td colspan="1">Filtrará todos os outros eventos personalizados que não estão relacionados ao RTP</td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>Etiqueta do evento</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Permite filtrar da campanha dos relatórios usando # no nome da campanha</td> 
  </tr> 
 </tbody> 
</table>

1. Defina este relatório para estar disponível para **Todos os dados do site **(ou altere se necessário)

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Clique em **Salvar**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!NOTE]
>
>**Artigos relacionados**
>
>[Integrar RTP ao Google Universal Analytics](integrate-rtp-with-google-universal-analytics.md)
>
>[Painéis RTP personalizados no Google Universal Analytics](custom-rtp-dashboards-in-google-universal-analytics.md)

