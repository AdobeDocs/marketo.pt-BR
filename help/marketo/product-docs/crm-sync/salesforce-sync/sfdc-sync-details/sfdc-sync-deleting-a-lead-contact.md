---
unique-page-id: 7515131
description: Entenda como a exclusão de clientes potenciais e contatos funciona entre o Salesforce e o Marketo. Saiba mais sobre as ações de fluxo Excluir pessoa e Excluir de SFDC do SFDC.
title: Sincronização da SFDC - Excluindo um cliente em potencial/contato
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/v0nRloqmlp-iedcmE4DdATxpYXnvB13cxkEn7809Hy4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 4%

---

# Sincronização do SFDC: exclusão de um lead/contato {#sfdc-sync-deleting-a-lead-contact}

Estes são alguns detalhes:

* O Marketo não exclui pessoas automaticamente apenas porque os clientes potenciais foram excluídos em [!DNL Salesforce]. Em vez disso, o sinalizador &quot;O SFDC foi excluído&quot; está definido como verdadeiro. É possível acionar esse campo para exclusão no Marketo, se desejado.
* Ação de fluxo [Excluir Pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md). Isso exclui uma pessoa no MKTO, mas você também tem a opção de excluir no `Salesforce`.

* [Ação de fluxo Excluir do SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md): isso exclui um cliente potencial no SFDC, mas você também pode excluir uma pessoa no Marketo.
* Se um cliente potencial for excluído em [!DNL Salesforce] (mas uma pessoa não for excluída no Marketo) e em seguida executar a ação de fluxo [Sincronizar com [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), ele criará um novo cliente potencial em [!DNL Salesforce].
