---
unique-page-id: 12982903
description: Programar programas de email com fuso horário do destinatário - Documentação do Marketo - Documentação do produto
title: Programar programas de e-mail com fuso horário do destinatário
exl-id: d0c3f3c1-9f21-4081-818d-7c5cb1766915
feature: Email Programs
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Programar programas de e-mail com fuso horário do destinatário {#schedule-email-programs-with-recipient-time-zone}

Há dois cenários possíveis ao agendar um programa de email enquanto o Fuso horário do recipient estiver habilitado:

1. Agendando o programa para execução **dentro** das próximas 25 horas
1. Agendando o programa para ser executado **mais** do que 25 horas no futuro (isto é, na próxima semana)

## Cenário 1: no prazo de 25 horas {#scenario-within-hours}

Considere que você aprove um programa de email com o Fuso horário do destinatário ativado e um horário de entrega agendado nas próximas 25 horas. Você pode ter pessoas em sua lista inteligente que vivem em fusos horários em que a hora agendada já passou.

Nesse cenário, permitimos que você decida o que fazer com esse subconjunto de pessoas qualificadas. Clique no ícone de engrenagem ao lado de **[!UICONTROL Fuso Horário do Destinatário]** no bloco **[!UICONTROL Agendamento]** do programa de email.

![](assets/image2017-12-5-10-3a46-3a42.png)

Isso oferece duas opções:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definição**
>
>* **[!UICONTROL Entregar o dia seguinte no fuso horário do destinatário]**: se o email estiver agendado para sair na terça-feira às 9:00am, as pessoas qualificadas que vivem nos fusos horários em que o horário agendado já passou receberão o email em *quarta-feira* às 9:00am.
>
>* **[!UICONTROL Entregar usando a hora definida padrão do programa]**: se o email estiver agendado para sair na terça-feira às 9:00am, as pessoas qualificadas que vivem nos fusos horários em que a hora agendada já passou receberão o email *com base nas configurações de fuso horário da sua assinatura*. Portanto, se as [configurações de fuso horário da sua assinatura](/help/marketo/product-docs/administration/settings/select-your-language-locale-and-time-zone.md) estiverem definidas como PDT America/Los Angeles, esses destinatários ainda receberão o email na terça-feira às 9:00am PDT (qualquer hora que estiver em seus próprios fusos horários).

>[!NOTE]
>
>[Saiba mais](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md#calculating-time-zone) sobre como o Marketo calcula fusos horários para destinatários.

Vamos considerar esse cenário mais detalhadamente. Digamos que você esteja em São Francisco, agendando um email às 7:00am para um envio de **9:00am**. Na sua lista inteligente, há pessoas das seguintes regiões:

* São Francisco
* Texas
* Nova York
* Itália

![](assets/image2017-12-6-10-3a52-3a41.png)

9:00am já passou em Nova York e na Itália, portanto, as pessoas qualificadas nesses dois fusos horários receberão o email com base nas **Configurações de Fuso Horário**:

* **[!UICONTROL Entregar o dia seguinte no fuso horário do destinatário]:** quarta-feira às 9:00am em seus respectivos fusos horários, **OU**

* **[!UICONTROL Entregar usando o horário definido padrão do programa]**: terça-feira às 9:00am PDT (Nova York - 12:00pm EDT e Itália - 6:00pm CET).

Depois de aprovar, o programa começa a ser executado em 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Embora o programa inicie o *processo* de envio de emails em 15 minutos, os emails não serão *entregues* nesse momento. Os destinatários ainda receberão emails com base nas **[!UICONTROL Configurações de Fuso Horário]** escolhidas por você.

## Cenário 2: mais de 25 horas {#scenario-more-than-hours}

Neste segundo cenário, você aprova um programa de email com **[!UICONTROL Fuso horário do destinatário]** habilitado e um tempo de entrega agendado de mais de 25 horas no futuro. Nesse caso, o programa começará a ser executado no horário agendado no fuso horário **mais antigo** no mundo (UTC + 14:00). Pode haver pessoas qualificadas para a sua lista inteligente em todos os fusos horários do mundo, portanto, iniciar no fuso horário mais antigo permite enviar o email na data/hora agendada para todos os destinatários em seus respectivos fusos horários.

**Início prévio**

Agora, vamos falar sobre como o [[!UICONTROL Head Start]](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funciona com o **[!UICONTROL Fuso Horário do Destinatário]**. Nosso recurso Head Start existente exige que o programa seja agendado com pelo menos 12 horas de antecedência. O que isso significa para o Fuso horário do recipient? Lembre-se de que quando o Fuso Horário do Destinatário é habilitado, começamos a executar o programa de email no horário agendado no fuso horário mais antigo (UTC +14:00). Portanto, para habilitar **o Head Start e o Fuso Horário do Destinatário**, os programas de email precisam ser agendados **com pelo menos 12 horas de antecedência em relação ao horário agendado em UTC +14:00.**

Isso significa que, se você estiver na América/Los Angeles e quiser habilitar o Head Start e o Fuso horário do destinatário, será necessário agendar o programa com **34 horas** de antecedência. Como chegamos a esse número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Em resumo, os programas de email agendados com o Fuso horário do destinatário precisam começar a ser executados no horário agendado no fuso horário mais antigo (ou seja, onde ele atinge a meia-noite primeiro) para acomodar todos os fusos horários. Portanto, se você agendar um programa de email...

* **com um tempo de entrega de *dentro de* 25 horas**, o programa começa a ser executado em 15 minutos. Os recipients que já passaram o horário agendado receberão o email com base nas configurações de fuso horário escolhidas.
* **com um tempo de entrega *superior a* 25 horas no futuro**, o programa começa a ser executado no horário agendado no fuso horário mais antigo (UTC +14:00).
* **com Head Start**, o programa inicia o processamento 12 horas antes do horário agendado no fuso horário mais antigo (UTC +14:00).

>[!CAUTION]
>
>Qualquer pessoa que cancelar a assinatura entre o momento em que você inicia seu envio de email e quando ele é realmente entregue ainda receberá o email. Recomendamos ajustar a notificação de cancelamento de inscrição para refletir que o cancelamento de inscrições pode levar de 1 a 2 dias úteis para ser processado.

>[!MORELIKETHIS]
>
>* [Noções Básicas sobre o Fuso Horário do Destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Head Start para Programas de Email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Anular a Entrega de Programas de Email Agendados com Fuso Horário do Destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)
