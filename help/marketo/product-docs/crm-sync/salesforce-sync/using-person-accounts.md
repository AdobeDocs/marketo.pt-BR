---
unique-page-id: 4719316
description: Uso de contas de pessoas - Documentação do Marketo - Documentação do produto
title: Uso de contas de pessoas
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Uso de contas de pessoas {#using-person-accounts}

Contas de pessoas podem ser configuradas no Salesforce para atender às necessidades de sua organização. Veja como o Marketo Engage trata contas pessoais.

>[!NOTE]
>
>As contas padrão do [!DNL Salesforce] são contas comerciais. O administrador do [!DNL Salesforce] precisa configurar as contas de pessoa separadamente.

## O que é uma conta de pessoa? {#what-is-a-person-account}

Uma conta de pessoa é muito semelhante ao objeto de conta em [!DNL Salesforce]. No entanto, uma conta de pessoa tem acesso aos campos de conta e de contato.

## O que acontece quando uma conta de pessoa é sincronizada com o Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Uma conta de pessoa é sincronizada com a Marketo como uma empresa e como uma pessoa.

>[!NOTE]
>
>Os campos personalizados de uma conta de pessoa são copiados para a empresa e para a pessoa no Marketo.

## Como posso diferenciar contas corporativas e contas pessoais? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Use o filtro &quot;É Conta Pessoal&quot; na sua Smart List para separar contas pessoais das contas comerciais padrão.

## Onde as informações de minhas contas pessoais são exibidas no Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

As atividades relacionadas às contas de pessoas são exibidas no painel **[!UICONTROL Conta]**.

>[!NOTE]
>
>As opções **[!UICONTROL Adicionar à Campanha do Marketo]** e **[!UICONTROL Enviar Email]** do Marketo Sales Insight não estão disponíveis no momento para contas pessoais.

## Como associar oportunidades a uma conta de pessoa? {#how-do-i-associate-opportunities-to-a-person-account}

O Marketo depende da função de contato da oportunidade para determinar a pessoa à qual associar a oportunidade. Você precisa adicionar a função de contato da oportunidade para cada conta de pessoa para conectar a oportunidade à pessoa apropriada no Marketo. Recomendamos que você configure um fluxo de trabalho para adicionar a função de contato da oportunidade automaticamente.

## Qual campo de email devo usar para contas de pessoas? {#which-email-field-should-i-use-for-person-accounts}

Há dois campos de email para uma conta de pessoa. Use o campo **[!UICONTROL Endereço de email]** em seus formulários (não o **[!UICONTROL Endereço de email da pessoa]**) para garantir que a eliminação de duplicação e outros processamentos de email da Marketo funcionem corretamente.
