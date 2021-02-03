---
unique-page-id: 2953467
description: Sincronização SFDC - Sincronização de Oportunidade - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de Oportunidades
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de Oportunidade {#sfdc-sync-opportunity-sync}

## Como os detalhes da oportunidade são mantidos em sincronia entre os dois sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

A sincronização é unidirecional: de Salesforce a Marketo. As atualizações de oportunidades no Salesforce serão sincronizadas com o Marketing.

>[!NOTE]
>
>As credenciais [inseridas no Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

## Posso iniciar uma sincronização de oportunidade? {#can-i-initiate-an-opportunity-sync}

Não, você não pode. As alterações em qualquer oportunidade no Salesforce serão sincronizadas automaticamente no Marketing.

## O Marketing suporta mais de uma moeda na Quantia de Oportunidade? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Não, o Marketo suporta apenas uma moeda. O valor da oportunidade será sincronizado do Salesforce, mas a moeda será a [moeda padrão](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) na sua subscrição de marketing.

## Como o Marketo associa oportunidades e contatos? {#how-does-marketo-associate-opportunities-and-contacts}

O Marketo associa Oportunidades e contatos usando [Funções de Contato de Oportunidade](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm). Oportunidades sem quaisquer Funções de Contato atribuídas serão sincronizadas com o Marketo, mas não pertencerão a ninguém. Por exemplo, a pessoa não qualificará o filtro Tem oportunidade.

## Como posso ver todas as oportunidades de uma pessoa? {#how-can-i-see-all-the-opportunities-of-a-person}

Você pode visualização uma lista de oportunidades na guia **Informações da oportunidade** na página [Detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Quais são os acionadores/filtros relacionados à oportunidade? {#what-are-the-triggers-filters-related-to-opportunity}

Acionadores:

* Adicionada à oportunidade
* Removido da oportunidade
* A oportunidade é atualizada

Filtros:

* Tem oportunidade
* A oportunidade foi atualizada/A oportunidade não foi atualizada
* Foi adicionado à Oportunidade/Não foi adicionado à Oportunidade
* Foi removido da Oportunidade/Não foi removido da Oportunidade
* Valor Total da Opção
* Número de Ópticos
* Receita Esperada da Opção Total

>[!TIP]
>
>Verifique as restrições em filtros e acionadores. Muitos detalhes legais lá dentro.
>
>Basta criar um novo campo no objeto de oportunidade no Salesforce e ele se tornará automaticamente uma restrição!
