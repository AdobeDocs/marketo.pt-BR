---
unique-page-id: 12983291
description: Noções básicas sobre fuso horário do destinatário - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre fuso horário do destinatário
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# Noções básicas sobre fuso horário do destinatário {#understanding-recipient-time-zone}

Os programas de email e de envolvimento podem ser configurados para serem entregues de acordo com os fusos horários dos recipients, eliminando a necessidade de criar vários programas. Enviar uma vez e o Marketo automaticamente armazena o email até o horário local correto.

>[!NOTE]
>
>Fuso horário do destinatário funciona atualmente **only** com conteúdo de email. Ele não funcionará para programas de envolvimento padrão.

## Programas de e-mail {#email-programs}

Há dois cenários principais quando [agendamento de um programa de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Agendamento do programa para ser executado nas próximas 25 horas.
1. Agendar o programa para ser executado mais de 25 horas no futuro (ou seja, na próxima semana).

Para acomodar cada fuso horário, os programas de email agendados com Fuso horário do destinatário começam a ser executados à meia-noite na **primeiro/primeiro** fuso horário no mundo (UTC +14:00).

## Programas de envolvimento {#engagement-programs}

Quando você [agendar um fluxo de programa de envolvimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e o Fuso horário do destinatário estiver ativo, o programa será executado à meia-noite em UTC +14:00. Exigimos que você programe a primeira transmissão pelo menos 25 horas no futuro (24 horas + algum tempo para iniciar a campanha), pois as pessoas podem se qualificar para a transmissão em cada fuso horário em todo o mundo. Iniciando o processamento nesse momento em UTC +14:00 garante que enviaremos o email na data e hora programadas para cada pessoa qualificada para esse elenco.

## Calculando Fuso Horário {#calculating-time-zone}

O Marketo calcula o fuso horário com base na Cidade, Estado, País ou CEP de uma pessoa. Se não pudermos calcular o fuso horário de alguém a partir desses valores, revertemos para os campos Inferred City, Inferred State, Inferred Country e Inferred Zip Code .

Nos casos em que **only** País ou **only** Estado disponível:

* Para países com três ou menos fusos horários, selecionamos o fuso horário médio.
* Para estados com dois fusos horários, selecionamos o anterior.

Se ainda não pudermos determinar o fuso horário de alguém a partir de qualquer combinação desses campos, nós iremos **not** atribuir um fuso horário e o email será enviado com base no fuso horário da assinatura do Marketo. Portanto, se seu programa estiver programado para 9:00 PDT, as pessoas sem fuso horário atribuído serão enviadas ao email às 9:00 PDT.

>[!NOTE]
>
>O Marketo recalcula automaticamente o fuso horário de uma pessoa quando qualquer um dos campos de entrada acima é alterado.

>[!MORELIKETHIS]
>
>* [Programar programas de e-mail com fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Início do cabeçalho para programas de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Programar programas de envolvimento com fuso horário do destinatário](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

