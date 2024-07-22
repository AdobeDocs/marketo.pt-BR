---
unique-page-id: 30082174
description: Momentos interessantes no Sales Connect - Marketo Docs - Documentação do produto
title: Momentos interessantes no Sales Connect
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
feature: Marketo Sales Connect
source-git-commit: 3a3287ed20962a052e0015161e34e33a95dd450a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Momentos interessantes no Sales Connect {#interesting-moments-in-sales-connect}

Momentos interessantes são a chave para se comunicar com sua equipe de vendas por meio do Marketo Sales Connect.

>[!AVAILABILITY]
>
>Eles estão disponíveis somente para clientes do [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) e do Marketo Sales Connect.

>[!PREREQUISITES]
>
>* Você deve ter uma [conexão com o Salesforce CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md){target="_blank"}
>* Você deve ser o proprietário do cliente em potencial ou contato no Salesforce
>* Você deve ter acesso a [conceder acesso à conexão Marketo Engage](/help/marketo/product-docs/marketo-sales-connect/marketo/granting-access-to-users.md){target="_blank"}

## O que é um momento interessante? {#what-is-an-interesting-moment}

Isso depende de você! Você decide quais informações são relevantes para sua equipe de vendas. Sua equipe de vendas pode querer saber quando um lead:

* Visita a página de preços no seu site
* Cliques em um link em um novo email de anúncio do produto
* Solicita uma demonstração do produto

## Como criar um momento interessante? {#how-do-i-create-an-interesting-moment}

1. Escolha uma [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), de preferência uma que sua equipe de vendas achará interessante se for acionada.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Arraste sobre a etapa de fluxo **Momentos interessantes**.

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Selecione um **tipo** (Email, Marco ou Web).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Escreva uma mensagem para sua equipe de vendas no campo **Descrição** que explique por que essa ação é importante.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >O Marketo também adicionará a data em que ocorreu e como o momento interessante foi adicionado (ou seja, ação principal > etapa de fluxo, API SOAP).

## Como se parece um momento interessante no Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Momentos interessantes serão exibidos em um [log de atividades do cliente potencial](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Como se parece um momento interessante no Sales Connect? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Momentos interessantes serão exibidos em tempo real no Feed ativo de um usuário. Utilizamos a ID de proprietário do lead no Salesforce para mostrar aos usuários momentos interessantes de clientes potenciais relevantes dos quais eles são proprietários. Os usuários podem acompanhar rapidamente com clientes potenciais por email/telefone/campanha de vendas clicando na lista suspensa ao lado do nome do cliente potencial.

![](assets/engagement.jpg)
