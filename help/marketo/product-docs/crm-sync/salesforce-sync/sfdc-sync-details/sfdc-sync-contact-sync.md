---
unique-page-id: 2953457
description: Sincronização SFDC - Sincronização de Contato - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de Contato
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de contato {#sfdc-sync-contact-sync}

Você sabia que o Marketo sincroniza todo seu banco de dados com o Salesforce? Sincroniza, então aguarda 5 minutos e sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketing trata especificamente os Contatos do Salesforce.

## Sincronizar direção {#sync-direction}

A sincronização de contato é bidirecional. Se você fizer alterações em um contato no Salesforce ou no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se as mudanças forem feitas em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Somos legais e deixamos Salesforce ganhar. É raro que esse tipo de colisão de dados ocorra.

## Posso converter uma pessoa em um contato no Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sim, use a ação de fluxo ** [Converter pessoa](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**.

>[!CAUTION]
>
>A conversão de uma pessoa no Marketo resultará em uma nova conta e oportunidade no Salesforce. Se você não quiser contas de duplicado, use o Salesforce para converter.

## Posso forçar manualmente uma sincronização de um contato? {#can-i-manually-force-a-sync-of-a-contact}

Sim, use a ação ** [Sincronizar Pessoa com SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **flow e ela será sincronizada em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais seu usuário de sincronização de marketing tem acesso.

## O Marketo respeitará as regras de validação do Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sim, se houver um conflito, registrará o resultado no Registro de Atividades de clientes potenciais.
