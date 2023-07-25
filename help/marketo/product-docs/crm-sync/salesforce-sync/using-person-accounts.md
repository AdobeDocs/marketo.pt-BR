---
unique-page-id: 4719316
description: Uso de contas de pessoas - Documentação do Marketo - Documentação do produto
title: Uso de contas de pessoas
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Uso de contas de pessoas {#using-person-accounts}

Contas de pessoas podem ser configuradas no Salesforce para atender às necessidades de sua organização. Veja como o Marketo trata contas pessoais.

>[!NOTE]
>
>As contas padrão do Salesforce são contas comerciais. Seu administrador do Salesforce precisa configurar contas pessoais separadamente.

## O que é uma conta de pessoa? {#what-is-a-person-account}

Uma conta de pessoa é muito semelhante ao objeto da conta no Salesforce. No entanto, uma conta de pessoa tem acesso aos campos de conta e de contato.

## O que acontece quando uma conta de pessoa é sincronizada com o Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Uma conta de pessoa é sincronizada com a Marketo como uma empresa e como uma pessoa.

>[!NOTE]
>
>Os campos personalizados de uma conta de pessoa são copiados para a empresa e para a pessoa no Marketo.

## Como posso diferenciar contas corporativas e contas pessoais? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Use o **É Conta Pessoal** filtre em sua lista inteligente para separar contas pessoais das contas comerciais padrão.

## Onde as informações de minhas contas pessoais são exibidas no Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

As atividades relacionadas às contas de pessoas são exibidas na **Conta** painel.

>[!NOTE]
>
>Marketo Sales Insight&#39;s **Adicionar ao Marketo Campaign** e **Enviar e-mail** as opções não estão disponíveis para contas de pessoas.

## Como associar oportunidades a uma conta de pessoa? {#how-do-i-associate-opportunities-to-a-person-account}

O Marketo depende da função de contato da oportunidade para determinar a pessoa à qual associar a oportunidade. Você precisa adicionar a função de contato da oportunidade para cada conta de pessoa para conectar a oportunidade à pessoa apropriada no Marketo. Recomendamos que você configure um fluxo de trabalho para adicionar a função de contato da oportunidade automaticamente.

## Qual campo de email devo usar para contas de pessoas? {#which-email-field-should-i-use-for-person-accounts}

Há dois campos de email para uma conta de pessoa. Use o **Endereço de e-mail** em seus formulários (não o campo **Endereço de email da pessoa**) para garantir que a eliminação de duplicação da Marketo e outros processos de e-mail funcionem corretamente.
