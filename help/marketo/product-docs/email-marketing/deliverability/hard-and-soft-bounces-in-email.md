---
unique-page-id: 1147328
description: Devoluções permanentes e suaves no email - Documentos da Marketo - Documentação do produto
title: Devoluções permanentes e suaves no email
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Devoluções permanentes e suaves no email {#hard-and-soft-bounces-in-email}

Um rejeição pode tornar o endereço de email de uma pessoa inválido quando um servidor de email informa à Marketo que o email da pessoa não pode ser entregue. Uma rejeição temporária significa que algo deu errado ao entregar o email para a pessoa; isso é resolvido automaticamente e, às vezes, pode levar dias. As devoluções permanentes e temporárias consistem em [várias categorias](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificação de rejeição {#bounce-classification}

Há 5 cadeias de caracteres de pessoa no Marketo relacionadas à entrega de e-mail com problemas.

1. **Email suspenso** - Defina como True quando ocorrer um determinado tipo de rejeição permanente.
1. **Causa Suspensa de Email** - Pode haver muitas razões. Este campo tenta explicar a causa.
1. **Email suspenso em** - Quando a rejeição ofensiva ocorrer, a Marketo suspenderá a correspondência à pessoa por 24 horas a partir desse carimbo de data e hora.
1. **Email Inválido** - Defina como True quando ocorrer um determinado tipo de rejeição permanente.
1. **Causa Inválida do Email** - A razão para a rejeição forçada.

>[!NOTE]
>
>Depois que uma pessoa chega **email suspenso** , não há como desmarcar a caixa de seleção suspensa do email. No entanto, a pessoa continuará a ser endereçável 24 horas após a suspensão inicial.
>
>Quando uma pessoa é marcada como **email inválido**, eles só podem ser redefinidos manualmente (o que recomendamos que você faça somente se tiver certeza de que o email deles é válido) desmarcando a caixa &quot;Email Invalid&quot; na guia Informações de pessoa do registro.

>[!PREREQUISITES]
>
>Seguir [essas etapas](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para criar um Relatório de desempenho de email que gerará dados de devolução.

Depois de criar o Relatório de desempenho de email, a tela deve ser semelhante a:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Filtros de spam às vezes criam rejeições. Esses &quot;falsos positivos&quot; não são uma indicação da verdadeira validade do endereço de email da pessoa.
