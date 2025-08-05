---
unique-page-id: 7515131
description: Sincronização da SFDC - Excluindo um cliente potencial/contato - Documentação do Marketo - Documentação do produto
title: Sincronização da SFDC - Excluindo um cliente em potencial/contato
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Sincronização da SFDC: excluindo um cliente em potencial/contato {#sfdc-sync-deleting-a-lead-contact}

Estes são alguns detalhes:

* O Marketo não exclui pessoas automaticamente apenas porque os clientes potenciais foram excluídos em [!DNL Salesforce]. Em vez disso, o sinalizador &quot;O SFDC foi excluído&quot; está definido como verdadeiro. É possível acionar esse campo para exclusão no Marketo, se desejado.
* Ação de fluxo [Excluir Pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md). Isso exclui uma pessoa no MKTO, mas você também tem a opção de excluir no `Salesforce`.

* [Ação de fluxo Excluir do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md): isso exclui um cliente potencial no SFDC, mas você também pode excluir uma pessoa no Marketo.
* Se um cliente potencial for excluído em [!DNL Salesforce] (mas uma pessoa não for excluída no Marketo) e em seguida executar a ação de fluxo [Sincronizar com [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), ele criará um novo cliente potencial em [!DNL Salesforce].
