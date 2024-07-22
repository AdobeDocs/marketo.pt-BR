---
unique-page-id: 2953473
description: Sincronização SFDC - Sincronização de atividade - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de atividades
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 4%

---

# Sincronização SFDC: Sincronização de Atividade {#sfdc-sync-activity-sync}

O Marketo Engage também é sincronizado com os dados de atividades do Salesforce. Aqui estão algumas perguntas e respostas.

## Em quais tipos de dados de atividade o Marketo é sincronizado? {#what-types-of-activity-data-does-marketo-sync-over}

O Marketo sincroniza eventos e tarefas associados a um cliente potencial ou contato.

## Como os detalhes da atividade são mantidos em sincronia entre os dois sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

A sincronização é unidirecional, do Salesforce para o Marketo. Mas você pode criar uma tarefa no Salesforce usando a etapa de fluxo [Criar tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} ou [Personalizar sincronização de atividades](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md){target="_blank"} para o Salesforce.

## Posso criar uma tarefa usando o Marketo? {#can-i-create-a-task-using-marketo}

Sim, você pode usar a [ação Criar fluxo de tarefas](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## Quais são os acionadores/filtros relacionados à atividade? {#what-are-the-triggers-filters-related-to-activity}

Gatilhos

* A atividade é registrada
* A atividade é atualizada

Filtros

* Atividade registrada/Não atividade registrada
* A atividade foi atualizada/Não, a atividade foi atualizada

>[!TIP]
>
>Não tem certeza sobre a frase &quot;Não é atividade&quot;? O &quot;não&quot; se refere a um Filtro de inatividade. Saiba mais sobre eles aqui: [Usar filtros de inatividade em uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
