---
unique-page-id: 13795727
description: Anular a entrega de programas de email agendados com fuso horário do destinatário - Documentação do Marketo - Documentação do produto
title: Interromper a entrega de programas de email agendados com o fuso horário do destinatário
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---

# Interromper a entrega de programas de email agendados com o fuso horário do destinatário {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

Em casos de emergência, você pode suspender o delivery de um programa de email que já começou a ser executado com o Fuso horário do recipient ativado.

Como os programas de email agendados com Fuso horário do destinatário podem ser executados por até 24 horas, abortar o delivery do programa cancelará todos os envios subsequentes após esse ponto.

1. Selecione o programa de email que deseja cancelar e clique em **Anular entrega** no bloco Aprovação do painel de controle.

   ![](assets/ptz-abortdelivery.png)

1. Confirme se deseja cancelar o delivery clicando em **Anular**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Após o cancelamento, a **Resultados** A grade do seu programa de email será semelhante à mostrada abaixo. Quaisquer envios subsequentes serão cancelados e serão exibidos como &quot;Email rejeitado Soft&quot; na **Tipo de atividade** coluna.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Os emails cancelados **não** aparecer como uma rejeição temporária *até* a hora em que foram originalmente agendadas para serem entregues em seus respectivos fusos horários. Até esse ponto, eles ainda serão exibidos como &quot;Enviar email&quot;.

1. Na grade, você pode clicar em qualquer email para exibir os detalhes da atividade. Para um envio cancelado, a janela pop-up de detalhes será semelhante a:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Noções básicas sobre o fuso horário do recipient](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Programar programas de e-mail com fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
