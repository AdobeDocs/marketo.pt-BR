---
unique-page-id: 12982903
description: Programar programas de email com fuso horário do destinatário - Documentos do Marketo - Documentação do produto
title: Programar programas de e-mail com fuso horário do destinatário
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Programar programas de e-mail com fuso horário do destinatário {#schedule-email-programs-with-recipient-time-zone}

Há dois cenários possíveis ao agendar um programa de email enquanto o Fuso horário do destinatário estiver ativado:

1. Agendamento do programa para execução **within** nas próximas 25 horas
1. Agendamento do programa para execução **more** mais de 25 horas no futuro (ou seja, na próxima semana)

## Cenário 1: Em 25 Horas {#scenario-within-hours}

Considere que você aprova um programa de email com Fuso horário do destinatário habilitado e um horário de entrega programado nas próximas 25 horas. Você pode ter pessoas em sua lista inteligente que vivem em fusos horários em que o horário agendado já tenha passado.

Nesse cenário, permitimos que você decida o que fazer com esse subconjunto de pessoas qualificadas. Clique no ícone de engrenagem ao lado de **Fuso Horário do Recipient** no **Agendar** bloco do programa de email.

![](assets/image2017-12-5-10-3a46-3a42.png)

Isso oferece duas opções:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definição**
>
>* **Enviar delivery do dia seguinte no fuso horário do recipient**: se o email estiver programado para sair na terça-feira às 9h, as pessoas qualificadas que viverem em fusos horários onde o horário programado já tiver passado receberão o email em *Quarta-feira* às 9h.
>
>* **Enviar delivery usando o tempo definido padrão do programa**: se o email estiver programado para sair na terça-feira às 9h, as pessoas qualificadas que vivem em fusos horários onde o horário programado já passou receberão o email _com base nas configurações de fuso horário da assinatura_. Assim, se o seu [configurações de fuso horário da assinatura](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) estiverem configurados como PDT América/Los Angeles, esses recipients ainda receberão o email na terça-feira às 9:00 PDT (qualquer hora que esteja em seus próprios fusos horários).


>[!NOTE]
>
>[Saiba mais](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) sobre como o Marketo calcula os fusos horários para recipients.

Vamos considerar este cenário com mais detalhes. Diga que você está em São Francisco, agendando um e-mail às 7:00 da manhã para um **9:00** enviar. Na sua lista inteligente, há pessoas das seguintes regiões:

* São Francisco
* Texas
* Nova York
* Itália

![](assets/image2017-12-6-10-3a52-3a41.png)

As 9h já passaram em Nova York e na Itália, portanto as pessoas qualificadas nesses dois fusos horários receberão o email com base na variável **Configurações de fuso horário**:

* **Enviar o delivery do dia seguinte no fuso horário do recipient:** Quarta-feira às 9h00 nos respectivos fusos horários, **OU**

* **Enviar delivery usando o tempo definido padrão do programa**: Terça-feira, às 9h PDT (Nova Iorque - 12h EDT e Itália - 18h CET).

Depois de aprovar seu programa, ele será executado em 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Embora o programa inicie o _processo_ ao enviar emails em 15 minutos, os emails não serão enviados _entregues_ naquela hora. Os recipients ainda receberão emails com base na variável **Configurações de fuso horário** você escolhe.

## Cenário 2: Mais de 25 horas {#scenario-more-than-hours}

Neste segundo cenário, você aprova um programa de email com **Fuso Horário do Recipient** ativado e um tempo de entrega programado que será superior a 25 horas no futuro. Nesse caso, o programa começará a ser executado no horário agendado no **soon** fuso horário no mundo (UTC + 14:00). Pode haver pessoas que se qualificam para sua lista inteligente em cada fuso horário em todo o mundo, portanto, iniciar no fuso horário mais antigo nos permite entregar o email na data/hora agendadas para todos os recipients em seus respectivos fusos horários.

**Head Start**

Agora, vamos falar sobre como [Início da Cabeça](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funciona com **Fuso Horário do Recipient**. A nossa funcionalidade de Início de Cabeça existente requer que o programa seja agendado com pelo menos 12 horas de antecedência. Então, o que isso significa para Fuso Horário do Recipient? Lembre-se de que quando o Fuso horário do destinatário estiver ativado, começamos a executar o programa de email no horário agendado no fuso horário mais antigo (UTC +14:00). Assim, para permitir **both** Fuso horário de início e destinatário, programas de email precisam ser agendados **pelo menos 12 horas antes do horário agendado em UTC +14:00.**

Isso significa que, se você estiver na América/Los Angeles e quiser ativar o Fuso Horário de Início e de Recipient, será necessário agendar o programa **34 horas** antecipadamente. Como chegamos a esse número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Em resumo, os programas de email agendados com Fuso horário do destinatário precisam começar a ser executados no horário agendado no fuso horário mais antigo (ou seja, onde ele atinge a meia-noite primeiro) para acomodar cada fuso horário. Então, se você agendar um programa de e-mail...

* **com um tempo de delivery _within_ 25 horas**, o programa começa a ser executado em 15 minutos. Os recipients que já passaram no horário agendado receberão o email com base nas configurações de fuso horário que você escolheu.
* **com um tempo de delivery _mais de_ 25 horas no futuro**, o programa começa a ser executado no horário agendado no fuso horário mais antigo (UTC +14:00).
* **com Início do Cabeçalho**, o programa inicia o processamento 12 horas antes da hora agendada no fuso horário mais antigo (UTC +14:00).

>[!CAUTION]
>
>Qualquer pessoa que cancelar a assinatura entre o momento em que você inicia o envio do email e quando ele é realmente entregue ainda receberá o email. Recomendamos o ajuste da sua notificação de cancelamento de subscrição para refletir que os cancelamentos de subscrição podem levar de 1 a 2 dias úteis para serem processados.

>[!MORELIKETHIS]
>
>* [Noções básicas sobre fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Início do cabeçalho para programas de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Cancelar entrega de programas de email agendados com fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

