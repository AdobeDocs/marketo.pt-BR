---
unique-page-id: 2953459
description: Sincronização SFDC - Sincronização de conta - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de Conta
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de conta {#sfdc-sync-account-sync}

O Marketo também sincroniza as informações de sua conta com o Salesforce. Aqui estão algumas coisas específicas que você deveria saber!

## De que forma as informações são sincronizadas? {#which-way-does-the-information-sync}

Apenas de uma maneira: da SFDC para Marketo.

## Como as atualizações funcionam? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, ele alterará os valores de todos os contatos que pertencem a essa conta no Marketo. Não sincroniza com SFDC. No entanto, da próxima vez que a conta for atualizada no SFDC, as alterações substituirão todas as informações da conta no Marketo.

## Um contato pode pertencer a várias contas?  {#can-a-contact-belong-to-multiple-accounts}

Não. Uma conta pode ter muitos contatos, um contato pode ter apenas uma conta.

## Posso criar contas do Marketo? {#can-i-create-accounts-from-marketo}

Na maioria das vezes, não. No entanto, se você usar a etapa de fluxo [Converter pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) em uma pessoa, ela criará um novo Contato, uma nova Conta e uma nova Oportunidade.

>[!CAUTION]
>
>Esta etapa de fluxo tem um caso de uso muito limitado. Se você não tem certeza, provavelmente não deveria usá-lo.

## Uma alteração em um campo de conta no Salesforce resulta em um log de Atividade de valores de dados de alteração para cada contato?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Na maioria das vezes, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no SFDC, nós sincronizaremos a alteração, mas não registraremos a atividade dos mais de 5.000 contatos.
