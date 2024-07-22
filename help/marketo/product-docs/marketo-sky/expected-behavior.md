---
description: Comportamento Esperado - Documentação do Marketo - Documentação do produto
title: Comportamento esperado
hide: true
hidefromtoc: true
exl-id: d19130cf-186e-4aad-be32-6aad18c9d08b
source-git-commit: fb77478cdcd2b455e9f2359e16aca50143ce492c
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Comportamento esperado {#expected-behavior}

Neste artigo, você encontrará informações sobre o comportamento esperado associado ao Predictive Audiences (PA).

## Considerações sobre dados e privacidade

* Todo o processamento de dados necessário para os modelos de IA/ML ocorre na América do Norte.
* Os modelos de IA/ML não usam informações específicas do lead, como nome ou sobrenome, sexo, emails, números de contato etc. Os modelos utilizam apenas atributos gerais derivados de firmográficos e registros de atividades.

**Para Públicos preditivos, você pode esperar o seguinte comportamento**

* O PA é acessível no Marketo Sky e na experiência do Marketo Classic. A disponibilidade de recursos específicos é a seguinte:
   * Filtros preditivos - [!DNL Sky/Classic]
   * Registros projetados - [!DNL Sky/Classic]
   * Previsões de probabilidade de nível de lead - [!DNL Sky/Classic]
   * Metas e rastreamento - somente [!DNL Sky]
   * Insights e recomendações - somente [!DNL Sky]
* A ativação inicial leva de **24-48 horas** para que todos os processos sejam concluídos após a habilitação do PA. Você verá todos os recursos de Públicos-alvo preditivos e Filtros preditivos na interface, mas pode levar até 24 horas para que esses recursos comecem a funcionar.
* **As previsões só serão geradas para novas campanhas que forem criadas após a ativação do recurso.**

**Há algumas considerações adicionais específicas para filtros preditivos**:

* Os filtros de registro e probabilidade de participação só podem ser usados com programas de evento ou webinário. Filtros semelhantes e de cancelamento de inscrição podem ser usados em emails, eventos e programas de webinário.
* Você pode aplicar filtros preditivos a uma campanha inteligente, mesmo se o programa principal for criado antes da ativação dos filtros preditivos.
* Os filtros preditivos não estão disponíveis para campanhas de acionador.
* Para executar uma campanha inteligente, os filtros de probabilidade precisam ser usados junto com outros filtros comuns.
* O recurso Regras salvas não está disponível para uso em campanhas que contêm filtros preditivos.
* Você pode usar **até 5** filtros preditivos em uma lista inteligente.
* Os filtros preditivos podem processar um **máximo de 1 milhão de clientes potenciais qualificados**.
* Você pode ter **até 50 programas ativos** com filtros preditivos. Um programa ativo é qualquer programa que usa filtros preditivos e foi agendado pelo menos uma vez.

## Quando os registros projetados não estão disponíveis?

Os registros projetados não estarão disponíveis nos seguintes casos de uso:

* se o programa foi criado antes da adição de Predictive Audiences
* quando os status do programa não são mapeados para os status do sistema
* quando não há membros no programa
* quando não houver programas semelhantes anteriores nos últimos 6 meses que correspondam aos critérios necessários
