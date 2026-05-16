---
unique-page-id: 2953461
description: Saiba mais sobre quais campos do Salesforce são sincronizados com o Marketo e como o SFDC Type e isDeleted funcionam. Adicione novos campos no Salesforce primeiro, para que eles sejam sincronizados com o Marketo automaticamente.
title: Sincronização do SFDC - Sincronização de campo
exl-id: fbd66829-53cb-47fd-a530-149d12baee0e
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/XUKJC6x2gIjkd3wkmeIMKISxR0jBaGu5vHg7ystMI6c
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 0%

---

# Sincronização do SFDC: sincronização de campos {#sfdc-sync-field-sync}

O Marketo sincroniza informações de campo de [!DNL Salesforce]. Aqui estão os detalhes.

## Quais campos são sincronizados? {#which-fields-are-synced}

Sincronizamos a maioria dos campos padrão no SFDC e qualquer campo personalizado que o usuário de sincronização tenha permissão para ver.

## Como você determina se um registro no Marketo é um cliente potencial ou um contato no [!DNL Salesforce]? {#how-do-you-determine-if-a-record-in-marketo-is-a-lead-or-a-contact-in-salesforce}

Temos um campo no Marketo chamado SFDC Type. Ela tem três valores possíveis: lead, contact ou está vazia. Se estiver vazio, significa que esse lead do Marketo não existe no SFDC.

## Como você determina se um cliente em potencial ou contato é excluído no SFDC? {#how-do-you-determine-if-a-lead-or-contact-is-deleted-in-sfdc}

Temos um campo no Marketo chamado SFDC isDeleted. Se o valor for true, o lead foi excluído no SFDC.

## Como posso garantir que um novo campo que adiciono no SFDC também seja adicionado ao Marketo? {#how-do-i-make-sure-a-new-field-i-add-in-sfdc-also-gets-added-to-marketo}

>[!TIP]
>
>Se quiser um campo em ambos os sistemas, crie-o primeiro no SFDC e ele será sincronizado automaticamente com o Marketo.

Se você adicionar um novo campo no SFDC e o usuário de sincronização tiver permissão para visualizá-lo, ele será adicionado automaticamente ao Marketo.

## E se eu alterar um rótulo de campo no SFDC? {#what-if-i-change-a-field-label-in-sfdc}

Alterar o rótulo do campo no SFDC não afeta o rótulo do campo no Marketo.

## E se eu alterar um tipo de campo no SFDC? {#what-if-i-change-a-field-type-in-sfdc}

Quando você altera um tipo de campo, o Marketo exclui os dados nos campos se eles não corresponderem (mas primeiro exibe um aviso). Para preservar os dados, exporte-os e reimporte-os depois de alterar o tipo de campo.

## E se eu alterar um nome de API no SFDC? {#what-if-i-change-an-api-name-in-sfdc}

Se você alterar o nome da API de um campo no SFDC, um novo campo será criado no Marketo.

## O que acontece se eu adicionar um novo valor de lista de opções no SFDC? {#what-happens-if-i-add-a-new-picklist-value-in-sfdc}

Se um novo valor de lista de opções for adicionado no SFDC a um campo, o Marketo enviará uma notificação.

## E os campos de pesquisa personalizados do SFDC? {#what-about-custom-sfdc-lookup-fields}

Os campos de pesquisa no SFDC sincronizam a ID, mas não o nome referenciado.

## E os Campos de Fórmula do SFDC? {#what-about-sfdc-formula-fields}

Os campos de fórmula são sincronizados, no entanto, as atualizações para as referências na fórmula não são sincronizadas até que haja uma atualização para um [Carimbo de Modo do Sistema](https://help.salesforce.com/apex/HTViewSolution?id=000193203&language=en_US){target="_blank"}.

## O que acontece quando eu excluo um campo do [!DNL Salesforce] que estava sincronizando anteriormente com o Marketo? {#what-happens-when-i-delete-a-field-from-salesforce-that-was-previously-syncing-with-marketo}

Se você excluir um campo no SFDC, ele não excluirá automaticamente o campo no Marketo. Ele apenas interrompe a sincronização.
