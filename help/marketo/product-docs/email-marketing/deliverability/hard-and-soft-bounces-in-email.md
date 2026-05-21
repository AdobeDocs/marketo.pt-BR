---
unique-page-id: 1147328
description: Saiba mais sobre rejeições permanentes e temporárias e como o Marketo as classifica. Use os campos Email suspenso e Email inválido para gerenciar o delivery com problemas.
title: Rejeições permanentes e temporárias no email
exl-id: 53298562-76b6-473a-bf9f-2bec682f4d35
feature: Deliverability
TQID: https://experienceleague.adobe.com/qr4rAdOWWg5dazZVztnoTUv6WJQE8Xpm2WKttjQaOOg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 14%

---

# Rejeições permanentes e temporárias no email {#hard-and-soft-bounces-in-email}

Uma rejeição permanente pode tornar o endereço de email de uma pessoa inválido quando um servidor de email informa ao Marketo que o email da pessoa não pode ser entregue. Uma rejeição temporária significa que algo deu errado ao enviar o email para a pessoa. Isso é resolvido automaticamente e, às vezes, pode levar dias. As rejeições permanentes e temporárias consistem em [várias categorias](https://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificação de rejeição {#bounce-classification}

Há 5 campos de pessoa no Marketo relacionados ao delivery de email com problemas.

1. **Email Suspenso** - Definido como Verdadeiro quando ocorrer um determinado tipo de rejeição permanente.
1. **Causa de suspensão de email** - Pode haver muitos motivos. Este campo tenta explicar a causa.
1. **Email Suspenso às** - Quando a rejeição ofensiva ocorrer, o Marketo suspenderá a correspondência para a pessoa por 24 horas a partir desse carimbo de data/hora.
1. **Email Inválido** - Definido como Verdadeiro quando ocorrer um determinado tipo de rejeição permanente.
1. **Causa Inválida de Email** - O motivo da rejeição permanente.

>[!NOTE]
>
>Depois que uma pessoa atinge o status de **email suspenso**, não há como limpar a caixa de seleção email suspenso. No entanto, a pessoa ainda poderá enviar correio 24 horas após a suspensão inicial.
>
>Quando uma pessoa é marcada como **email inválido**, ela só pode ser redefinida manualmente (o que é recomendado somente se você tiver confirmado que o endereço de email é válido) ao desmarcar a caixa &quot;Email inválido&quot; na guia Informações da pessoa de seu registro.

>[!PREREQUISITES]
>
>Siga [estas etapas](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para criar um Relatório de desempenho de email que gerará dados de devolução.

Depois de criar o Relatório de desempenho de email, sua tela deve ter esta aparência:

![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Os filtros de spam às vezes criam rejeições permanentes. Esses &quot;falsos positivos&quot; não são uma indicação da verdadeira validade do endereço de email da pessoa.
