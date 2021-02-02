---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronização de campo - Documentos do Marketing - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de campo
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização de campo {#microsoft-dynamics-sync-field-sync}

A sincronização de marketing com o Dynamics é super poderosa. Aqui estão os detalhes.

## Como os detalhes de campo são mantidos em sincronia entre os dois sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional para entidades de lead e contato. Se você fizer alterações em um cliente potencial ou contato no Dynamics ou em uma pessoa no Marketing Cloud, suas atualizações serão refletidas em ambos os sistemas.

Para entidades de conta, usuário, oportunidade, equipe e personalizadas, a sincronização é unidirecional: Dinâmica para o Marketo. Se você fizer alterações nessas entidades no Dynamics, suas atualizações serão refletidas no Marketo.

## E se forem feitas alterações no mesmo campo em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora seja raro, o Marketo ganhará por pessoas (clientes potenciais) e o Dynamics ganhará por contatos. Isso porque consideramos o departamento de marketing autoritativo para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM). Para entidades de sincronização unidirecionais, o Dynamics sempre ganhará.

## É possível criar um campo no Dynamics usando o Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Não, isso não é suportado no momento.

## Criei um campo no Dynamics. Posso sincronizá-lo com o Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sim, você pode [sincronizar o campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) desde que o usuário de sincronização tenha acesso a ele no Dynamics.

Quais campos serão sincronizados com o Marketo?

Você pode [selecionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante a configuração.

## E se eu precisar adicionar um campo personalizado após a sincronização do Marketo e do Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

É possível adicionar campos a qualquer momento e esperar que os dados sejam atualizados do Dynamics para o Marketing. Consulte [Usar sincronização rápida com o Microsoft Dynamics para obter um novo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obter detalhes.
