---
unique-page-id: 7516241
description: Saiba como atribuir pessoas às filas de clientes potenciais do Salesforce no Marketo. Use as ações de fluxo Sincronizar Pessoa com o SFDC ou Alterar Proprietário para distribuição de clientes potenciais.
title: Sincronização do SFDC - Fila de clientes potenciais
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/aUrT7qSMy65t3K07O176nt-Bzjm9urgnXKAkZgs1-cs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 150
ht-degree: 17%

---

# Sincronização do SFDC: fila de leads {#sfdc-sync-lead-queue}

O Marketo permite adicionar pessoas às [[!DNL Salesforce] filas de clientes potenciais](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm) para ajudar na distribuição de clientes potenciais. Aqui estão os detalhes.

## Como atribuir uma pessoa a uma fila no Marketo? {#how-to-assign-a-person-to-a-queue-in-marketo}

Você pode atribuir uma pessoa a uma fila de clientes em potencial [!DNL Salesforce] usando uma destas ações de fluxo:

* [Sincronizar pessoa ao SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}
* [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}

>[!NOTE]
>
>Não é possível criar ou alterar filas no Marketo.

## Como as informações do proprietário do lead são armazenadas se a pessoa pertencer a uma fila? {#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

Se um cliente potencial pertencer a uma fila em [!DNL Salesforce], esses campos de proprietário de vendas serão mantidos vazios até que o cliente potencial seja atribuído a um proprietário.

* Nome do proprietário das vendas
* Sobrenome do proprietário das vendas
* Título do Proprietário de Vendas
* Telefone do proprietário das vendas
* Endereço de e-mail do proprietário das vendas
