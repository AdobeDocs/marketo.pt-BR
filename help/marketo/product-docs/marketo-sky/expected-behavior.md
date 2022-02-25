---
description: Comportamento esperado - Documentos do Marketo - Documentação do produto
title: Comportamento esperado
hide: true
hidefromtoc: true
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# Comportamento esperado {#expected-behavior}

Neste artigo, você encontrará informações sobre o comportamento esperado associado a públicos-alvo preditivos (PA).

## Considerações sobre dados e privacidade

* Todo o processamento de dados necessário para os modelos de AI/ML ocorre na América do Norte.
* Os modelos AI/ML não usam informações específicas de lead, como nomes ou sobrenomes, gênero, emails, números de contato, etc. Os modelos utilizam apenas atributos gerais derivados de firmográficos e registros de atividades.

**Para públicos-alvo preditivos, você pode esperar o seguinte comportamento**

* O PA pode ser acessado no Marketo Sky e na experiência do Marketo Classic. A disponibilidade de recursos específicos é a seguinte:
   * Filtros preditivos - [!DNL Sky/Classic]
   * Registros projetados - [!DNL Sky/Classic]
   * Previsões de probabilidade de nível de lead - [!DNL Sky/Classic]
   * Metas e rastreamento - [!DNL Sky] only
   * Insights e recomendações - [!DNL Sky] only
* [Ativação inicial](/help/marketo/product-docs/marketo-sky/getting-started-with-predictive-audiences.md) take **24 a 48 horas** para que todos os processos sejam concluídos após a ativação do PA. Você verá todos os recursos de Predictive Audiences e Predictive Filters na interface, mas pode levar até 24 horas para que esses recursos comecem a funcionar.
* **As previsões só serão geradas para novas campanhas que são criadas após a ativação do recurso.**

**Existem algumas considerações adicionais específicas para os filtros preditivos**:

* Os filtros de Probabilidade de Registro e Participação só podem ser usados com programas de evento ou webinar. Filtros de pesquisa e cancelamento de inscrição podem ser usados em programas de email, evento e webinar.
* Você pode aplicar filtros preditivos a uma campanha inteligente mesmo se o programa pai for criado antes da ativação de filtros preditivos.
* Filtros preditivos não estão disponíveis para campanhas do acionador.
* Para executar uma campanha inteligente, os filtros de probabilidade precisam ser usados junto com outros filtros regulares.
* O recurso Regras salvas não está disponível para uso em campanhas que contêm filtros preditivos.
* Você pode usar **até 5** filtros preditivos em uma lista inteligente.
* Filtros preditivos podem processar um **máximo de 1 milhão de clientes potenciais qualificados**.
* Você pode ter **até 50 programas ativos** com filtros preditivos. Um programa ativo é qualquer programa que usa filtros preditivos e foi agendado pelo menos uma vez.

## Quando os registros projetados não estão disponíveis?

Os registros projetados não estarão disponíveis nos seguintes casos de uso:

* se o programa foi criado antes da adição de Públicos preditivos
* quando os status do programa não são mapeados para status do sistema
* quando não houver membros no programa
* quando não existirem programas similares nos últimos 6 meses que correspondam aos critérios exigidos
