---
unique-page-id: 2953463
description: SFDC Sync - Sincronização de cliente potencial/proprietário de conta - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de cliente potencial/proprietário de conta
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 13%

---

# Sincronização da SFDC: sincronização do lead/proprietário da conta {#sfdc-sync-lead-account-owner-sync}

Eles estão sincronizando tecnicamente a tabela &quot;usuário&quot; em [!DNL Salesforce]. No entanto, nos referiremos a ela como campos de Líder/Proprietário da conta.

## Quais campos serão sincronizados com o Marketo Engage? {#which-fields-will-sync-to-marketo-engage}

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

Absolutamente, use a ação de fluxo [Alterar Proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}.

>[!NOTE]
>
>Não é possível alterar as informações do proprietário usando a [Página de Detalhes da Pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## O que posso fazer com esses dados? {#what-can-i-do-with-this-data}

Há vários motivos para usar esses dados, como

* Enviar um email personalizado com assinatura do proprietário das vendas
* Filtrar representantes de vendas específicos para marketing ou até mesmo analisar a eficácia
* Regras de atribuição (e reatribuição) no Marketo
* Use-os nas ações de fluxo [Alterar Proprietário](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Sincronizar Pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} e [Criar Tarefa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}

O Marketo tem uma sincronização [!DNL Salesforce] incrível. Ninguém mais faz tão bem!
