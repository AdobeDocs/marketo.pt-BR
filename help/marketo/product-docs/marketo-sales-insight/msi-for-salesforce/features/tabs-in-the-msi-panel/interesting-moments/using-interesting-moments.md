---
unique-page-id: 2951640
description: Uso de momentos interessantes - Documentação da Marketo - Documentação do produto
title: Uso de momentos interessantes
exl-id: ccf7664b-08e1-490a-a3f9-5fa3bd8fb05f
source-git-commit: e651aa8eb79935f5c00594104c60818df9617fb6
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Uso de momentos interessantes {#using-interesting-moments}

Os momentos interessantes são a chave para se comunicar com sua equipe de vendas por meio do aplicativo Marketo Sales Insight.

>[!AVAILABILITY]
>
>Eles estão disponíveis para o Marketo Sales Insight e [Marketo Sales Connect](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-sales-connect.md) somente clientes.

## O que é um momento interessante? {#what-is-an-interesting-moment}

Isso depende de você! Você decide quais informações são relevantes para sua equipe de vendas. Sua equipe de vendas pode desejar saber quando um cliente potencial:

* Visita a página de preços em seu site
* Clica em um link em um novo email de anúncio de produto
* Solicita uma demonstração de produto

## Como criar um momento interessante?  {#how-do-i-create-an-interesting-moment}

1. Escolha um [campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md), preferencialmente uma de suas equipes de vendas acharia interessante se fosse acionado.

   ![](assets/using-interesting-moments-1.png)

1. Arraste para o **Momentos interessantes** etapa de fluxo.

   ![](assets/using-interesting-moments-2.png)

1. Selecione um **type** (Email, Marco ou Web).

   ![](assets/using-interesting-moments-3.png)

1. Escreva uma mensagem para sua equipe de vendas no **Descrição** que explica a importância desta ação.

   ![](assets/using-interesting-moments-4.png)

   >[!NOTE]
   >
   >A Marketo também adicionará a data de ocorrência e como o momento interessante foi adicionado (ou seja, ação de lead > etapa de fluxo, API SOAP).

## Como isso pode se tornar ainda mais interessante?  {#how-can-this-get-even-more-interesting}

Tokens! Adicione-os no campo de descrição para fornecer à equipe de vendas informações mais específicas, como a linha de assunto do email aberto pelo cliente potencial ou por quem ele foi enviado. Verifique quais tokens estão disponíveis para uso no [Tokens para Momentos Interessantes](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) glossário.

>[!TIP]
>
>Comece com cinco momentos interessantes e trabalhe com sua equipe de vendas para determinar quais informações eles estão interessados em ver.

## Como é um momento interessante no Marketo?  {#what-does-an-interesting-moment-look-like-in-marketo}

Os momentos interessantes serão exibidos em um [log de atividades do lead](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

![](assets/using-interesting-moments-5.png)

## Como se parece um momento interessante em Salesforce?  {#what-does-an-interesting-moment-look-like-in-salesforce}

Uma vez que você tiver [instalado o aplicativo Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md), momentos interessantes serão exibidos nas páginas de lead, contato, conta ou oportunidade. Eles também aparecem no painel Informações sobre vendas no Feed de clientes potenciais, Melhores apostas e Lista de monitoramento.

![](assets/using-interesting-moments-6.png)

## Como se parece um momento interessante em Salesforce1? {#what-does-an-interesting-moment-look-like-in-salesforce-1}

Depois de instalar ou atualizar o Marketo Sales Insight for Salesforce1, momentos interessantes serão exibidos nos links relacionados do cliente potencial.

![](assets/using-interesting-moments-7.png)

## Inscrever-se em momentos interessantes {#subscribe-to-interesting-moments}

Você pode assinar um Momento Interessante clicando no botão Assinar na guia Momento Interessante ou no Feed de lead. As etapas abaixo são as mesmas para ambos.

1. Clique no ícone Subscribe . Em seguida, você navegará até a guia Email Subscribe .

1. Você pode escolher o tipo de alerta de email que gostaria de receber com base em Nome, Conta, Tipo ou Descrição.

1. Escolha para quais endereços de email você deseja enviar os alertas (você mesmo/membros da equipe)

1. Clique em **Assinar**.

>[!NOTE]
>
>Ao se inscrever em Tipos de momento ou descrições interessantes, o usuário receberá notificações por email das pessoas (leads/contatos) de sua propriedade quando acionar um momento interessante correspondente a esse Tipo ou Descrição.

![](assets/using-interesting-moments-8.png)
