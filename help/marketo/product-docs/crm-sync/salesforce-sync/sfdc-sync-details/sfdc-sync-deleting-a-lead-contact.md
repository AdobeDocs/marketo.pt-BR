---
unique-page-id: 7515131
description: Sincronização SFDC - Excluindo um cliente potencial/contato - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Excluindo um cliente potencial/contato
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Sincronização SFDC: Excluindo um cliente potencial/contato {#sfdc-sync-deleting-a-lead-contact}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Estes são alguns dos detalhes:

* O Marketo não exclui automaticamente as pessoas apenas porque as vendas foram excluídas no Salesforce. Em vez disso, um sinalizador de campo &quot;SFDC Está Excluído&quot; é definido como true. Você pode disparar esse campo para excluir no Marketo, se desejar.
* [Ação de fluxo Excluir Pessoa](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) . Isso exclui uma pessoa no MKTO, mas você também tem a opção de excluí-la `Salesforce` .

* [Ação Excluir do fluxo SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) : Isso exclui um cliente potencial no SFDC, mas você também tem a opção de excluir uma pessoa no Marketo.
* Se um cliente potencial for excluído no Salesforce (mas uma pessoa não for excluída no Marketo) e, em seguida, executar a ação de fluxo [Sincronizar com Salesforce](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) , ele criará um novo cliente potencial no Salesforce.

Em outras palavras, funciona como mágica!

![--](assets/image2015-5-20-15-3a3-3a27.png)

