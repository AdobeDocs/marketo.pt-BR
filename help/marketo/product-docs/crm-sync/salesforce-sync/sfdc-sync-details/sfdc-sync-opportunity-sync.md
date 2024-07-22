---
unique-page-id: 2953467
description: Sincronização SFDC - Sincronização de oportunidade - Documentação do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Oportunidades
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 6%

---

# Sincronização SFDC: Sincronização de Oportunidades {#sfdc-sync-opportunity-sync}

## Como os detalhes da oportunidade são mantidos em sincronia entre os dois sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

A sincronização é uma maneira: do Salesforce para o Marketo Engage. As atualizações de oportunidades no Salesforce serão sincronizadas com o Marketo.

>[!NOTE]
>
>As [credenciais inseridas no Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

## Posso iniciar uma sincronização de oportunidade? {#can-i-initiate-an-opportunity-sync}

Não, não pode. As alterações em qualquer oportunidade no Salesforce serão sincronizadas com o Marketo automaticamente.

## O Marketo oferece suporte a mais de uma moeda no Valor da oportunidade? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Não, o Marketo oferece suporte a apenas uma moeda. O valor da oportunidade será sincronizado do Salesforce, mas a moeda será a [moeda padrão](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription){target="_blank"} na sua assinatura do Marketo.

## Como o Marketo associa oportunidades e contatos? {#how-does-marketo-associate-opportunities-and-contacts}

A Marketo associa oportunidades e contatos usando [Funções de contato da oportunidade](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Oportunidades sem Funções de contato atribuídas serão sincronizadas com a Marketo, mas não pertencerão a ninguém. Por exemplo, a pessoa não qualificará o filtro Tem oportunidade.

## Como posso ver todas as oportunidades de uma pessoa? {#how-can-i-see-all-the-opportunities-of-a-person}

Você pode exibir uma lista de oportunidades na guia **Informações da oportunidade** na página [Detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Quais são os acionadores/filtros relacionados à oportunidade? {#what-are-the-triggers-filters-related-to-opportunity}

Gatilhos:

* Adicionado à oportunidade
* Removido da oportunidade
* A oportunidade é atualizada

Filtros:

* Possui oportunidade
* A oportunidade foi atualizada/A oportunidade não foi atualizada
* Foi adicionado à oportunidade/Não foi adicionado à oportunidade
* Foi removido da oportunidade/Não foi removido da oportunidade
* Valor total da oport
* Número de oport
* Receita total esperada da oport

>[!TIP]
>
>Verifique as restrições em filtros e acionadores. Muitos detalhes legais lá dentro.
>
>Crie um novo campo no objeto de oportunidade no Salesforce e ele se tornará automaticamente uma restrição!
