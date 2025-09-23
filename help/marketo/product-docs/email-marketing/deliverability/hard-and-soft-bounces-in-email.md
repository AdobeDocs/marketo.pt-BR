---
unique-page-id: 1147328
description: Rejeições permanentes e temporárias no email - Documentação do Marketo - Documentação do produto
title: Rejeições permanentes e temporárias no email
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 15%

---

# Rejeições permanentes e temporárias no email {#hard-and-soft-bounces-in-email}

Uma rejeição permanente pode tornar o endereço de email de uma pessoa inválido quando um servidor de email informa ao Marketo que o email da pessoa não pode ser entregue. Uma rejeição temporária significa que algo deu errado ao enviar o email para a pessoa. Isso é resolvido automaticamente e, às vezes, pode levar dias. As rejeições permanentes e temporárias consistem em [várias categorias](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificação de rejeição {#bounce-classification}

Há 5 strings de pessoas no Marketo relacionadas à entrega de email com problemas.

1. **Email Suspenso** - Definido como Verdadeiro quando ocorrer um determinado tipo de rejeição permanente.
1. **Causa de suspensão de email** - Pode haver muitos motivos. Este campo tenta explicar a causa.
1. **Email Suspenso às** - Quando a rejeição ofensiva ocorrer, o Marketo suspenderá a correspondência para a pessoa por 24 horas a partir desse carimbo de data/hora.
1. **Email Inválido** - Definido como Verdadeiro quando ocorrer um determinado tipo de rejeição permanente.
1. **Causa Inválida de Email** - O motivo da rejeição permanente.

>[!NOTE]
>
>Depois que uma pessoa atinge o status de **email suspenso**, não há como limpar a caixa de seleção email suspenso. No entanto, a pessoa ainda poderá enviar correio 24 horas após a suspensão inicial.
>
>Quando uma pessoa é marcada como **email inválido**, ela só pode ser redefinida manualmente (o que recomendamos que você saiba que o email dela é válido) ao desmarcar a caixa &quot;Email inválido&quot; na guia Informações da pessoa do registro.

>[!PREREQUISITES]
>
>Siga [estas etapas](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para criar um Relatório de desempenho de email que gerará dados de devolução.

Depois de criar o Relatório de desempenho de email, sua tela deve ter esta aparência:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Os filtros de spam às vezes criam rejeições permanentes. Esses &quot;falsos positivos&quot; não são uma indicação da verdadeira validade do endereço de email da pessoa.
