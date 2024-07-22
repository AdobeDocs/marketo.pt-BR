---
unique-page-id: 2949158
description: Integração do RTP com o Google Analytics - Documentação do Marketo - Documentação do produto
title: Integrar o RTP com o Google Analytics
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Integrar o RTP com o Google Analytics {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>O Universal Analytics agora é o padrão operacional e todas as propriedades no Google foram atualizadas para o Universal Analytics.
>
>Este artigo mostra como usar o Google Standard Analytics antigo, mas recomendamos que você mude para o Universal Analytics.
>
>Se você ainda não estiver usando o [código de rastreamento do analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/), a Google recomenda que você remarque seu site para usá-lo. Os seguintes itens estão sendo descontinuados pelo Google:
>
>* ga.js
>* urchin.js
>* WAP/snippets do lado do servidor
>* YT/MO
>* Variáveis personalizadas
>* Variáveis definidas pelo usuário
>
>Veja como integrar o [Web Personalization com o Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Introdução {#introduction}

Analise sua análise da Web de um novo ângulo usando o fluxo de dados direto do Marketo Real-Time Personalization (RTP) para sua conta Google Analytics (GA). Meça suas visitas da Web no GA de acordo com organizações, setores e campanhas RTP. Visualize métricas como os tipos de setores ou segmentos RTP no GA e como eles executam e geram leads de acordo com diferentes fontes de tráfego (social, paga, orgânica), analisando taxas de click-through em campanhas e medindo o impacto que as campanhas de personalização têm em seu site. Aproveite essa capacidade para obter o máximo benefício da sua conta RTP

**Audience Analytics RTP**

Com a integração, você terá uma nova dimensão em sua conta do GA. O RTP aprimora automaticamente seus painéis com:

1. Organizações e setores
1. Segmentos personalizados no RTP
1. listas do Account-Based Marketing

Concentre-se em seus principais clientes potenciais B2B. Analisar canais por setores e segmentos direcionados.

## Relatório de canal {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

O Painel B2B do RTP ajuda você a entender o detalhamento de seus visitantes de acordo com as verticais e a segmentação RTP. Você pode ver o desempenho do visitante de acordo com o setor financeiro e com diferentes campanhas de marketing (pagas, orgânicas, sociais). O painel também fornece uma visão geral de alto nível de como os segmentos de RTP estão se saindo e detalha para mostrar as principais organizações que visitam seu site.

## Fluxo comportamental {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

O relatório Fluxo de comportamento (veja a imagem) visualiza o caminho que os visitantes viajam de uma página ou evento para a próxima. O exemplo de imagem mostra o caminho de todos os visitantes do setor financeiro. Este relatório pode ajudar você a descobrir qual conteúdo mantém os visitantes envolvidos com seu site.

## Desempenho de RTP {#rtp-performance}

Meça suas campanhas RTP e correlacione-as com a média geral do site. Saiba como essas campanhas afetam as métricas do seu site e use esses dados para concentrar seus esforços de personalização nos públicos-alvo certos. Gere relatórios personalizados para entender melhor o desempenho de suas campanhas de personalização.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Configuração do RTP com Google Analytics {#setting-up-rtp-with-google-analytics}

1. Adicione o email rtp.ga2@gmail.com como um usuário de Leitura e Análise à sua conta do GA. Para obter mais detalhes, consulte [aqui](https://support.google.com/analytics/answer/2884495?hl=en).

1. Na sua conta RTP. Vá para **Configurações da conta**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Em **Configurações de Conta**, **Domínio** e **Analytics**.

1. Clique em **Google Analytics**.

1. Ative as **Variáveis personalizadas** e **Eventos** relevantes para anexar esses dados da RTP ao Google Analytics.

1. Insira o número de **Slot** para enviar dados de variáveis personalizadas (o padrão é 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Clique em **Salvar**.

>[!NOTE]
>
>Para enviar dados de segmento para o GA, na [página Editar segmento](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) da plataforma RTP, marque a caixa de seleção **Enviar evento para Google Analytics na Correspondência de segmentos**.

## Configuração de relatórios do Google Analytics com dados RTP {#setting-up-google-analytics-reports-with-rtp-data}

No Google Analytics, é possível usar painéis, segmentação do GA e relatórios para exibir seus dados de RTP:

* Os [painéis](https://support.google.com/analytics/answer/1068216?hl=en) fornecem uma visão geral do desempenho do site.
* Um Segmento do GA tem como objetivo filtrar visitantes na interface do GA e visualizar o tráfego por segmento. Veja como criar um segmento [aqui](https://support.google.com/analytics/answer/3124493?hl=en).
* Criando [relatórios personalizados](https://support.google.com/analytics/answer/1033013?hl=en) para exibir e/ou configurar emails agendados. Consulte em Personalização > Novo relatório personalizado.
