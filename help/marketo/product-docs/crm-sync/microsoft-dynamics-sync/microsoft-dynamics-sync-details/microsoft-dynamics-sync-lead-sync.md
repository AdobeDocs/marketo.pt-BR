---
unique-page-id: 3571848
description: Sincronização do Microsoft Dynamics - Sincronização de clientes potenciais - Documentos do Marketo - Documentação do produto
title: Sincronização do Microsoft Dynamics - Sincronização de clientes potenciais
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Sincronização do Microsoft Dynamics: Sincronização de lead {#microsoft-dynamics-sync-lead-sync}

A sincronização do Marketo com o Dynamics é super poderosa. Veja os detalhes:

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional. Se você fizer alterações em um cliente potencial no Dynamics ou em uma pessoa no Marketo, sua atualização será refletida em ambos os sistemas.

>[!NOTE]
>
>As exclusões nem sempre são sincronizadas automaticamente em ambas as direções. Consulte [Excluindo um Lead ou Contato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## E se forem feitas alterações no mesmo campo em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, a Marketo ganhará por pessoas (leads) e o Dynamics ganhará por contatos. Isso ocorre porque consideramos que o departamento de marketing é autoritativo para as pessoas, enquanto o sistema oficial de registro para contatos está no departamento de vendas (CRM).

## Posso criar um lead no Dynamics usando o Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sim, use a ação de fluxo [Sincronizar Pessoa com Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Isso criará um lead no Dynamics se o lead não existir. Se o lead existir, a etapa do fluxo não executará nenhuma ação.

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;Sincronizar pessoa com a Microsoft&quot; (somente em uma campanha de acionador), o lead/contato será criado em tempo real no Dynamics.

## Posso forçar manualmente uma sincronização de uma pessoa do Marketo a um cliente potencial no Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Não, a sincronização automatizada em segundo plano é a única maneira de sincronizar atualizações entre o Marketo e o Dynamics. A ação de fluxo [Sync Person to Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) não forçará uma sincronização do lead.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante a configuração.

## O Marketo respeitará as regras de validação do Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou faltando informações de campo necessárias. O Marketo registrará o resultado no registro de atividades da pessoa, se isso ocorrer.
