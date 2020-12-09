---
unique-page-id: 12983291
description: Noções sobre o fuso horário do Recipient - Documentos do Marketing - Documentação do produto
title: Noções básicas sobre o fuso horário do Recipient
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Noções básicas sobre o fuso horário do Recipient {#understanding-recipient-time-zone}

Os programas de e-mail e envolvimento podem ser configurados para serem entregues de acordo com os fusos horários dos recipient, eliminando a necessidade de criar vários programas — enviar uma vez e Marketo armazenam automaticamente o e-mail até o horário local correto.

>[!NOTE]
>
>Atualmente, o Fuso horário do recipient funciona **somente** com conteúdo de email. Não funcionará para programas de envolvimento padrão.

## Programas de e-mail {#email-programs}

Há dois cenários principais ao [agendar um programa](schedule-email-programs-with-recipient-time-zone.md)de email:

1. Agendamento do programa para ser executado dentro das próximas 25 horas.
1. Agendamento do programa para execução futura superior a 25 horas (isto é, semana que vem).

Para acomodar cada fuso horário, programas de e-mail programados com start de fuso horário do Recipient funcionando à meia-noite no fuso horário **primeiro/mais antigo** do mundo (UTC +14:00).

## Programas de envolvimento {#engagement-programs}

Quando você [agendar um fluxo](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md) de programa de envolvimento e o Fuso horário do Recipient estiver ativo, o módulo programa será executado à meia-noite em UTC +14:00. Exigimos que você agende o primeiro elenco pelo menos 25 horas no futuro (24 horas + algum tempo para começar a campanha) porque as pessoas podem se qualificar para o elenco em cada fuso horário do mundo. Começar o processamento neste momento no UTC +14:00 garante que entregaremos o email na data e hora agendadas para cada pessoa que se qualificar para este elenco.

## Calculando fuso horário {#calculating-time-zone}

O Marketo calcula o fuso horário com base na Cidade, Estado, País ou CEP de uma pessoa. Se não pudermos calcular o fuso horário de alguém a partir desses valores, revertemos para os campos Cidade Inferida, Estado Inferido, País Inferido e Código Postal Inferido.

Nos casos em que **apenas **País ou **apenas** Estado disponível:

* Para países com três ou menos fusos horários, selecionamos o fuso horário médio.
* Para estados com dois fusos horários, selecionamos o anterior dos dois.

Se ainda não for possível determinar o fuso horário de alguém a partir de qualquer combinação desses campos, **não** atribuiremos um fuso horário e o email será entregue com base no fuso horário da subscrição do Marketo. Portanto, se seu programa estiver programado para PDT das 9h00, as pessoas sem fuso horário atribuído receberão o email às 9h00 PDT.

>[!NOTE]
>
>O Marketo calcula novamente o fuso horário de uma pessoa quando qualquer um dos campos de entrada acima é alterado.

>[!MORELIKETHIS]
>
>* [Agendar Programas de e-mail com fuso horário do Recipient](schedule-email-programs-with-recipient-time-zone.md)
>* [Start principal para Programas de e-mail](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)

   >
   >
* [Agendar Programas de envolvimento com fuso horário do Recipient](../../../../../product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence/schedule-engagement-programs-with-recipient-time-zone.md)

>



