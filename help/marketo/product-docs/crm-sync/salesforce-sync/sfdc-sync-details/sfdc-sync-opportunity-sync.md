---
unique-page-id: 2953467
description: SFDC Sync - Sincronização de oportunidade - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de oportunidade
exl-id: f8acc528-c631-43f0-8899-2f3c6fdabe9e
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 8%

---

# Sincronização do SFDC: sincronização de oportunidade {#sfdc-sync-opportunity-sync}

## Como os detalhes da oportunidade são mantidos em sincronia entre os dois sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

A sincronização é unidirecional: de [!DNL Salesforce] para Marketo. As atualizações de oportunidades no [!DNL Salesforce] serão sincronizadas com o Marketo.

>[!NOTE]
>
>As [credenciais inseridas no Marketo para [!DNL Salesforce]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

## Posso iniciar uma sincronização de oportunidade? {#can-i-initiate-an-opportunity-sync}

Não, não pode. As alterações em qualquer oportunidade no [!DNL Salesforce] serão sincronizadas com o Marketo automaticamente.

## O Marketo oferece suporte a mais de uma moeda no Valor da oportunidade? {#does-marketo-support-more-than-one-currency-in-the-opportunity-amount}

Não, o Marketo oferece suporte a apenas uma moeda. O valor da oportunidade será sincronizado de [!DNL Salesforce], mas a moeda será a [moeda padrão](/help/marketo/product-docs/administration/settings/set-default-location-settings-for-a-subscription.md#set-the-default-currency-settings-for-a-subscription) na sua assinatura do Marketo.

## Como o Marketo associa oportunidades e contatos? {#how-does-marketo-associate-opportunities-and-contacts}

A Marketo associa oportunidades e contatos usando [Funções de contato da oportunidade](https://help.salesforce.com/HTViewHelpDoc?id=contactroles.htm){target="_blank"}. Oportunidades sem Funções de contato atribuídas serão sincronizadas com a Marketo, mas não pertencerão a ninguém. Por exemplo, a pessoa não qualificará o filtro Tem oportunidade.

## Como posso ver todas as oportunidades de uma pessoa? {#how-can-i-see-all-the-opportunities-of-a-person}

Você pode exibir uma lista de oportunidades na guia **[!UICONTROL Informações da oportunidade]** na página [Detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

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
>Basta criar um novo campo no objeto de oportunidade em [!DNL Salesforce] e ele se tornará automaticamente uma restrição!
