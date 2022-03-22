---
description: Momentos interessantes em ações de insight de vendas - Documentos da Marketo - Documentação do produto
title: Momentos interessantes em ações de insight de vendas
hide: true
hidefromtoc: true
source-git-commit: 2f86e4df7dec01ece6ef820674f84fd1ae8ebaf2
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Momentos interessantes em ações de insight de vendas {#interesting-moments-in-sales-insight-actions}

Os momentos interessantes são a chave para se comunicar com sua equipe de vendas por meio das Ações de informações de vendas da Marketo.

## O que é um momento interessante? {#what-is-an-interesting-moment}

Isso depende de você! Você decide quais informações são relevantes para sua equipe de vendas. Sua equipe de vendas pode desejar saber quando um cliente potencial:

* Visita a página de preços em seu site
* Clica em um link em um novo email de anúncio de produto
* Solicita uma demonstração de produto

## Como criar um momento interessante? {#how-do-i-create-an-interesting-moment}

1. Escolha um [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target=&quot;_blank&quot;}, preferencialmente uma de suas equipes de vendas acharia interessante se fosse acionado.

   ![](assets/interesting-moments-in-sales-insight-actions-1.png)

1. Arraste para o **Momentos interessantes** etapa de fluxo.

   ![](assets/interesting-moments-in-sales-insight-actions-2.png)

1. Selecione um **type** (Email, Marco ou Web).

   ![](assets/interesting-moments-in-sales-insight-actions-3.png)

1. Escreva uma mensagem para sua equipe de vendas no **Descrição** que explica a importância desta ação.

   ![](assets/interesting-moments-in-sales-insight-actions-4.png)

   >[!NOTE]
   >
   >A Marketo também adicionará a data de ocorrência e como o momento interessante foi adicionado (ou seja, ação de lead > etapa de fluxo, API SOAP).

## Como é um momento interessante no Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Os momentos interessantes serão exibidos em um [log de atividades do lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target=&quot;_blank&quot;}.

![](assets/interesting-moments-in-sales-insight-actions-5.png)

## Como é um momento interessante nas Ações de insight de vendas? {#what-does-an-interesting-moment-look-like-in-sales-insight-actions}

Momentos interessantes serão exibidos em tempo real no Feed ao vivo de um usuário. Usamos a ID do proprietário principal no Salesforce para mostrar aos usuários momentos interessantes de leads relevantes dos quais eles são proprietários. Os usuários podem acompanhar rapidamente os clientes potenciais por email/telefone/campanha de vendas clicando na lista suspensa ao lado do nome do cliente potencial.

![](assets/interesting-moments-in-sales-insight-actions-6.png)
