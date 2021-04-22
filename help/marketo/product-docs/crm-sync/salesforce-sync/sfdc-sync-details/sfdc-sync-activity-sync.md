---
unique-page-id: 2953473
description: Sincronização SFDC - Sincronização de Atividade - Documentos do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Atividade
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 4%

---

# Sincronização SFDC: Sincronização de atividade {#sfdc-sync-activity-sync}

O Marketo também sincroniza os dados de atividades do Salesforce. Aqui estão algumas perguntas e respostas.

## Quais tipos de dados de atividade o Marketo sincroniza? {#what-types-of-activity-data-does-marketo-sync-over}

O Marketo sincroniza Eventos e Tarefas associados a um cliente potencial ou contato.

## Como os detalhes da atividade são mantidos em sincronia entre os dois sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

A sincronização é uma maneira, do Salesforce ao Marketo. Mas você pode criar uma tarefa no Salesforce usando a etapa de fluxo [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ou [Personalizar Sincronização de Atividades](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) no Salesforce.

## Posso criar uma tarefa usando o Marketo? {#can-i-create-a-task-using-marketo}

Sim, você pode usar a ação [Criar fluxo de tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md).

## Quais são os acionadores/filtros relacionados à atividade? {#what-are-the-triggers-filters-related-to-activity}

Gatilhos

* A atividade é registrada
* A atividade é atualizada

Filtros

* A atividade foi registrada/a atividade não foi registrada
* A atividade foi atualizada/a atividade não foi atualizada

>[!TIP]
>
>Não tem a certeza sobre esta redação &quot;Não é Atividade&quot;? O &quot;não&quot; refere-se a um Filtro de inatividade. Saiba mais sobre eles aqui: [Utilizar Filtros de Inatividade numa Lista Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
