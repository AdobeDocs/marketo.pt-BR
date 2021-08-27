---
unique-page-id: 4719316
description: Usar contas de pessoa - Documentos do Marketo - Documentação do produto
title: Usando contas de pessoa
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Usando contas de pessoa {#using-person-accounts}

As contas de pessoa podem ser configuradas no Salesforce para atender às necessidades de sua organização. Veja como a Marketo trata as contas pessoais.

>[!NOTE]
>
>As contas padrão do Salesforce são contas comerciais. Seu administrador do Salesforce precisa configurar contas pessoais separadamente.

## O que é uma conta de pessoa? {#what-is-a-person-account}

Uma conta de pessoa é muito semelhante ao objeto de conta no Salesforce. No entanto, uma conta de pessoa tem acesso aos campos da conta e aos campos de contato.

## O que acontece quando uma conta de pessoa é sincronizada com o Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Uma conta de pessoa é sincronizada com o Marketo como uma empresa e como uma pessoa.

>[!NOTE]
>
>Os campos personalizados de uma conta de pessoa são copiados para a empresa e para a pessoa no Marketo.

## Como faço para diferenciar contas comerciais e contas pessoais? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Use o filtro **Is Person Account** em sua lista inteligente para separar as contas de pessoas das contas comerciais padrão.

## Onde estão as informações de contas pessoais exibidas no Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

As atividades relacionadas às contas pessoais são exibidas no painel **Conta**.

>[!NOTE]
>
>As opções **Add to Marketo Campaign** e **Send Email** do Marketo Sales Insight não estão disponíveis no momento para contas pessoais.

## Como associo oportunidades a uma conta de pessoa? {#how-do-i-associate-opportunities-to-a-person-account}

O Marketo depende da função de contato da oportunidade para determinar a pessoa à qual associar a oportunidade. É necessário adicionar a função de contato de oportunidade para cada conta de pessoa para conectar a oportunidade à pessoa adequada no Marketo. Recomendamos que você configure um workflow para adicionar a função de contato de oportunidade automaticamente.

## Qual campo de email devo usar para contas de pessoas? {#which-email-field-should-i-use-for-person-accounts}

Há dois campos de email para uma conta de pessoa. Use o campo **Endereço de email** em seus formulários (não o **Endereço de email da pessoa**) para garantir que a eliminação da duplicação do Marketo e outro processamento de email funcionem corretamente.
