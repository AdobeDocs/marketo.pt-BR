---
unique-page-id: 2953459
description: Sincronização do SFDC - Sincronização da conta - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de Conta
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Sincronização do SFDC: Sincronização de Conta {#sfdc-sync-account-sync}

O Marketo Engage também sincroniza as informações de sua conta com o Salesforce. Aqui estão algumas coisas específicas que você deve saber!

## De que forma as informações são sincronizadas? {#which-way-does-the-information-sync}

Somente uma maneira: de SFDC para Marketo.

## Como funcionam as atualizações? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, os valores de todos esses contatos que pertencem a essa conta serão alterados no Marketo. Ele não é sincronizado com o SFDC. No entanto, na próxima vez que a conta for atualizada no SFDC, as alterações substituirão todas as informações da conta no Marketo.

## Um contato pode pertencer a várias contas?  {#can-a-contact-belong-to-multiple-accounts}

Não. Uma conta pode ter muitos contatos, um contato pode ter apenas uma conta.

## Posso criar contas a partir do Marketo? {#can-i-create-accounts-from-marketo}

Na maioria das vezes, não. No entanto, se você usar a variável [Converter pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} etapa de fluxo em uma pessoa, criará um novo Contato, uma nova Conta e uma nova Oportunidade.

>[!CAUTION]
>
>Essa etapa do fluxo tem um caso de uso muito limitado. Se você não tem certeza, provavelmente não deve usá-lo.

## Uma alteração em um campo Conta no Salesforce resulta em um registro de atividade Alterar valor de dados para cada contato?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Principalmente, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no SFDC, sincronizamos a alteração, mas não registramos a atividade dos mais de 5.000 contatos.
