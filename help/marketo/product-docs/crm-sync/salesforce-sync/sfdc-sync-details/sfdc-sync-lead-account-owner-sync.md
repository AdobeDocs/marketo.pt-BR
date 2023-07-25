---
unique-page-id: 2953463
description: Sincronização do SFDC - Sincronização de cliente potencial/proprietário de conta - Documentação da Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de Cliente Potencial/Proprietário da Conta
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# Sincronização do SFDC: Sincronização de Cliente Potencial/Proprietário da Conta {#sfdc-sync-lead-account-owner-sync}

Eles estão sincronizando tecnicamente a tabela &quot;usuário&quot; no Salesforce, no entanto, nos referiremos a ela como campos de líder/proprietário de conta.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Para cada pessoa sincronizada com o Marketo, também sincronizamos os seguintes campos de proprietário:

* Nome do proprietário das vendas
* Sobrenome do proprietário das vendas
* Título do Proprietário de Vendas
* Telefone do proprietário das vendas
* Endereço de e-mail do proprietário das vendas

Para cada contato, sincronizamos os cinco campos de proprietário do lead acima, bem como estes campos de proprietário da conta:

* Nome do proprietário da conta
* Sobrenome do proprietário da conta
* Endereço de e-mail do proprietário da conta

## Posso alterar o proprietário do lead no Marketo? {#can-i-change-the-lead-owner-in-marketo}

Absolutamente, apenas use o [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) ação de fluxo.

>[!NOTE]
>
>Não é possível alterar as informações do proprietário usando o [Usando a Página Detalhes da Pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## O que posso fazer com esses dados? {#what-can-i-do-with-this-data}

Há vários motivos para usar esses dados, como

* Enviar um email personalizado com assinatura do proprietário das vendas
* Filtrar representantes de vendas específicos para marketing ou até mesmo analisar a eficácia
* Regras de atribuição (e reatribuição) no Marketo
* Use-as no [Alterar proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Sincronizar pessoa ao SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), e [Criar tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) ações de fluxo

O Marketo tem uma sincronização incrível do Salesforce. Ninguém mais faz tão bem!
