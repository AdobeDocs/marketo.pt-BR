---
unique-page-id: 10094576
description: Cancelamento de inscrição durável - Documentos do Marketo - Documentação do produto
title: Cancelamento de inscrição durável
exl-id: e03a5a01-7395-45b3-8351-7931ec413236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Cancelamento de inscrição durável {#durable-unsubscribe}

A Marketo aprimorou o comportamento da funcionalidade de cancelamento de inscrição para torná-la &quot;durável&quot;. Adicionamos um status de email principal, que é separado do sinalizador de cancelamento de inscrição visível no registro de detalhes da pessoa.

Se o sinalizador de cancelamento de inscrição for definido de false para true, o status principal do email será atualizado e a alteração será propagada para outras pessoas com o mesmo endereço de email. Se uma pessoa for removida e recriada, ou se um novo registro for criado com o mesmo endereço de email, o sinalizador de cancelamento de assinatura será **not** ser substituído.

>[!NOTE]
>
>O cancelamento de inscrição durável funciona em todas as partições de todo o banco de dados do Marketo.

## Atualizar o Sinalizador de Cancelamento de Assinatura de Verdadeiro para Falso (por exemplo, Assinar novamente uma pessoa) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Há várias maneiras de assinar novamente uma pessoa.

Em Salesforce, **limpar** o campo Recusa de email no registro do cliente potencial/contato. Isso será sincronizado com o Marketo.

![](assets/one.png)

No Marketo, **limpar** a caixa cancelada na guia Informações do registro da pessoa.

![](assets/two.png)

Execute um **Alterar valor de dados** etapa do fluxo, conforme mostrado abaixo, em uma ou várias pessoas.

![](assets/three.png)

Atualize uma pessoa existente por meio da API SOAP.

## Criação de uma nova pessoa {#creating-a-new-person}

Quando uma nova pessoa é criada, o Marketo a verifica em relação à tabela de status de email principal. Se a pessoa tiver cancelado a assinatura anteriormente, atualizaremos o registro para cancelar a assinatura.

## Alterar um endereço de email {#changing-an-email-address}

Se você alterar o endereço de email de uma pessoa para um endereço de email não assinado, essa pessoa será cancelada. Essa alteração pode ocorrer no Marketo ou no Salesforce.

Se você alterar um endereço de email que cancelou a assinatura para um que está inscrito, essa pessoa se tornará subscrita.

## Inscrição novamente {#re-subscribing}

Da mesma forma que cancelar a assinatura faria com que todas as pessoas com o mesmo endereço de email se tornassem canceladas, um novo script de assinatura retornaria a assinatura de todas as pessoas com o mesmo endereço de email.

## Registro de atividades {#activity-log}

Definições de Alteração do valor de dados para _updateLeadEmailStatus_ e _resetLeadEmailStatus_ pode ser encontrado em [artigo da Comunidade](https://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Noções básicas sobre cancelamento de inscrição](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
