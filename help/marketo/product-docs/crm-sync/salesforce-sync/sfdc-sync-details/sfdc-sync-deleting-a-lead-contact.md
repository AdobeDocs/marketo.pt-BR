---
unique-page-id: 7515131
description: Sincronização do SFDC - Exclusão de um cliente em potencial/contato - Documentação da Marketo - Documentação do produto
title: Sincronização SFDC - Excluindo um cliente em potencial/contato
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Sincronização do SFDC: Excluindo um cliente em potencial/contato {#sfdc-sync-deleting-a-lead-contact}

Estes são alguns detalhes:

* O Marketo Engage não exclui pessoas automaticamente apenas porque os clientes em potencial foram excluídos no Salesforce. Em vez disso, o sinalizador &quot;SFDC está excluído&quot; está definido como verdadeiro. É possível acionar esse campo para exclusão no Marketo, se desejado.
* [Excluir pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md){target="_blank"} ação de fluxo. Isso exclui uma pessoa no MKTO, mas você tem a opção de excluir no `Salesforce` também.

* [Excluir do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md){target="_blank"} Ação de fluxo: exclui um cliente potencial no SFDC, mas você tem a opção de excluir uma pessoa no Marketo também.
* Se um cliente em potencial for excluído no Salesforce (mas uma pessoa não for excluída no Marketo) e, em seguida, passar pela [Sincronizar com o Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} ação de fluxo, então criaria um novo lead no Salesforce.
