---
unique-page-id: 2953463
description: Sincronização SFDC - Sincronização de cliente potencial/proprietário da conta - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de cliente potencial/proprietário da conta
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de cliente potencial/proprietário de conta {#sfdc-sync-lead-account-owner-sync}

Tecnicamente, eles estão sincronizando a tabela &quot;usuário&quot; no Salesforce, no entanto, nós a referenciaremos como campos de cliente potencial/proprietário da conta.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Para cada pessoa sincronizada com o Marketo, também sincronizamos os seguintes campos de proprietário:

* Nome do proprietário da venda
* Sobrenome do proprietário de vendas
* Título do proprietário de vendas
* Número de Telefone do Proprietário de Vendas
* Endereço de email do proprietário de vendas

Para cada contato, sincronizamos os cinco campos do proprietário principal acima, bem como estes campos do proprietário da conta:

* Nome do proprietário da conta
* Sobrenome do proprietário da conta
* Endereço de email do proprietário da conta

## Posso mudar o proprietário principal em Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolutamente, use a ação de fluxo [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>Não é possível alterar as informações do proprietário usando [Usando a Página de detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## O que posso fazer com esses dados? {#what-can-i-do-with-this-data}

Há muitas razões para usar esses dados, como

* Enviar um email personalizado com assinatura do proprietário das vendas
* Filtrar em representantes de vendas específicos para marketing ou até mesmo analisar a eficácia
* Regras de atribuição (e reatribuição) no Marketing
* Use-os nas ações de fluxo [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizar pessoa com SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) e [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)

Marketo tem uma incrível sincronização Salesforce. Ninguém mais faz tão bem!
