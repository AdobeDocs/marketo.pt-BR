---
title: comportamento esperado
description: Comportamento esperado
translation-type: tm+mt
source-git-commit: 642fd57105afff1031f18883c5809206f136b7c6
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---


# Comportamento esperado

<br> 

Neste artigo, você encontrará informações sobre o comportamento esperado associado às Audiências preditivas (PA).

## Considerações sobre dados e privacidade

* Todo o processamento de dados necessário para os modelos AI/ML ocorre na América do Norte.
* Os modelos AI/ML não usam informações específicas de cliente potencial, como nomes próprios ou sobrenomes, gênero, e-mails, números de contato etc. Os modelos utilizam apenas atributos gerais derivados de firmgráficos e registros de atividades.

## Para Audiências preditivas, você pode esperar o seguinte comportamento:

* O PA pode ser acessado tanto no Marketo Sky quanto na experiência do Marketo Classic. A disponibilidade de recursos específicos é a seguinte:
   * Filtros preditivos - [!DNL Sky/Classic]
   * Registros projetados - [!DNL Sky/Classic]
   * Previsões de probabilidade em nível de cliente potencial - [!DNL Sky/Classic]
   * Metas e rastreamento - somente [!DNL Sky]
   * Insights e recomendações - somente [!DNL Sky]
* [A ](/help/sky/getting-started-with-predictive-audiences.md) ativação inicial leva de **24 a 48** horas para que todos os processos sejam concluídos após a ativação do PA. Você verá todos os recursos de Audiências preditivas e Filtros preditivos na interface, mas pode levar até 24 horas para que esses recursos comecem a funcionar.
* **As previsões serão geradas somente para novas campanhas que são criadas após o recurso ser ativado.**

## Há algumas considerações adicionais específicas para filtros preditivos:

* Os filtros de Probabilidade de Registro e Participação só podem ser usados com programas de evento ou webinar. Os filtros Looklike e Unsubscribe podem ser usados em programas de e-mail, evento e webinar.
* Você pode aplicar filtros preditivos a uma campanha inteligente mesmo se o programa pai for criado antes de filtros preditivos serem ativados.
* Filtros preditivos não estão disponíveis para campanhas de disparo.
* Para executar uma campanha inteligente, filtros de probabilidade precisam ser usados em conjunto com outros filtros regulares.
* O recurso Regras salvas não está disponível para uso em campanhas que contêm filtros preditivos.
* Você pode usar **até 5** filtros preditivos em uma lista inteligente.
* Filtros preditivos podem processar um **máximo de 1 milhão de clientes potenciais qualificados**.
* Você pode ter **até 50 programas ativos** com filtros preditivos. Um programa ativo é qualquer programa que usa filtros preditivos e foi agendado pelo menos uma vez.

## Quando os registros projetados não estão disponíveis?

Os registros projetados não estarão disponíveis nos seguintes casos de uso:

* se o programa foi criado antes da adição de Audiências preditivas
* quando os status dos programas não estiverem mapeados para status do sistema
* quando não houver membros no programa
* quando não houver programas similares passados nos últimos 6 meses que correspondam aos critérios necessários
