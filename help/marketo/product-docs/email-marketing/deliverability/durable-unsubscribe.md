---
unique-page-id: 10094576
description: Cancelamento de assinatura durável - Documentos do Marketing - Documentação do produto
title: Cancelamento de assinatura durável
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---


# Cancelamento de assinatura durável {#durable-unsubscribe}

O Marketo aprimorou o comportamento da funcionalidade de cancelamento de assinatura para torná-la &quot;duradoura&quot;. Adicionamos um status de email principal, que é separado do sinalizador de cancelamento de inscrição visível no registro de detalhes da pessoa.

Se o sinalizador de cancelamento de inscrição for definido de false para true, o status principal do email será atualizado e a alteração será propagada para outras pessoas com o mesmo endereço de email. Se uma pessoa for removida e recriada, ou se um novo registro for criado com o mesmo endereço de email, o sinalizador de cancelamento de inscrição será substituído **not**.

>[!NOTE]
>
>A Cancelamento de assinatura durável funciona em todas as partições em todo o banco de dados do Marketo.

## Atualize o Sinalizador de cancelamento de assinatura de Verdadeiro para Falso (por exemplo, Reinscreva uma Pessoa) {#update-the-unsubscribe-flag-from-true-to-false-e-g-re-subscribe-a-person}

Há várias maneiras de uma pessoa se inscrever novamente.

No Salesforce, **clear** o campo Opt out de email no registro do cliente potencial/contato. Isso será sincronizado com o Marketo.

![](assets/one.png)

No Marketo, **clear** a caixa de cancelamento de inscrição na guia Informações do registro da pessoa.

![](assets/two.png)

Execute uma etapa de fluxo **Alterar valor de dados** como mostrado abaixo em uma ou várias pessoas.

![](assets/three.png)

Atualize uma pessoa existente por meio da API SOAP.

## Criando uma Nova Pessoa {#creating-a-new-person}

Quando uma nova pessoa é criada, o Marketo verifica-a em relação à tabela de status de e-mail principal. Se a pessoa tiver sido anteriormente cancelada, atualizaremos o registro para ser cancelada.

## Alteração de um endereço de email {#changing-an-email-address}

Se você alterar o endereço de email de uma pessoa para um endereço de email não inscrito, essa pessoa será cancelada a inscrição. Essa alteração pode ocorrer no Marketo ou no Salesforce.

Se você alterar um endereço de email não inscrito para um que esteja inscrito, essa pessoa se tornará assinante.

## Inscrever-se novamente {#re-subscribing}

Da mesma forma que cancelar a inscrição faria com que todas as pessoas com o mesmo endereço de email ficassem sem assinatura, um novo script de uma pessoa de fato reescreveria todas as pessoas com o mesmo endereço de email.

## Log de atividades {#activity-log}

As definições de Alteração do valor de dados para _updateLeadEmailStatus_ e _resetLeadEmailStatus_ podem ser encontradas em [este artigo da Comunidade](http://nation.marketo.com/t5/Knowledgebase/Durable-Unsubscribe-Activity-Log/ta-p/252688).

>[!MORELIKETHIS]
>
>[Noções Gerais de Cancelamento de Assinatura](/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md)
