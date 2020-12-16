---
unique-page-id: 2953455
description: Sincronização SFDC - Sincronização líder - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de cliente potencial
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de cliente potencial {#sfdc-sync-lead-sync}

Você sabia que o Marketo sincroniza com seu banco de dados Salesforce? Sincroniza, aguarda 5 minutos e sincroniza novamente. O dia todo, todos os dias. Aqui estão alguns detalhes sobre como o Marketo trata o Salesforce especificamente.

## Sincronizar direção {#sync-direction}

O cliente potencial (pessoa) e a sincronização de contato são bidirecionais. Se você fizer alterações em um registro no Salesforce ou no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se as mudanças forem feitas em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo ganha. É raro que esse tipo de colisão de dados ocorra.

## Posso criar uma perspectiva de venda no Salesforce usando o Marketo? {#can-i-create-a-lead-in-salesforce-using-marketo}

Sim, use a ação de fluxo [Sincronizar Pessoa com SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) . Isso criará uma oportunidade potencial no Salesforce se a oportunidade não existir.

## Posso forçar manualmente uma sincronização de uma pessoa em Marketo para uma liderança em Salesforce? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Sim, use a ação de fluxo [Sincronizar Pessoa com SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) e ela será sincronizada em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário de sincronização do Salesforce tem acesso.

## O Marketo respeitará as regras de validação do Salesforce? {#will-marketo-respect-the-salesforce-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou se não houver informações de campo necessárias. Se isso acontecer, o Marketo registrará o resultado no Registro de Atividades de clientes potenciais.
