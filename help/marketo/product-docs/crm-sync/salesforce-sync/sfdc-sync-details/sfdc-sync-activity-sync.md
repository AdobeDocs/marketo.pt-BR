---
unique-page-id: 2953473
description: Sincronização SFDC - Sincronização de Atividade - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de Atividade
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de atividade {#sfdc-sync-activity-sync}

O Marketo também é sincronizado com os dados do Salesforce atividade. Aqui estão algumas perguntas e respostas.

## Por que tipos de dados de atividade o Marketo sincroniza? {#what-types-of-activity-data-does-marketo-sync-over}

O Marketo sincroniza tanto Eventos quanto Tarefas associadas a um cliente potencial ou contato.

## Como os detalhes da atividade são mantidos em sincronia entre os dois sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

A sincronização é de uma maneira, de Salesforce a Marketo. Mas é possível criar uma tarefa no Salesforce usando a etapa [Criar fluxo de Tarefa](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ou [Personalizar sincronização](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) do Atividade para o Salesforce.

## Posso criar uma tarefa usando o Marketo? {#can-i-create-a-task-using-marketo}

Sim, você pode usar a ação [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)Criar fluxo de Tarefa.

## Quais são os acionadores/filtros relacionados à atividade? {#what-are-the-triggers-filters-related-to-activity}

Acionadores

* A atividade está registrada
* A atividade foi atualizada

Filtros

* A atividade foi registrada/a Atividade não foi registrada
* A atividade foi atualizada/A Atividade não foi atualizada

>[!TIP]
>
>Não tem certeza sobre essa redação &quot;não Atividade&quot;? O &quot;não&quot; refere-se a um Filtro de inatividade. Saiba mais sobre eles aqui: [Usar Filtros de inatividade em uma Lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

