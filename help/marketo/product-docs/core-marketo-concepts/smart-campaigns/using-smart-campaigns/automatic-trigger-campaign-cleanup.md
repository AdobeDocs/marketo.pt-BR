---
unique-page-id: 1147074
description: Limpeza automática do Campaign de acionador - Documentação do Marketo - Documentação do produto
title: Limpeza de campanha com gatilho automático
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 3%

---

# Limpeza de campanha com gatilho automático {#automatic-trigger-campaign-cleanup}

O Marketo tem um serviço gratuito para desativar campanhas inteligentes acionadas que não recebem mais atividade. Isso acelera o desempenho geral do sistema e economiza tempo.

## O que acontece? {#what-happens}

Uma vez por trimestre, o Marketo encontrará campanhas inteligentes que permaneceram inativas (sem pessoas) por seis meses ou mais e as desativará.

## Você vai me notificar primeiro? {#will-you-notify-me-first}

Claro! Uma vez por trimestre, você receberá uma notificação com uma semana de antecedência, mostrando todas as campanhas que pretendemos desativar.

1. Clique em **Notificação** ícone.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Clique em **Limpeza de Campanha do Acionador Ocioso Agendada**. Em seguida, clique no link **Essas campanhas do acionador ocioso serão desativadas** link.

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Você verá uma lista de campanhas inteligentes agendadas para serem desativadas.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## Quais campanhas serão desativadas? {#which-campaigns-will-be-deactivated}

Desativaremos apenas campanhas de acionadores que estiveram ativas por mais de 6 meses, mas que tiveram 0 pessoas qualificadas nesse período de tempo.

## Espere! Esta campanha não! {#wait-not-this-campaign}

Não se preocupe - o relógio em qualquer campanha inteligente pode ser redefinido por:

* Uma pessoa qualificada para a campanha.
* Desativar e reativar manualmente a campanha.

Qualquer um redefinirá o contador de 6 meses.

## Você me informará quais campanhas foram desativadas? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolutamente - uma semana após a notificação original, desativaremos as campanhas listadas (menos qualquer uma que tenha qualificado pelo menos uma pessoa ou que tenha sido desativada/reativada) e postaremos uma notificação de confirmação.

1. Selecione o **Limpeza de Campanha do Acionador Ocioso Agendada** notificação. Clique em **Essas Campanhas De Acionador Ocioso** link.

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. Você verá uma lista de campanhas desativadas.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
