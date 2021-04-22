---
unique-page-id: 7515131
description: Sincronização SFDC - Exclusão de um lead/contato - Documentos da Marketo - Documentação do produto
title: Sincronização SFDC - Excluindo um Lead/Contato
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# Sincronização SFDC: Excluindo um Lead/Contato {#sfdc-sync-deleting-a-lead-contact}

Estes são alguns dos detalhes:

* O Marketo não exclui automaticamente pessoas apenas porque os leads foram excluídos no Salesforce. Em vez disso, um sinalizador de campo &quot;SFDC é Excluído&quot; é definido como true. Você pode acionar esse campo para excluir no Marketo, se desejar.
* [Ação Excluir ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) fluxo de trabalho. Isso exclui uma pessoa no MKTO, mas você também tem a opção de excluir em `Salesforce`.

* [Ação Excluir do ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow: Isso exclui um lead no SFDC, mas você também tem a opção de excluir uma pessoa no Marketo.
* Se um lead for excluído no Salesforce (mas uma pessoa não for excluída no Marketo) e, em seguida, passar pela ação de fluxo [Sincronizar com Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), ele criará um novo lead no Salesforce.
