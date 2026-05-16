---
unique-page-id: 2953473
description: Saiba mais sobre como as atividades e tarefas do Salesforce são sincronizadas com o Marketo. Crie tarefas do Marketo e use acionadores de atividades e filtros em Campanhas inteligentes.
title: SFDC Sync - Sincronização de atividades
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/N-pw1q0NXaJGKW1J1R4iqhgXhA42sX5nP0OWPXCuaBc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 175
ht-degree: 6%

---

# Sincronização do SFDC: sincronização de atividade {#sfdc-sync-activity-sync}

O Marketo também sincroniza os dados das atividades [!DNL Salesforce]. Aqui estão algumas perguntas e respostas.

## Em quais tipos de dados de atividade o Marketo é sincronizado? {#what-types-of-activity-data-does-marketo-sync-over}

O Marketo sincroniza eventos e tarefas associados a um cliente potencial ou contato.

## Como os detalhes da atividade são mantidos em sincronia entre os dois sistemas? {#how-are-activity-details-kept-in-sync-between-the-two-systems}

A sincronização é unidirecional, de [!DNL Salesforce] para Marketo. Mas você pode criar uma tarefa em [!DNL Salesforce] usando a etapa de fluxo [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ou [Personalizar Atividades Sincronizar](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) para [!DNL Salesforce].

## Posso criar uma tarefa usando o Marketo? {#can-i-create-a-task-using-marketo}

Sim, você pode usar a [ação Criar fluxo de tarefas](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}.

## Quais são os acionadores/filtros relacionados à atividade? {#what-are-the-triggers-filters-related-to-activity}

Acionadores

* A atividade é registrada
* A atividade é atualizada

Filtros

* Atividade registrada/Não atividade registrada
* A atividade foi atualizada/Não, a atividade foi atualizada

>[!TIP]
>
>Não tem certeza sobre a frase &quot;Não é atividade&quot;? O &quot;não&quot; se refere a um Filtro de inatividade. Saiba mais sobre eles aqui: [Usar filtros de inatividade em uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
