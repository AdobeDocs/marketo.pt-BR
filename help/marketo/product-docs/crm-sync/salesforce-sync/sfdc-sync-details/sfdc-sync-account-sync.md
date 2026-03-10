---
unique-page-id: 2953459
description: Saiba mais sobre como as informações da conta são sincronizadas do Salesforce para o Marketo. Entenda a sincronização unidirecional, o relacionamento de conta de contato e a criação de contas por meio da opção Converter pessoa.
title: SFDC Sync - Sincronização de conta
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 2%

---

# Sincronização do SFDC: sincronização de conta {#sfdc-sync-account-sync}

O Marketo também sincroniza as informações da sua conta com o [!DNL Salesforce]. Aqui estão algumas coisas específicas que você deve saber!

## De que forma as informações são sincronizadas? {#which-way-does-the-information-sync}

Somente uma maneira: do SFDC para o Marketo.

## Como funcionam as atualizações? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, os valores de todos esses contatos que pertencem a essa conta serão alterados no Marketo. Ele não é sincronizado com o SFDC. No entanto, na próxima vez que a conta for atualizada no SFDC, as alterações substituirão todas as informações da conta no Marketo.

## Um contato pode pertencer a várias contas?  {#can-a-contact-belong-to-multiple-accounts}

Não. Uma conta pode ter muitos contatos, um contato pode ter apenas uma conta.

## Posso criar contas a partir do Marketo? {#can-i-create-accounts-from-marketo}

Na maioria das vezes, não. No entanto, se você usar a etapa de fluxo [Converter pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} em uma pessoa, ela criará um novo Contato, uma nova Conta e uma nova Oportunidade.

>[!CAUTION]
>
>Essa etapa do fluxo tem um caso de uso muito limitado. Se você não tem certeza, provavelmente não deve usá-lo.

## Uma alteração em um Campo de Conta em [!DNL Salesforce] resulta em um Log de Atividade Alterar Valor de Dados para cada contato?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Principalmente, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no SFDC, nós sincronizamos a alteração, mas não registramos a atividade para os mais de 5.000 contatos.
