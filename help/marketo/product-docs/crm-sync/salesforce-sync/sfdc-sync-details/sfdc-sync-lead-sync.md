---
unique-page-id: 2953455
description: Sincronização SFDC - Sincronização de lead - Documentos do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Chumbo
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Sincronização SFDC: Sincronização de lead {#sfdc-sync-lead-sync}

Você conhecia sincronizações do Marketo de seu banco de dados do Salesforce? Ele sincroniza, aguarda 5 minutos e sincroniza novamente. Todo dia, todos os dias. Aqui estão alguns detalhes sobre como a Marketo trata o Salesforce leads especificamente.

## Sincronizar Direção {#sync-direction}

O lead (pessoa) e a sincronização de contato são bidirecionais. Se você fizer alterações em um registro no Salesforce ou no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se as alterações forem feitas em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo ganha. É raro que esse tipo de colisão de dados ocorra.

## Posso criar um lead no Salesforce usando o Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sim, use a ação de fluxo [Sincronizar Pessoa com SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Isso criará um lead no Salesforce se o lead não existir.

## Posso forçar manualmente uma sincronização de uma pessoa no Marketo a um lead no Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sim, use a ação de fluxo [Sincronizar Pessoa com SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) e ela será sincronizada em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário de sincronização do Salesforce tem acesso.

## A Marketo respeitará as regras de validação do Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou faltando informações de campo necessárias. A Marketo registrará o resultado no registro de atividades de leads, se isso ocorrer.
