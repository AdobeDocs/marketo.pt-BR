---
unique-page-id: 12982909
description: Programar programas de envolvimento com fuso horário do destinatário - Documentos do Marketo - Documentação do produto
title: Programar programas de envolvimento com fuso horário do destinatário
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Programar programas de envolvimento com fuso horário do destinatário {#schedule-engagement-programs-with-recipient-time-zone}

Quando você agendar um fluxo de programa de engajamento e o fuso horário do recipient estiver ativo, o lançamento do programa começará a ser executado à meia-noite no primeiro fuso horário (UTC +14:00). Exigimos que você programe o primeiro lançamento **pelo menos 25 horas** no futuro porque pode haver pessoas qualificadas para o elenco em todos os fusos horários do mundo. Iniciar o processamento nesse momento no primeiro fuso horário garante que o email seja entregue na data e hora agendadas para cada recipient.

1. No programa de engajamento, navegue até o **Fluxos** e clique no cronograma de cadência de um fluxo para editá-lo.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Defina suas configurações de cadência](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) como normalmente faria, marque a opção **Fuso Horário do Recipient** caixa. Lembre-se de que seu primeiro elenco deve ter pelo menos 25 horas no futuro. Clique em **Salvar**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Observe que com o Fuso horário do destinatário ativo, a programação de cadência não mostrará um fuso horário específico, pois pode haver vários. Ele só exibirá a hora.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Noções básicas sobre fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Definir cadência das transmissões](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)

