---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Sincronização de Chumbo - Documentos do Marketing - Documentação do Produto
title: Microsoft Dynamics Sync - Sincronização de cliente potencial
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização de cliente potencial {#microsoft-dynamics-sync-lead-sync}

A sincronização de marketing com o Dynamics é super poderosa. Estes são os detalhes:

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional. Se você fizer alterações em um cliente potencial no Dynamics ou em uma pessoa no Marketing, sua atualização será refletida em ambos os sistemas.

>[!NOTE]
>
>As exclusões nem sempre são sincronizadas automaticamente em ambas as direções. Consulte [Excluindo um cliente potencial ou Contato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## E se forem feitas alterações no mesmo campo em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora seja raro, o Marketo ganhará por pessoas (clientes potenciais) e o Dynamics ganhará por contatos. Isso porque consideramos o departamento de marketing autoritativo para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM).

## Posso criar uma perspectiva de venda no Dynamics usando o Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sim, use a ação de fluxo [Sincronizar Pessoa com Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Isso criará um cliente potencial no Dynamics se o cliente potencial não existir. Se o cliente potencial existir, a etapa de fluxo não executará nenhuma ação.

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;Sincronizar Pessoa com a Microsoft&quot; (somente em uma campanha de disparo), o cliente potencial/contato será criado em tempo real no Dynamics.

## Posso forçar manualmente uma sincronização de uma pessoa da Marketo para uma liderança na Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Não, a sincronização em segundo plano automatizada é a única maneira de sincronizar atualizações entre o Marketo e o Dynamics. A ação de fluxo [Sincronizar Pessoa com Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) não forçará uma sincronização do cliente potencial.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante a configuração.

## O Marketo respeitará as regras de validação do Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou se não houver informações de campo necessárias. O Marketo registrará o resultado no Registro de Atividades da pessoa, se isso acontecer.
