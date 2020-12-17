---
unique-page-id: 12982903
description: Agendar Programas de e-mail com fuso horário do Recipient - Documentos do Marketing - Documentação do produto
title: Agendar Programas de e-mail com fuso horário do Recipient
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---


# Agendar Programas de e-mail com fuso horário do Recipient {#schedule-email-programs-with-recipient-time-zone}

Há dois cenários possíveis ao agendar um programa de email enquanto o Fuso horário do Recipient estiver ativado:

1. Agendamento do programa para executar **em** nas próximas 25 horas
1. Agendamento do programa para executar **mais** do que 25 horas no futuro (isto é, na próxima semana)

## Cenário 1: Dentro de 25 horas {#scenario-within-hours}

Vamos supor que você aprove um programa de email com Fuso horário do Recipient ativado e um horário agendado o delivery dentro das próximas 25 horas. Você pode ter pessoas em sua lista inteligente que vivem em fusos horários nos quais o horário agendado já passou.

Neste cenário, permitimos que você decida o que fazer com esse subconjunto de pessoas qualificadas. Clique no ícone de engrenagem ao lado de **Fuso horário do Recipient** no bloco **Agendamento** do programa de email.

![](assets/image2017-12-5-10-3a46-3a42.png)

Isso oferece duas opções:

![](assets/image2017-12-5-10-3a31-3a28.png)

>[!NOTE]
>
>**Definição**
>
>* **Entregue o dia seguinte no fuso horário** do recipient: se o e-mail estiver programado para sair na terça-feira às 9:00, as pessoas qualificadas que vivem em fusos horários nos quais o horário programado já passou, receberão o e-mail às 9: ** 00 da manhã.
   >
   >
* **Entregar usando a hora** padrão do programa: se o e-mail estiver programado para sair na terça-feira às 9h, as pessoas qualificadas que vivem em fusos horários nos quais o horário programado já passou receberão o e-mail  *com base nas configurações* de fuso horário da sua subscrição. Portanto, se suas [s](../../../../../product-docs/administration/settings/select-your-language-locale-and-time-zone.md) [configurações de fuso horário de assinatura](../../../../../product-docs/administration/settings/set-default-location-settings-for-a-subscription.md) estiverem definidas como PDT America/Los Angeles, esses recipient ainda receberão o email na terça-feira às 9h00am PDT (qualquer hora que esteja em seus próprios fusos horários).

>



>[!NOTE]
>
>[Saiba ](https://docs.marketo.com/display/DOCS/Understanding+Recipient+Time+Zone#UnderstandingRecipientTimeZone-CalculatingTimeZone) mais sobre como o Marketo calcula os fusos horários para recipient.

Vamos considerar esse cenário com mais detalhes. Diga que você está em São Francisco, agendando um email às 7h00 para um **9h00am** envio. Em sua lista inteligente, há pessoas das seguintes regiões:

* São Francisco
* Texas
* Nova York
* Itália

![](assets/image2017-12-6-10-3a52-3a41.png)

As 9h00 já passaram em Nova York e na Itália, portanto, as pessoas qualificadas nesses dois fusos horários receberão o email com base nas **Configurações de fuso horário**:

* **Entregar o dia seguinte no fuso horário do recipient:** quarta-feira às 9h00 em seus respectivos fusos horários,  **OU**

* **Entregar usando a hora** padrão do programa: Terça-feira, às 9h00 PDT (Nova Iorque - 12h00 EDT e Itália - 18h CET).

Depois que você aprovar seu programa, ele start em execução dentro de 15 minutos.

![](assets/screen-shot-2017-12-09-at-3.34.14-pm.png)

>[!NOTE]
>
>Embora o programa start o *processo* de enviar emails em 15 minutos, os emails não serão *entregues* no momento. Os recipient ainda receberão emails com base nas **Configurações de fuso horário** escolhidas.

## Cenário 2: Mais de 25 horas {#scenario-more-than-hours}

Neste segundo cenário, você aprova um programa de email com **Fuso Horário do Recipient** ativado e um horário agendado o delivery de mais de 25 horas no futuro. Nesse caso, o programa será start em execução no horário agendado no fuso horário **mais antigo** do mundo (UTC + 14:00). Pode haver pessoas que se qualificam para sua lista inteligente em todos os fusos horários do mundo, portanto, a partir do fuso horário mais antigo, nós enviamos o email na data/hora agendada para todos os recipient em seus respectivos fusos horários.

Start

Agora, vamos falar sobre como [Start de Cabeça](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) funciona com **Fuso Horário do Recipient**. A nossa característica de Start principal exige que o programa seja agendado com pelo menos 12 horas de antecedência. Então o que isso significa para o Fuso Horário do Recipient? Lembre-se de que, quando o Fuso horário do Recipient estiver ativado, será start executar o programa de email no horário agendado no fuso horário mais antigo (UTC +14:00). Assim, para habilitar **tanto** Start de cabeçalho quanto Fuso horário do Recipient, os programas de e-mail precisam ser programados **pelo menos 12 horas antes do horário agendado em UTC +14:00.**

Isso significa que se você estiver na América/Los Angeles e quiser ativar o fuso horário dos Recipient e Start, você precisará agendar o programa **34 horas** antecipadamente. Como chegamos a esse número?

![](assets/image2017-12-5-13-3a11-3a38.png)

<br> 

Resumindo, programas de e-mail programados com o Fuso horário do Recipient precisam ser executados no horário agendado no fuso horário mais antigo (ou seja, no local em que atinge a meia-noite primeiro) para acomodar cada fuso horário. Então, se você agendar um programa por email...

* **com um tempo de delivery  *dentro*  de 25 horas**, os start do programa são executados dentro de 15 minutos. Os recipient que já passaram no horário agendado receberão o email com base nas configurações de fuso horário escolhidas.
* **com um tempo de delivery  ** *superior*  a 25 horas no futuro**, os start de programa em execução no horário agendado no fuso horário mais antigo (UTC +14:00).
* **com Start** de cabeça, o start do programa é processado 12 horas antes da hora prevista no fuso horário mais antigo (UTC +14:00).

>[!CAUTION]
>
>Qualquer pessoa que cancelar a inscrição entre o momento em que você start seu email e quando ele for realmente entregue ainda receberá o email. Recomendamos o ajuste da sua notificação de cancelamento de assinatura para refletir que as cancelar a assinatura podem levar de 1 a 2 dias úteis para serem processadas.

>[!MORELIKETHIS]
>
>* [Noções básicas sobre o fuso horário do Recipient](understanding-recipient-time-zone.md)
>* [Start principal para Programas de e-mail](../../../../../product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md)
>* [Cancelar Delivery de Programas de e-mail agendados com fuso horário do Recipient](abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)

>



