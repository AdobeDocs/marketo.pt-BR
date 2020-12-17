---
unique-page-id: 7515131
description: Sincronização SFDC - Excluindo um cliente potencial/contato - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Excluindo um cliente potencial/contato
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Sincronização SFDC: Excluindo um cliente potencial/contato {#sfdc-sync-deleting-a-lead-contact}

Estes são alguns dos detalhes:

* O Marketo não exclui automaticamente as pessoas apenas porque as vendas foram excluídas no Salesforce. Em vez disso, um sinalizador de campo &quot;SFDC Está Excluído&quot; é definido como true. Você pode disparar esse campo para excluir no Marketo, se desejar.
* [Ação Excluir ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) fluxo de pessoal. Isso exclui uma pessoa no MKTO, mas você também tem a opção de excluir em `Salesforce`.

* [Ação Excluir do ](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) SFDCflow: Isso exclui um cliente potencial no SFDC, mas você também tem a opção de excluir uma pessoa no Marketo.
* Se um cliente potencial for excluído no Salesforce (mas uma pessoa não for excluída no Marketo) e, em seguida, for executado pela ação de fluxo [Sincronizar com o Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), ele criará um novo cliente potencial no Salesforce.

Em outras palavras, funciona como mágica!

![—](assets/image2015-5-20-15-3a3-3a27.png)

