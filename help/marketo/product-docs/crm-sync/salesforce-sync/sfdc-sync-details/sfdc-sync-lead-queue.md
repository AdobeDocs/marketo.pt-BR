---
unique-page-id: 7516241
description: Sincronização SFDC - Fila de lead - Documentos do Marketo - Documentação do produto
title: Sincronização SFDC - Fila de lead
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 15%

---

# Sincronização SFDC: Fila de lead {#sfdc-sync-lead-queue}

O Marketo permite adicionar pessoas ao [Filas de lead do Salesforce](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) para ajudar na distribuição de leads. Aqui estão os detalhes.

## Como atribuir uma pessoa a uma fila no Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Você pode atribuir uma pessoa a uma fila de lead do Salesforce usando uma destas ações de fluxo:

* [Sincronizar pessoa à SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Não é possível criar ou alterar filas no Marketo.

## Como as informações do proprietário do cliente potencial são armazenadas se a pessoa pertencer a uma fila? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se um lead for de propriedade de uma fila no Salesforce, esses campos do proprietário das vendas serão mantidos vazios até que o lead seja atribuído a um proprietário.

* Nome do proprietário das vendas
* Sobrenome do proprietário das vendas
* Título do Proprietário de Vendas
* Telefone do proprietário das vendas
* Endereço de e-mail do proprietário das vendas
