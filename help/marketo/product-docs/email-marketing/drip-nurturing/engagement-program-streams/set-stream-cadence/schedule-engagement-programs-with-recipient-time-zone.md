---
unique-page-id: 12982909
description: Programar programas de engajamento com fuso horário do recipient - Documentação do Marketo - Documentação do produto
title: Agendar programas de engajamento com fuso horário do recipient
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Agendar programas de engajamento com fuso horário do recipient {#schedule-engagement-programs-with-recipient-time-zone}

Quando você agendar um fluxo de programa de engajamento e o fuso horário do recipient estiver ativo, a conversão do programa começará a ser executada à meia-noite no primeiro fuso horário (UTC +14:00). Precisamos que você agende o primeiro elenco **pelo menos 25 horas** no futuro porque pode haver pessoas que se qualificam para o elenco em todos os fusos horários em todo o mundo. Iniciar o processamento neste horário no primeiro fuso horário garante que enviaremos o email na data e hora programadas para cada recipient.

1. No programa de engajamento, navegue até o **Fluxos** e clique na programação de cadência de um fluxo para editá-lo.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Definir suas configurações de cadência](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) como normalmente faria, verifique a **Fuso horário do recipient** caixa. Lembre-se de que seu primeiro elenco deve ter pelo menos 25 horas no futuro. Clique em **Salvar**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Observe que com o Fuso horário do recipient ativo, o agendamento de cadência não mostrará um fuso horário específico, pois pode haver vários. Ele só exibirá a hora.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Noções básicas sobre o fuso horário do recipient](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Definir cadência das transmissões](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
