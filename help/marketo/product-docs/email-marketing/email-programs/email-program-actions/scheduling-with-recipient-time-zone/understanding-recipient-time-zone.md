---
unique-page-id: 12983291
description: Noções básicas sobre fuso horário do recipient - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre o fuso horário do recipient
exl-id: 8895241e-94c9-43a2-9158-11c1994df09b
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 1%

---

# Noções básicas sobre o fuso horário do recipient {#understanding-recipient-time-zone}

Os programas de email e de engajamento podem ser configurados para serem entregues de acordo com os fusos horários dos destinatários, eliminando a necessidade de criar vários programas — enviar uma vez e o Marketo retém automaticamente o email até o horário local correto.

>[!NOTE]
>
>[!UICONTROL Fuso Horário do Destinatário] funciona atualmente **somente** com conteúdo de email. Ele não funcionará para programas de engajamento padrão.

## Programas de email {#email-programs}

Há dois cenários principais ao [agendar um programa de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md):

1. Agendando o programa para execução nas próximas 25 horas.
1. Agendar o programa para execução por mais de 25 horas no futuro (ou seja, na próxima semana).

Para acomodar cada fuso horário, os programas de email agendados com o [!UICONTROL Fuso Horário do Destinatário] começam a ser executados à meia-noite no fuso horário **primeiro/primeiro** no mundo (UTC +14:00).

## Programas de envolvimento {#engagement-programs}

Quando você [agendar uma transmissão de programa de envolvimento](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) e o [!UICONTROL Fuso Horário do Destinatário] estiver ativo, a transmissão do programa começará à meia-noite em UTC +14:00. Nós exigimos que você agende o primeiro elenco de pelo menos 25 horas no futuro (24 horas + algum tempo para começar a campanha) porque as pessoas podem se qualificar para o elenco em todos os fusos horários em todo o mundo. Começar a processar neste horário em UTC +14:00 garante que enviaremos o email na data e hora agendadas para cada pessoa que se qualificar para essa conversão.

## Calcular Fuso Horário {#calculating-time-zone}

O Marketo calcula o fuso horário com base na cidade, estado, país ou CEP de uma pessoa. Se não formos capazes de calcular o fuso horário de alguém a partir desses valores, revertemos para os campos Cidade inferida, Estado inferido, País inferido e CEP inferido.

Nos casos em que temos **somente** País ou **somente** Estado disponível:

* Para países com três ou menos fusos horários, selecionamos o fuso horário intermediário.
* Para estados com dois fusos horários, selecionamos o mais antigo dos dois.

Se ainda não for possível determinar o fuso horário de alguém a partir de qualquer combinação desses campos, **não** atribuiremos um fuso horário e o email será enviado com base no fuso horário da sua assinatura do Marketo. Assim, se o seu programa estiver agendado para 9:00am PDT, as pessoas sem fuso horário atribuído receberão o email em 9:00am PDT.

>[!NOTE]
>
>O Marketo recalcula automaticamente o fuso horário de uma pessoa quando qualquer um dos campos de entrada acima é alterado.

>[!MORELIKETHIS]
>
>* [Agendar Programas de Email com [!UICONTROL Fuso Horário do Destinatário]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Head Start para Programas de Email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>
>* [Agendar Programas de Envolvimento com [!UICONTROL Fuso Horário do Destinatário]](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)
