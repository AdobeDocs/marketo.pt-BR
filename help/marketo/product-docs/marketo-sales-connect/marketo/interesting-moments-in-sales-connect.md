---
unique-page-id: 30082174
description: Momentos interessantes no Sales Connect - Documentos da Marketo - Documentação do produto
title: Momentos interessantes na conexão de vendas
exl-id: 210f31d1-606a-479d-8a2b-351b2b1a7678
source-git-commit: b18b2172e2c20cdb740854924a48fc996caf59f9
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Momentos interessantes na conexão de vendas {#interesting-moments-in-sales-connect}

Momentos interessantes são a chave para se comunicar com sua equipe de vendas por meio do Marketo Sales Connect.

>[!AVAILABILITY]
>
>Eles estão disponíveis somente para [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/using-interesting-moments.md) e clientes do Marketo Sales Connect.

## O que é um momento interessante? {#what-is-an-interesting-moment}

Isso depende de você! Você decide quais informações são relevantes para sua equipe de vendas. Sua equipe de vendas pode desejar saber quando um cliente potencial:

* Visita a página de preços em seu site
* Clica em um link em um novo email de anúncio de produto
* Solicita uma demonstração de produto

## Como criar um momento interessante? {#how-do-i-create-an-interesting-moment}

1. Escolha uma [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferencialmente uma que sua equipe de vendas acharia interessante se fosse acionada.

   ![](assets/image2015-1-8-18-3a8-3a54.png)

1. Arraste sobre a etapa de fluxo **Momentos interessantes** .

   ![](assets/image2015-1-8-18-3a15-3a20.png)

1. Selecione um **tipo** (Email, Marco ou Web).

   ![](assets/image2015-1-8-18-3a17-3a16.png)

1. Escreva uma mensagem para sua equipe de vendas no campo **Description** que explica por que essa ação é importante.

   ![](assets/image2015-1-8-18-3a18-3a23.png)

   >[!NOTE]
   >
   >A Marketo também adicionará a data de ocorrência e como o momento interessante foi adicionado (ou seja, ação de lead > etapa de fluxo, API SOAP).

## Como é um momento interessante no Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Os momentos interessantes serão exibidos em um log de atividades de [lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/image2015-1-14-18-3a45-3a58.png)

## Como é um momento interessante no Sales Connect? {#what-does-an-interesting-moment-look-like-in-sales-connect}

Momentos interessantes serão exibidos em tempo real no Feed ao vivo de um usuário. Usamos a ID do proprietário principal no Salesforce para mostrar aos usuários momentos interessantes de leads relevantes dos quais eles são proprietários. Os usuários podem acompanhar rapidamente os clientes potenciais por email/telefone/campanha de vendas clicando na lista suspensa ao lado do nome do cliente potencial.

![](assets/engagement.jpg)
