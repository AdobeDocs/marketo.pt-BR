---
unique-page-id: 2953455
description: Sincronização SFDC - Sincronização de clientes potenciais - Documentação do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de clientes potenciais
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# Sincronização SFDC: sincronização de clientes potenciais {#sfdc-sync-lead-sync}

Você sabia sincronizações de Marketo Engage do banco de dados do Salesforce? Ele sincroniza, aguarda 5 minutos e sincroniza novamente. O dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketo trata os clientes potenciais do Salesforce especificamente.

## Direção da sincronização {#sync-direction}

A sincronização de lead (pessoa) e contato é bidirecional. Se você fizer alterações em um registro no Salesforce ou no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se forem feitas alterações em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo ganha. É raro ocorrer esse tipo de colisão de dados.

## Posso criar um cliente potencial no Salesforce usando o Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sim, use o [Sincronizar pessoa ao SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} ação de fluxo. Isso criará um cliente em potencial no Salesforce se o cliente em potencial não existir.

## Posso forçar manualmente uma sincronização de uma pessoa no Marketo para um cliente potencial no Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sim, use o [Sincronizar pessoa ao SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} fluxo e será sincronizado em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais seu usuário de sincronização do Salesforce tem acesso.

## O Marketo respeitará as regras de validação do Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou se faltarem informações de campo obrigatórias. O Marketo registrará o resultado no registro de atividades de clientes potenciais se isso acontecer.
