---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronização de campo - Documentos do Marketo - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de campo
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronização de campo {#microsoft-dynamics-sync-field-sync}

A sincronização do Marketo com o Dynamics é super poderosa. Aqui estão os detalhes.

## Como os detalhes do campo são mantidos em sincronia entre os dois sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional para entidades de cliente potencial e de contato. Se você fizer alterações em um lead ou contato no Dynamics ou em uma pessoa no Marketo, suas atualizações serão refletidas em ambos os sistemas.

Para entidades de conta, usuário, oportunidade, equipe e personalizadas, a sincronização é unidirecional: Dinâmica para o Marketo. Se você fizer alterações nessas entidades no Dynamics, suas atualizações serão refletidas no Marketo.

## E se forem feitas alterações no mesmo campo em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, a Marketo ganhará por pessoas (leads) e o Dynamics ganhará por contatos. Isso ocorre porque consideramos que o departamento de marketing é autoritativo para as pessoas, enquanto o sistema oficial de registro para contatos está no departamento de vendas (CRM). Para entidades de sincronização unidirecionais, o Dynamics sempre ganhará.

## Posso criar um campo no Dynamics usando o Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Não, isso não é compatível no momento.

## Criei um campo no Dynamics. Posso sincronizá-lo com o Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sim, você pode [sincronizar o campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) desde que o usuário de sincronização tenha acesso a ele no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos a serem sincronizados](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) durante a configuração.

## E se eu precisar adicionar um campo personalizado depois que o Marketo e o Dynamics forem sincronizados? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Você pode adicionar campos a qualquer momento e esperar que os dados sejam atualizados do Dynamics para Marketo. Consulte [Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obter detalhes.

## E se eu quiser excluir um campo no Dynamics depois que o campo for adicionado à sincronização? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazer isso com a variável [sincronização desativada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando o [Selecionar Campos para Sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
