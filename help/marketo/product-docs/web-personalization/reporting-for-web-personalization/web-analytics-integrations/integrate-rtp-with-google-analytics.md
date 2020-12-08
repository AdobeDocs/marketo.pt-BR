---
unique-page-id: 2949158
description: Integrar RTP aos Google Analytics - Documentos do Marketing - Documentação do produto
title: Integrar RTP a Google Analytics
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---


# Integrar RTP a Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>O Universal Analytics agora é o padrão operacional e todas as propriedades no Google foram atualizadas para o Universal Analytics.
>
>Este artigo mostra como usar o Google Standard Analytics antigo, mas recomendamos que você passe para o Universal Analytics.
>
>Se você ainda não estiver usando o código [de rastreamento do](https://developers.google.com/analytics/devguides/collection/analyticsjs/)analytics.js, o Google recomenda que você remarque seu site para usá-lo. Os itens a seguir estão sendo substituídos pelo Google:
>
>* ga.js
>* urchin.js
>* Trechos de WAP/servidor
>* YT / MO
>* Variáveis personalizadas
>* Variáveis definidas pelo usuário

>
>
Veja como integrar a personalização [da Web ao Universal Analytics](integrate-rtp-with-google-universal-analytics.md)

## Introdução {#introduction}

Analise suas análises da Web de um novo ângulo usando o fluxo direto de dados do mercado para a personalização em tempo real (RTP) para sua conta Google Analytics (GA). Meça suas visitas na Web no GA de acordo com organizações, setores e campanhas RTP. Métricas de visualização, como os tipos de setores ou segmentos RTP em GA e como eles executam e geram clientes potenciais de acordo com diferentes fontes de tráfego (social, pago, orgânico), analisando as taxas de cliques em campanhas e medindo o impacto que as campanhas de personalização têm em seu site. Aproveite essa capacidade para obter o máximo benefício da sua conta RTP

**AUDIENCE ANALYTICS RTP**

Com a integração, você tem uma nova dimensão em sua conta GA. O RTP aprimora automaticamente seus painéis com:

1. Organizações e indústrias
1. Segmentos personalizados no RTP
1. Listas de marketing baseadas em conta

Concentre-se nos seus principais prospectos B2B. Analise canais por setores e segmentos direcionados.

## Relatório de canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

O Painel RTP B2B ajuda você a entender o detalhamento dos visitantes de acordo com verticais e segmentação RTP. Você pode ver o desempenho do seu visitante de acordo com o setor financeiro e de acordo com diferentes campanhas de marketing (pagas, orgânicas, sociais). O painel também fornece uma visão geral de alto nível sobre o desempenho dos segmentos RTP e detalha para mostrar as principais organizações que visitam seu site.

## Fluxo comportamental {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

O relatório de fluxo de comportamento (veja a imagem) visualiza o caminho que os visitantes viajam de uma Página ou Evento para a próxima. O exemplo de imagem mostra o caminho de todos os visitantes do setor financeiro. Este relatório pode ajudá-lo a descobrir qual conteúdo mantém os visitantes envolvidos no site.

## Desempenho RTP {#rtp-performance}

Meça suas campanhas RTP e correlacione-as com a média geral do site. Saiba como essas campanhas afetam as métricas do seu site e use esses dados para focar seus esforços de personalização nos públicos alvos certos. Gere relatórios personalizados para entender melhor o desempenho de suas campanhas de personalização.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configurando RTP com Google Analytics {#setting-up-rtp-with-google-analytics}

1. Adicione o e-mail [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#0674727628616734466b67746d6372692865696b), como um usuário do Read &amp; Analyze (Leia e analise), à sua conta GA. Para obter mais detalhes, consulte [aqui](https://support.google.com/analytics/answer/2884495?hl=en).
1. Na sua conta RTP. Vá para Configurações **da** conta.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Em Configurações **de** conta, **Domínio** e **Analytics**
1. Clique em Google Analytics**.**
1. Ative as Variáveis **e** Eventos **** personalizados relevantes para anexar esses dados de RTP a Google Analytics.
1. Insira o número do **slot** para enviar dados de variável personalizados (o padrão é 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

Clique em **SALVAR**.

>[!NOTE]
>
>Para enviar dados de segmento para o GA, na página [](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) Editar segmento na plataforma RTP, marque a caixa de seleção **Enviar Evento para Google Analytics na Correspondência** de segmentos.

## Configuração de relatórios de Google Analytics com dados RTP {#setting-up-google-analytics-reports-with-rtp-data}

Em Google Analytics, você pode usar painéis, segmentação de GA e relatórios para visualização dos dados RTP:

* [Os painéis](https://support.google.com/analytics/answer/1068216?hl=en) fornecem uma visão geral do desempenho do site.
* Um segmento GA é destinado a filtrar visitantes na interface GA e a visualização do tráfego por segmento. Veja como criar um segmento [aqui](https://support.google.com/analytics/answer/3124493?hl=en).
* Criar relatórios [](https://support.google.com/analytics/answer/1033013?hl=en) personalizados para visualização e/ou configurar e-mails programados. Consulte em Personalização > Novo relatório personalizado.
