---
unique-page-id: 2951640
description: Uso De Momentos Interessantes - Documentação Do Marketo - Documentação Do Produto
title: Usar momentos interessantes
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Usar momentos interessantes {#using-interesting-moments}

Momentos interessantes são a chave para se comunicar com sua equipe de vendas por meio do aplicativo Marketo Sales Insight.

>[!AVAILABILITY]
>
>Eles estão disponíveis somente para clientes do Marketo Sales Insight e do [Marketo Sales Connect](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md).

## O que é um momento interessante? {#what-is-an-interesting-moment}

Isso depende de você! Você decide quais informações são relevantes para sua equipe de vendas. Sua equipe de vendas pode querer saber quando um lead:

* Visita a página de preços no seu site
* Cliques em um link em um novo email de anúncio do produto
* Solicita uma demonstração do produto

## Como criar um momento interessante?  {#how-do-i-create-an-interesting-moment}

1. Escolha uma [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), de preferência uma que sua equipe de vendas achará interessante se for acionada.

   ![](assets/using-interesting-moments-1.png)

1. Arraste sobre a etapa de fluxo **Momentos interessantes**.

   ![](assets/using-interesting-moments-2.png)

1. Selecione um **tipo** (Email, Marco ou Web).

   ![](assets/using-interesting-moments-3.png)

1. Escreva uma mensagem para sua equipe de vendas no campo **Descrição** que explique por que essa ação é importante.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >O Marketo também adicionará a data em que ocorreu e como o momento interessante foi adicionado (ou seja, ação principal > etapa de fluxo, API SOAP).

## Como isso pode ficar ainda mais interessante?  {#how-can-this-get-even-more-interesting}

Tokens! Adicione-os no campo de descrição para fornecer à sua equipe de vendas informações mais específicas, como a linha de assunto do email que o cliente potencial abriu ou por quem foi enviado. Confira quais tokens estão disponíveis para uso no glossário [Tokens para momentos interessantes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md).

>[!TIP]
>
>Comece com cinco momentos interessantes e trabalhe com sua equipe de vendas para determinar quais informações eles estão interessados em ver.

## Como se parece um momento interessante no Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Momentos interessantes serão exibidos em um [log de atividades do cliente potencial](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## Como se parece um momento interessante no Salesforce?  {#what-does-an-interesting-moment-look-like-in-salesforce}

Depois que você [instalar o aplicativo Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md), momentos interessantes serão exibidos nas páginas de cliente potencial, contato, conta ou oportunidade. Elas também aparecem no painel Sales Insight no feed de lead, nas Melhores opções e na Lista de observação.

![](assets/using-interesting-moments-6.png)

## Como é um momento interessante no Salesforce1? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Depois de instalar ou atualizar o Marketo Sales Insight for Salesforce1, momentos interessantes serão exibidos nos links relacionados ao lead.

![](assets/using-interesting-moments-7.png)

## Inscrever-se em momentos interessantes {#subscribe-to-interesting-moments}

Você pode assinar um momento interessante clicando no botão Assinar na guia Momento interessante ou no Feed principal. As etapas abaixo são as mesmas para ambos.

1. Clique no ícone Subscribe. Você será direcionado para a guia Email Subscribe.

1. Você pode escolher o tipo de alerta por email que gostaria de receber com base em Nome, Conta, Tipo ou Descrição.

1. Escolha quais endereços de email você gostaria de enviar para os alertas (você mesmo/membros da equipe)

1. Clique em **Assinar**.

>[!NOTE]
>
>Ao se inscrever em Tipos ou Descrições de momento interessantes, o usuário receberá notificações por email das pessoas (clientes potenciais/contatos) que possuem quando acionarem um Momento interessante correspondente a esse Tipo ou Descrição.

![](assets/using-interesting-moments-8.png)
