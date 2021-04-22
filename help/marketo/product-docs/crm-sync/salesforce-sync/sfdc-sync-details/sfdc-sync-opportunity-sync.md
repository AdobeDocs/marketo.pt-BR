---
unique-page-id: 2953467
description: Sincronização SFDC - Sincronização de Oportunidade - Documentos do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Oportunidades
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 4%

---

# Sincronização SFDC: Sincronização de Oportunidades {#sfdc-sync-opportunity-sync}

## Como os detalhes da oportunidade são mantidos em sincronia entre os dois sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

A sincronização é uma das maneiras: do Salesforce para o Marketo. As atualizações de oportunidades no Salesforce serão sincronizadas com o Marketo.

>[!NOTE]
>
>As credenciais [inseridas no Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

## Posso iniciar uma Sincronização de Oportunidades? {#can-i-initiate-an-opportunity-sync}

Não, não pode. As alterações em qualquer oportunidade no Salesforce serão sincronizadas automaticamente no Marketo.

## O Marketo suporta mais de uma moeda no Valor da Oportunidade? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Não, a Marketo suporta apenas uma moeda. O valor da oportunidade será sincronizado do Salesforce, mas a moeda será a [moeda padrão](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) na sua assinatura do Marketo.

## Como a Marketo associa oportunidades e contatos? {#how-does-marketo-associate-opportunities-and-contacts}

O Marketo associa Oportunidades e contatos usando [Funções de Contato de Oportunidade](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). As oportunidades sem quaisquer Funções de contato atribuídas serão sincronizadas com o Marketo, mas não pertencerão a ninguém. Por exemplo, a pessoa não qualificará o filtro Tem Oportunidade .

## Como posso ver todas as oportunidades de uma pessoa? {#how-can-i-see-all-the-opportunities-of-a-person}

Você pode exibir uma lista de oportunidades na guia **Informações da oportunidade** na página [Detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Quais são os acionadores/filtros relacionados à oportunidade? {#what-are-the-triggers-filters-related-to-opportunity}

Gatilhos:

* Adicionada à oportunidade
* Removido da oportunidade
* A oportunidade é atualizada

Filtros:

* Possui oportunidade
* A Oportunidade foi Atualizada/Não Oportunidade foi Atualizada
* Foi adicionado à Oportunidade/Não foi adicionado à Oportunidade
* Foi removido da Oportunidade/Não foi Removido da Oportunidade
* Valor total da oport.
* Número de oport.
* Receita total esperada da oport.

>[!TIP]
>
>Verifique as restrições em filtros e acionadores. Muitos detalhes legais lá dentro.
>
>Basta criar um novo campo no objeto de oportunidade no Salesforce e ele se tornará automaticamente uma restrição!
