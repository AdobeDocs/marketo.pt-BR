---
unique-page-id: 10094576
description: Cancelamento de assinatura durável - Documentação do Marketo - Documentação do produto
title: Cancelamento de assinatura durável
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
feature: Deliverability
source-git-commit: 777413b4256ab5342b933fa04c34d8a8d1201c0e
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Cancelamento de assinatura durável {#durable-unsubscribe}

A Marketo aprimorou o comportamento da funcionalidade de cancelamento de inscrição para torná-la &quot;durável&quot;. Adicionamos um status de email principal, que é separado do sinalizador de cancelamento de inscrição visível no registro de detalhes da pessoa.

Se o sinalizador de cancelamento de inscrição estiver definido como falso para verdadeiro, o status do email principal será atualizado e a alteração será propagada para outras pessoas com o mesmo endereço de email. Se uma pessoa for removida e recriada, ou se um novo registro for criado com o mesmo endereço de email, o sinalizador de cancelamento de inscrição **não** será substituído.

>[!NOTE]
>
>O cancelamento de inscrição durável funciona em todas as partições em todo o banco de dados do Marketo.

## Atualizar o sinalizador de cancelamento de inscrição de Verdadeiro para Falso (por exemplo, Assinar novamente uma pessoa) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Há várias maneiras de uma pessoa ser inscrita novamente.

No Salesforce, desmarque o campo Recusa de email no registro do lead/contato. Isso será sincronizado com o Marketo.

![tela do Salesforce](assets/durable-unsubscribe-1.png)

No Marketo, desmarque a caixa de cancelamento de inscrição na guia Informações do registro da pessoa.

![Limpando a caixa de cancelamento de inscrição em um registro de pessoa](assets/durable-unsubscribe-2.png)

Execute uma etapa de fluxo _Alterar Valor de Dados_ como mostrado abaixo em uma ou várias pessoas.

![Alterar etapa do fluxo de valor de dados](assets/durable-unsubscribe-3.png)

## Criar uma nova pessoa {#creating-a-new-person}

Quando uma nova pessoa é criada, o Marketo a verifica em relação à tabela principal de status de email. Se a inscrição da pessoa foi cancelada anteriormente, atualizaremos o registro para cancelar a inscrição.

## Alteração de um endereço de email {#changing-an-email-address}

Se você alterar o endereço de email de uma pessoa para um endereço de email cuja assinatura foi cancelada, essa pessoa terá a assinatura cancelada. Essa alteração pode ocorrer no Marketo ou no Salesforce.

## Assinando novamente {#re-subscribing}

Da mesma forma que um cancelamento de inscrição faria com que todas as pessoas com o mesmo endereço de email tivessem suas assinaturas canceladas, uma reinscrição assinaria todas as pessoas com o mesmo endereço de email.

>[!MORELIKETHIS]
>
>[Noções básicas sobre o cancelamento de inscrição](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
