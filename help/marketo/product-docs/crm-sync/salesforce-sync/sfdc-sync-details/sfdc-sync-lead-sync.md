---
unique-page-id: 2953455
description: SFDC Sync - Sincronização de clientes potenciais - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização com o lead
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Sincronização do SFDC: sincronização com o lead {#sfdc-sync-lead-sync}

Você sabia que o Marketo é sincronizado a partir do banco de dados [!DNL Salesforce]? Ele sincroniza, aguarda 5 minutos e sincroniza novamente. O dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente os clientes em potencial [!DNL Salesforce].

## Direção da sincronização {#sync-direction}

A sincronização de lead (pessoa) e contato é bidirecional. Se você fizer alterações em um registro no [!DNL Salesforce] ou no Marketo, suas atualizações serão refletidas nos dois sistemas.

## E se forem feitas alterações em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo ganha. É raro ocorrer esse tipo de colisão de dados.

## Posso criar um cliente em potencial no [!DNL Salesforce] usando o Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sim, use a ação de fluxo [Sincronizar Pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Isso criará um cliente em potencial em [!DNL Salesforce] se ele não existir.

## Posso forçar manualmente uma sincronização de uma pessoa no Marketo para um cliente potencial no [!DNL Salesforce]? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sim, use a ação de fluxo [Sincronizar Pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} e ela será sincronizada em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário de sincronização do [!DNL Salesforce] tem acesso.

## O Marketo respeitará as regras de validação [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou se faltarem informações de campo obrigatórias. O Marketo registrará o resultado no registro de atividades de clientes potenciais se isso acontecer.
