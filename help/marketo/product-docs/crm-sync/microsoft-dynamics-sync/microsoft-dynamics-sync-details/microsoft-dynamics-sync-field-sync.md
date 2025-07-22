---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronização de campo - Documentação do Marketo - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de campo
exl-id: 78eef0eb-4086-45c5-bce3-a3399016f228
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# Sincronização de [!DNL Microsoft Dynamics]: Sincronização de Campo {#microsoft-dynamics-sync-field-sync}

A sincronização do Marketo com o [!DNL Dynamics] é super poderosa. Aqui estão os detalhes.

## Como os detalhes de campo são mantidos em sincronia entre os dois sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional para entidades de lead e contato. Se você fizer alterações em um cliente potencial ou contato no [!DNL Dynamics] ou em uma pessoa no Marketo, suas atualizações serão refletidas em ambos os sistemas.

Para contas, usuários, oportunidades, equipes e entidades personalizadas, a sincronização é unidirecional: [!DNL Dynamics] ao Marketo. Se você fizer alterações nessas entidades no [!DNL Dynamics], suas atualizações serão refletidas no Marketo.

## E se forem feitas alterações no mesmo campo, em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, o Marketo vencerá para as pessoas (clientes potenciais) e o [!DNL Dynamics] vencerá para os contatos. Isso ocorre porque consideramos que o departamento de marketing tem autoridade para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM). Para entidades de sincronização unidirecional, [!DNL Dynamics] sempre vencerá.

## Posso criar um campo no [!DNL Dynamics] usando o Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Não, não há suporte no momento.

## Criei um campo em [!DNL Dynamics]. Posso sincronizá-la com o Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sim, você pode [sincronizar o campo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync), desde que o usuário de sincronização tenha acesso a ele em [!DNL Dynamics].

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a instalação.

## E se for necessário adicionar um campo personalizado depois que o Marketo e o [!DNL Dynamics] forem sincronizados? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

Você pode adicionar campos a qualquer momento e esperar que os dados sejam atualizados de [!DNL Dynamics] para o Marketo. Consulte [Usar sincronização rápida com [!DNL Microsoft Dynamics] para obter um Novo campo personalizado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) para obter detalhes.

## E se eu quiser excluir um campo em [!DNL Dynamics] depois que ele for adicionado à sincronização? {#what-if-i-want-to-delete-a-field-in-dynamics-after-the-field-has-been-added-to-sync}

O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo em [!DNL Dynamics], recomendamos fazê-lo com a [sincronização desabilitada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando os [Selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).
