---
unique-page-id: 2953457
description: Sincronização do SFDC - Sincronização de contatos - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de Contatos
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Sincronização do SFDC: Sincronização de Contatos {#sfdc-sync-contact-sync}

Você sabia que o Marketo Engage sincroniza todo o seu banco de dados com o Salesforce? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketo trata os contatos do Salesforce especificamente.

## Direção da sincronização {#sync-direction}

A sincronização de contatos é bidirecional. Se você fizer alterações em um contato no Salesforce ou no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se forem feitas alterações em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Somos bons e deixamos a Salesforce ganhar. É raro ocorrer esse tipo de colisão de dados.

## Posso converter uma pessoa em um contato no Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sim, use a ação de fluxo **[Converter pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>A conversão de uma pessoa no Marketo resultará em uma nova conta e oportunidade no Salesforce. Se você não quiser contas duplicadas, use o Salesforce para converter.

## Posso forçar manualmente uma sincronização de um contato? {#can-i-manually-force-a-sync-of-a-contact}

Sim, use a ação de fluxo **[Sincronizar Pessoa com SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** e ela será sincronizada em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário do Marketo Sync tem acesso.

## O Marketo respeitará as regras de validação do Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sim, se houver um conflito, ele registrará o resultado no Registro de atividades dos clientes potenciais.
