---
unique-page-id: 1147328
description: Rejeições rígidas e suaves no e-mail - Documentos do Marketing - Documentação do produto
title: Rejeições rígidas e suaves no email
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Rejeições rígidas e suaves no email {#hard-and-soft-bounces-in-email}

Uma rejeição em disco pode tornar inválido o endereço de email de uma pessoa quando um servidor de email informa ao Marketo que o email da pessoa não pode ser entregue. Uma rejeição suave significa que algo deu errado ao entregar o email para a pessoa; isso é resolvido automaticamente e às vezes pode levar dias. As rejeições de hardware e software consistem em [várias categorias](http://nation.marketo.com/t5/Knowledgebase/Maintaining-a-Directory-of-Leads-Bouncing-Emails/ta-p/300838).

## Classificação de rejeição {#bounce-classification}

Há cinco strings no Marketo relacionadas ao delivery de email com problemas.

1. **Email suspenso**  - definido como Verdadeiro quando ocorrer um determinado tipo de rejeição.
1. **Causa**  suspensa por email - Pode haver muitos motivos. Este campo tenta explicar a causa.
1. **E-mail suspenso em **- Quando ocorrer a rejeição ofensiva, o Marketo suspenderá o envio de mensagens para a pessoa por 24 horas a partir desse carimbo de data e hora.
1. **Email inválido**  - Defina como Verdadeiro quando ocorrer um determinado tipo de rejeição.
1. **Causa**  inválida do email - o motivo para a rejeição.

>[!NOTE]
>
>Depois que uma pessoa atingir o status **email suspenso**, não há como limpar a caixa de seleção suspensa do email. No entanto, a pessoa continuará a poder ser enviada 24 horas após a suspensão inicial.
>
>Quando uma pessoa está marcada como **email inválido**, ela só pode ser redefinida manualmente (o que recomendamos que você faça somente se souber que o email dela é válido) desmarcando a caixa &quot;Email inválido&quot; na guia Informações da pessoa de seu registro.

>[!PREREQUISITES]
>
>Siga [estas etapas](../../../product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md) para criar um Relatório de desempenho de email, que gerará dados de rejeição.

Depois de criar seu Relatório de desempenho de email, sua tela deve se parecer com o seguinte: ![](assets/soft-hard-bounce.png)

>[!NOTE]
>
>Filtros de spam às vezes criam rejeições. Esses &quot;falsos positivos&quot; não são uma indicação da verdadeira validade do endereço de email da pessoa.

