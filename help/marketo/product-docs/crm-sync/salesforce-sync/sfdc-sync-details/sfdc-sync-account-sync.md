---
unique-page-id: 2953459
description: Sincronização SFDC - Sincronização de Conta - Documentos do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Conta
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Sincronização SFDC: Sincronização de conta {#sfdc-sync-account-sync}

A Marketo também sincroniza suas informações de conta com o Salesforce. Aqui estão algumas coisas específicas que você deveria saber!

## Como as informações são sincronizadas? {#which-way-does-the-information-sync}

Apenas uma maneira: do SFDC para o Marketo.

## Como funcionam as atualizações? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, ele alterará os valores de todos os contatos pertencentes a essa conta no Marketo. Ele não sincroniza com o SFDC. No entanto, na próxima vez que a conta for atualizada no SFDC, as alterações substituirão todas as informações da conta no Marketo.

## Um contato pode pertencer a várias contas?  {#can-a-contact-belong-to-multiple-accounts}

Nº Uma conta pode ter muitos contatos. Um contato pode ter apenas uma conta.

## Posso criar contas no Marketo? {#can-i-create-accounts-from-marketo}

Na maioria das vezes, não. No entanto, se você usar a etapa de fluxo [Converter Pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) em uma pessoa, ela criará um novo Contato, uma nova Conta e uma nova Oportunidade.

>[!CAUTION]
>
>Essa etapa de fluxo tem um caso de uso muito limitado. Se você não tem certeza, provavelmente não deveria usá-lo.

## Uma alteração em um Campo de conta no Salesforce resulta em um Log de atividade de alteração de valor de dados para cada contato?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Na maioria das vezes, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no SFDC, sincronizamos a alteração, mas não registramos a atividade para mais de 5.000 contatos.
