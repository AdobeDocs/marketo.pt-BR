---
unique-page-id: 7515131
description: Sincronização SFDC - Exclusão de um lead/contato - Documentos da Marketo - Documentação do produto
title: Sincronização SFDC - Excluindo um Lead/Contato
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincronização SFDC: Excluindo um Lead/Contato {#sfdc-sync-deleting-a-lead-contact}

Estes são alguns dos detalhes:

* O Marketo não exclui automaticamente pessoas apenas porque os leads foram excluídos no Salesforce. Em vez disso, um sinalizador de campo &quot;SFDC é Excluído&quot; é definido como true. Você pode acionar esse campo para excluir no Marketo, se desejar.
* [Excluir pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) ação de fluxo. Isso exclui uma pessoa no MKTO, mas você tem a opção de excluir no `Salesforce` também.

* [Excluir do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) ação de fluxo: Isso exclui um lead no SFDC, mas você também tem a opção de excluir uma pessoa no Marketo.
* Se um cliente potencial for excluído no Salesforce (mas uma pessoa não for excluída no Marketo) e, em seguida, passar pelo [Sincronizar com o Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) ação de fluxo, então criaria um novo lead no Salesforce.
