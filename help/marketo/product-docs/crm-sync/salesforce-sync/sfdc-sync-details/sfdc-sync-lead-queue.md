---
unique-page-id: 7516241
description: Sincronização SFDC - Fila de clientes potenciais - Documentação do Marketo - Documentação do produto
title: Sincronização SFDC - Fila de clientes potenciais
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 15%

---

# Sincronização SFDC: Fila de clientes potenciais {#sfdc-sync-lead-queue}

Marketo Engage permite adicionar pessoas a [Filas de clientes potenciais do Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm){target="_blank"} para ajudar na distribuição de clientes potenciais. Aqui estão os detalhes.

## Como atribuir uma pessoa a uma fila no Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Você pode atribuir uma pessoa a uma fila de clientes potenciais do Salesforce usando uma destas ações de fluxo:

* [Sincronizar pessoa à SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Não é possível criar ou alterar filas no Marketo.

## Como as informações do proprietário do lead são armazenadas se a pessoa pertencer a uma fila? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se um cliente potencial pertencer a uma fila no Salesforce, esses campos do proprietário das vendas serão mantidos vazios até que o cliente potencial seja atribuído a um proprietário.

* Nome do proprietário das vendas
* Sobrenome do proprietário das vendas
* Título do Proprietário de Vendas
* Telefone do proprietário das vendas
* Endereço de e-mail do proprietário das vendas
