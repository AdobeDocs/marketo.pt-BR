---
unique-page-id: 2953463
description: Sincronização SFDC - Sincronização de Cliente Potencial/Conta - Documentos Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Cliente Potencial/Conta
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# Sincronização SFDC: Sincronização de Cliente Potencial/Conta {#sfdc-sync-lead-account-owner-sync}

Eles estão sincronizando tecnicamente a tabela de &quot;usuário&quot; no Salesforce, no entanto, nos referiremos a ela como campos de Lead/Proprietário da conta.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Para cada pessoa sincronizada com o Marketo, também sincronizamos os seguintes campos de proprietário:

* Nome do proprietário das vendas
* Sobrenome do proprietário das vendas
* Título do Proprietário de Vendas
* Telefone do proprietário das vendas
* Endereço de e-mail do proprietário das vendas

Para cada contato, sincronizamos os cinco campos de proprietários de clientes potenciais acima, bem como estes campos de proprietários de contas:

* Nome do proprietário da conta
* Sobrenome do proprietário da conta
* Endereço de e-mail do proprietário da conta

## Posso alterar o proprietário do cliente potencial no Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolutamente, use o [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) ação de fluxo.

>[!NOTE]
>
>Não é possível alterar as informações do proprietário usando o [Usando a Página de detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## O que posso fazer com esses dados? {#what-can-i-do-with-this-data}

Há muitas razões para usar esses dados, como

* Enviar um email personalizado com assinatura do proprietário das vendas
* Filtrar relatórios de vendas específicos para marketing ou até mesmo analisar a eficácia
* Regras de atribuição (e reatribuição) no Marketo
* Use-os na [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizar pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)e [Criar tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ações de fluxo

A Marketo tem uma sincronização do Salesforce incrível. Ninguém mais faz tão bem!
