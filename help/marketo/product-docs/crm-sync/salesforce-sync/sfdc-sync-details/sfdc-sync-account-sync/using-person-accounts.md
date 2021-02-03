---
unique-page-id: 4719316
description: Usar contas pessoais - Documentos do marketing - Documentação do produto
title: Usando Contas de Pessoa
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Usando contas pessoais {#using-person-accounts}

As contas pessoais podem ser configuradas no Salesforce para atender às necessidades de sua organização. É assim que o Marketo trata as contas pessoais.

>[!NOTE]
>
>As contas padrão do Salesforce são contas comerciais. Seu administrador do Salesforce precisa configurar contas pessoais separadamente.

## O que é uma conta de pessoa? {#what-is-a-person-account}

Uma conta de pessoa é muito semelhante ao objeto de conta no Salesforce. No entanto, uma conta de pessoa tem acesso aos campos de conta e de contato.

## O que acontece quando uma conta pessoal é sincronizada com o Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Uma conta de pessoa é sincronizada ao Marketo como uma empresa e como uma pessoa.

>[!NOTE]
>
>Os campos personalizados de uma conta pessoal são copiados para a empresa e para a pessoa no Marketo.

## Como faço para diferenciar contas de negócios e contas pessoais? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Use o filtro **Conta pessoal** na sua lista inteligente para separar as contas pessoais das contas comerciais padrão.

## Onde as informações de contas pessoais são exibidas no Marketing Insight de Vendas? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Atividades relacionadas a contas pessoais são exibidas no painel **Conta**.

>[!NOTE]
>
>As opções de **Adicionar à Campanha do Marketing Insight** e **Enviar e-mail** não estão disponíveis atualmente para contas pessoais.

## Como associo oportunidades a uma conta de pessoa? {#how-do-i-associate-opportunities-to-a-person-account}

O Marketo depende da função de contato de oportunidade para determinar a pessoa à qual associar a oportunidade. É necessário adicionar a função de contato de oportunidade para cada conta de pessoa para conectar a oportunidade à pessoa adequada no Marketo. Recomendamos que você configure um fluxo de trabalho para adicionar a função de contato de oportunidade automaticamente.

## Qual campo de email devo usar para contas pessoais? {#which-email-field-should-i-use-for-person-accounts}

Há dois campos de email para uma conta de pessoa. Use o campo **Endereço de email** em seus formulários (não o **Endereço de email da pessoa**) para garantir que a eliminação da duplicação do Marketo e outros tipos de processamento de email funcionem corretamente.
