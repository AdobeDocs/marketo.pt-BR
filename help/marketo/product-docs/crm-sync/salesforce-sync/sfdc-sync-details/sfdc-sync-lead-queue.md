---
unique-page-id: 7516241
description: Sincronização SFDC - Fila principal - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Fila de cliente em potencial
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Sincronização SFDC: Fila de cliente potencial {#sfdc-sync-lead-queue}

O Marketo permite que você adicione pessoas às filas [de clientes potenciais do](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) Salesforce para ajudar na distribuição de clientes potenciais. Aqui estão os detalhes.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Como atribuir uma pessoa a uma fila no Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Você pode atribuir uma pessoa a uma fila de clientes potenciais do Salesforce usando uma destas ações de fluxo:

* [Sincronizar Pessoa com SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Alterar proprietário](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Não é possível criar ou alterar filas no Marketo.

## Como as informações do proprietário principal são armazenadas se a pessoa pertence a uma fila? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se um cliente potencial for propriedade de uma fila no Salesforce, esses campos do proprietário das vendas serão mantidos vazios até que o cliente potencial seja atribuído a um proprietário.

* Nome do proprietário da venda
* Sobrenome do proprietário de vendas
* Título do proprietário de vendas
* Número de Telefone do Proprietário de Vendas
* Endereço de email do proprietário de vendas

