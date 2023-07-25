---
unique-page-id: 12982903
description: Programar programas de email com fuso horário do destinatário - Documentação do Marketo - Documentação do produto
title: Programar programas de e-mail com fuso horário do destinatário
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 1%

---

# Programar programas de e-mail com fuso horário do destinatário {#schedule-email-programs-with-recipient-time-zone}

Há dois cenários possíveis ao agendar um programa de email enquanto o Fuso horário do recipient estiver habilitado:

1. Agendando a execução do programa **no prazo de** as próximas 25 horas
1. Agendando a execução do programa **mais** mais de 25 horas no futuro (ou seja, na próxima semana)

## Cenário 1: no prazo de 25 horas {#scenario-within-hours}

Considere que você aprove um programa de email com o Fuso horário do destinatário ativado e um horário de entrega agendado nas próximas 25 horas. Você pode ter pessoas em sua lista inteligente que vivem em fusos horários em que a hora agendada já passou.

Nesse cenário, permitimos que você decida o que fazer com esse subconjunto de pessoas qualificadas. Clique no ícone de engrenagem ao lado de **Fuso horário do recipient** no **Agendar** bloco do programa de email.

![](assets/image2017-12-5-10-3a46-3a42.png)

Isso oferece duas opções:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definição**
>
>* **Entregar o dia seguinte no fuso horário do destinatário**: se o email estiver agendado para sair na terça-feira às 9h, pessoas qualificadas que vivem em fusos horários em que o horário agendado já passou receberão o email em *Quarta-feira* às 9h.
>
>* **Entregar usando o tempo definido padrão do programa**: se o email estiver agendado para sair na terça-feira às 9h, pessoas qualificadas que vivem em fusos horários em que o horário agendado já passou receberão o email _com base nas configurações de fuso horário da sua assinatura_. Então, se o seu [configurações de fuso horário da assinatura](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) estiverem definidos como PDT America/Los Angeles, esses recipients ainda receberão o email na terça-feira às 9:00 PDT (qualquer hora que estiver em seus próprios fusos horários).

>[!NOTE]
>
>[Saiba mais](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) sobre como o Marketo calcula fusos horários para destinatários.

Vamos considerar esse cenário mais detalhadamente. Digamos que você esteja em São Francisco, agendando um e-mail às 7:00 da manhã para um **9h** enviar. Na sua lista inteligente, há pessoas das seguintes regiões:

* São Francisco
* Texas
* Nova York
* Itália

![](assets/image2017-12-6-10-3a52-3a41.png)

As 9h já passaram em Nova York e na Itália, portanto, pessoas qualificadas nesses dois fusos horários receberão o email com base no **Configurações de Fuso Horário**:

* **Entregar o dia seguinte no fuso horário do destinatário:** Quarta-feira às 9h em seus respectivos fusos horários, **OU**

* **Entregar usando o tempo definido padrão do programa**: Terça-feira às 9h PDT (Nova York - 12h EDT e Itália - 18h CET).

Depois de aprovar, o programa começa a ser executado em 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Embora o programa vá iniciar o _processo_ de enviar emails em 15 minutos, os emails não serão _entregue_ nesse momento. Os recipients ainda receberão emails com base no **Configurações de Fuso Horário** você escolhe.

## Cenário 2: mais de 25 horas {#scenario-more-than-hours}

Nesse segundo cenário, você aprova um programa de email com **Fuso horário do recipient** ativado e um tempo de delivery agendado de mais de 25 horas no futuro. Nesse caso, o programa começará a ser executado no horário agendado no **mais antigo** fuso horário no mundo (UTC + 14:00). Pode haver pessoas qualificadas para a sua lista inteligente em todos os fusos horários do mundo, portanto, iniciar no fuso horário mais antigo permite enviar o email na data/hora agendada para todos os destinatários em seus respectivos fusos horários.

**Head Start**

Agora, vamos falar sobre como [Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funciona com **Fuso horário do recipient**. Nosso recurso Head Start existente exige que o programa seja agendado com pelo menos 12 horas de antecedência. O que isso significa para o Fuso horário do recipient? Lembre-se de que quando o Fuso horário do recipient está ativado, começamos a executar o programa de email no horário agendado no fuso horário mais antigo (UTC +14:00). Assim, para habilitar **ambos** Head Start e Fuso horário do recipient. Os programas de email precisam ser agendados **pelo menos 12 horas antes do horário previsto em UTC +14:00.**

Isso significa que, se você estiver na América/Los Angeles e quiser ativar o Head Start e o Fuso horário do recipient, será necessário agendar o programa **34 horas** antecipadamente. Como chegamos a esse número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Em resumo, os programas de email agendados com o Fuso horário do destinatário precisam começar a ser executados no horário agendado no fuso horário mais antigo (ou seja, onde ele atinge a meia-noite primeiro) para acomodar todos os fusos horários. Portanto, se você agendar um programa de email...

* **com um tempo de delivery _no prazo de_ 25 horas**, o programa começa a ser executado em 15 minutos. Os recipients que já passaram o horário agendado receberão o email com base nas configurações de fuso horário escolhidas.
* **com um tempo de delivery _mais de_ 25 horas no futuro**, o programa começa a ser executado no horário agendado no fuso horário mais antigo (UTC +14:00).
* **com Head Start**, o programa inicia o processamento 12 horas antes do horário agendado no fuso horário mais antigo (UTC +14:00).

>[!CAUTION]
>
>Qualquer pessoa que cancelar a assinatura entre o momento em que você inicia seu envio de email e quando ele é realmente entregue ainda receberá o email. Recomendamos ajustar a notificação de cancelamento de inscrição para refletir que o cancelamento de inscrições pode levar de 1 a 2 dias úteis para ser processado.

>[!MORELIKETHIS]
>
>* [Noções básicas sobre o fuso horário do recipient](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start para programas de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Interromper a entrega de programas de email agendados com o fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
