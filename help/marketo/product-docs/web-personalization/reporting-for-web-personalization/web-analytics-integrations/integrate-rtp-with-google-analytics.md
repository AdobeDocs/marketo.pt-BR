---
unique-page-id: 2949158
description: Integrar RTP ao Google Analytics - Marketo Docs - Documentação do produto
title: Integrar RTP com Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Integrar RTP com Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>O Universal Analytics agora é o padrão operacional e todas as propriedades no Google foram atualizadas para o Universal Analytics.
>
>Este artigo mostra como usar o antigo Google Standard Analytics, mas recomendamos que você passe para o Universal Analytics.
>
>Se você ainda não estiver usando o [código de rastreamento do analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), a Google recomenda que você arraste o site para usá-lo. Os seguintes estão sendo descontinuados pelo Google:
>
>* ga.js
>* urchin.js
>* Snippets WAP/do lado do servidor
>* YT / MO
>* Variáveis personalizadas
>* Variáveis definidas pelo usuário
>
>Veja como integrar [Personalização da Web com o Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introdução {#introduction}

Analise suas análises da Web de um novo ângulo usando o fluxo de dados direto da Marketo Real-Time Personalization (RTP) para sua conta Google Analytics (GA). Meça suas visitas da Web no GA de acordo com organizações, setores e campanhas RTP. Exiba métricas como os tipos de setores ou segmentos RTP na DG e como elas executam e geram leads de acordo com diferentes fontes de tráfego (social, pago, orgânico), analisando as taxas de cliques em campanhas e medindo o impacto que as campanhas de personalização têm em seu site. Aproveite essa capacidade para obter o máximo benefício de sua conta RTP

**Audience Analytics RTP**

Com a integração, você tem uma nova dimensão em sua conta do GA. A RTP aprimora automaticamente seus painéis com:

1. Organizações e indústrias
1. Segmentos personalizados em RTP
1. Listas do Account-Based Marketing

Concentre-se em seus prospetos B2B principais. Analise canais por setores e segmentos direcionados.

## Relatório de Canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

O Painel B2B RTP ajuda você a entender o detalhamento dos visitantes de acordo com setores e segmentação RTP. Você pode ver o desempenho do visitante de acordo com o setor financeiro e de acordo com diferentes campanhas de marketing (pagas, orgânicas, sociais). O painel também fornece uma visão geral de alto nível de como seus segmentos RTP estão se saindo e faz drill-down para mostrar as principais organizações que visitam seu site.

## Fluxo comportamental {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

O relatório Fluxo de comportamento (veja a imagem) visualiza o caminho que os visitantes viajam de uma Página ou Evento para outra. O exemplo de imagem mostra o caminho de todos os visitantes do setor financeiro. Este relatório pode ajudar você a descobrir qual conteúdo mantém os visitantes envolvidos com seu site.

## Desempenho RTP {#rtp-performance}

Meça suas campanhas RTP e correlacione-as com sua média geral do site. Saiba como essas campanhas afetam as métricas do seu site e use esses dados para concentrar seus esforços de personalização nos alvos certos. Gere relatórios personalizados para entender melhor o desempenho de suas campanhas de personalização.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configurando RTP com Google Analytics {#setting-up-rtp-with-google-analytics}

1. Adicione o email rtp.ga2@gmail.com como um usuário Lido e Analisado em sua conta GA. Para obter mais detalhes, consulte [here](https://support.google.com/analytics/answer/2884495?hl=en).

1. Na sua conta RTP. Ir para **Configurações da conta**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Em **Configurações da conta**, **Domínio** e **Analytics**.

1. Clique em **Google Analytics**.

1. Ative o **Variáveis personalizadas** e **Eventos** para anexar esses dados da RTP ao Google Analytics.

1. Insira o **Slot** número para enviar dados de variável personalizada (o padrão é 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Clique em **Salvar**.

>[!NOTE]
>
>Para enviar dados do segmento para o GA, no [Página Editar segmento](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) na plataforma RTP, marque a caixa de seleção **Enviar evento para Google Analytics na correspondência do segmento**.

## Configuração de relatórios Google Analytics com dados RTP {#setting-up-google-analytics-reports-with-rtp-data}

No Google Analytics, você pode usar painéis, segmentação de GA e relatórios para exibir seus dados RTP:

* [Painéis](https://support.google.com/analytics/answer/1068216?hl=en) forneça uma visão geral do desempenho do site.
* Um Segmento GA destina-se a filtrar visitantes na interface do GA e visualizar o tráfego por segmento. Veja como criar um segmento [here](https://support.google.com/analytics/answer/3124493?hl=en).
* Criação [relatórios personalizados](https://support.google.com/analytics/answer/1033013?hl=en) para exibir e/ou configurar emails agendados. Consulte em Personalização > Novo relatório personalizado.
