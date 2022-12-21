---
unique-page-id: 13795727
description: Cancelar entrega de programas de email agendados com fuso horário do destinatário - Documentos do Marketo - Documentação do produto
title: Cancelar entrega de programas de email agendados com fuso horário do destinatário
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Cancelar entrega de programas de email agendados com fuso horário do destinatário {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

Em casos de emergência, você pode suspender a entrega de um programa de email que já começou a ser executado com o Fuso Horário do Recipient habilitado.

Como os programas de email agendados com Fuso horário do destinatário podem ser executados por até 24 horas, suspender a entrega do programa cancelará todos os envios subsequentes após esse ponto.

1. Selecione o programa de email que deseja cancelar e clique em **Cancelar entrega** no bloco Aprovação no painel de controle.

   ![](assets/ptz-abortdelivery.png)

1. Confirme se deseja cancelar o delivery clicando em **Abortar**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Após o cancelamento, a variável **Resultados** a grade do seu programa de email será parecida com a abaixo. Quaisquer envios subsequentes são cancelados e serão exibidos como &quot;Enviar email por SMS com rejeição suave&quot; na **Tipo de atividade** coluna.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Os emails cancelados serão **not** mostrar como uma devolução temporária *until* A hora em que foram originalmente programadas para serem entregues nos respectivos fusos horários. Até esse ponto, eles ainda serão exibidos como &quot;Enviar email&quot;.

1. Na grade, você pode clicar em qualquer email para exibir os detalhes da atividade. Para um envio cancelado, a pop-up de detalhes terá esta aparência:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Noções básicas sobre fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Programar programas de e-mail com fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)

