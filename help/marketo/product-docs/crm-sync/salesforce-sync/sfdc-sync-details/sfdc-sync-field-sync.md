---
unique-page-id: 2953461
description: Sincronização SFDC - Sincronização de campo - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de campo
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de campo {#sfdc-sync-field-sync}

O Marketo sincroniza informações de campo do Salesforce. Aqui estão os detalhes.

## Quais campos são sincronizados? {#which-fields-are-synced}

Sincronizamos a maioria dos campos padrão no SFDC e qualquer campo personalizado que o usuário da sincronização tenha permissão para ver.

## Como determinar se um registro no Marketo é um líder ou um contato no Salesforce? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Temos um campo em Marketo chamado SFDC Type. Ele tem três valores possíveis: chumbo, contato ou está vazio. Se estiver vazio, significa que este líder de marketing não existe no SFDC.

## Como determinar se um cliente potencial ou contato é excluído no SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Temos um campo em Marketo chamado SFDC isDeleted. Se o valor for verdadeiro, o cliente potencial foi excluído no SFDC.

## Como faço para garantir que um novo campo que adiciono no SFDC também seja adicionado ao Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Se você quiser um campo em ambos os sistemas, crie-o primeiro no SFDC e ele será automaticamente sincronizado para o Marketo.

Se você adicionar um novo campo no SFDC e o usuário de sincronização tiver permissão para vê-lo, ele será automaticamente adicionado ao Marketo.

## E se eu alterar uma etiqueta de campo no SFDC? {#what-if-i-change-a-field-label-in-sfdc}

Alterar o rótulo do campo no SFDC não afeta o rótulo do campo no Marketo.

## E se eu alterar um tipo de campo no SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Quando você altera um tipo de campo, Marketo exclui os dados nos campos se eles não corresponderem (mas exibe primeiro um aviso). Para preservar os dados, exporte-os e volte a importá-los depois de alterar o tipo de campo.

## E se eu alterar um nome de API no SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Se você alterar o nome da API de um campo no SFDC, um novo campo será criado no Marketo.

## O que acontece se eu adicionar um novo valor de lista de opções no SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Se um novo valor de lista de seleção for adicionado no SFDC a um campo, o Marketo enviará uma notificação.

## E os campos de pesquisa personalizados SFDC? {#what-about-custom-sfdc-lookup-fields}

Os campos de pesquisa no SFDC sincronizam a ID, mas não o nome referenciado.

## E os campos de fórmula SFDC? {#what-about-sfdc-formula-fields}

Os campos de fórmula são sincronizados, no entanto, as atualizações às referências na fórmula não são sincronizadas até que haja uma atualização para um carimbo [de modo do](https://help.salesforce.com/apex/HTViewSolution?id=000193203&amp;language=en_US)sistema.

## O que acontece quando eu excluo um campo do Salesforce que era sincronizado anteriormente com o Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Se você excluir um campo no SFDC, ele não excluirá automaticamente o campo no Marketo, ele apenas interrompe a sincronização.
