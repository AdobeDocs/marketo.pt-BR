---
unique-page-id: 13795727
description: Anular a entrega de programas de email agendados com fuso horário do destinatário - Documentação do Marketo - Documentação do produto
title: Interromper a entrega de programas de email agendados com o fuso horário do destinatário
exl-id: e69afa4a-32fb-4791-a9b6-683d64d610d6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Interromper a entrega de programas de email agendados com o fuso horário do destinatário {#abort-delivery-of-email-programs-scheduled-with-recipient-time-zone}

Em casos de emergência, você pode suspender o delivery de um programa de email que já começou a ser executado com o Fuso horário do recipient ativado.

Como os programas de email agendados com Fuso horário do destinatário podem ser executados por até 24 horas, abortar o delivery do programa cancelará todos os envios subsequentes após esse ponto.

1. Selecione o programa de email que deseja cancelar e clique em **[!UICONTROL Interromper Entrega]** no bloco [!UICONTROL Aprovação] do painel de controle.

   ![](assets/ptz-abortdelivery.png)

1. Confirme se deseja cancelar a entrega clicando em **[!UICONTROL Abortar]**.

   ![](assets/image2018-2-23-11-3a20-3a27.png)

1. Após o cancelamento, a grade de **[!UICONTROL Resultados]** do seu programa de email será semelhante à grade abaixo. Todos os envios subsequentes serão cancelados e exibidos como &quot;Email rejeitado temporariamente&quot; na coluna **[!UICONTROL Tipo de atividade]**.

   ![](assets/image2018-2-23-11-3a22-3a11.png)

   >[!NOTE]
   >
   >Os emails cancelados **não** serão exibidos como uma rejeição temporária *até* a hora em que foram originalmente agendados para serem entregues em seus respectivos fusos horários. Até esse ponto, eles ainda serão exibidos como &quot;Enviar email&quot;.

1. Na grade, você pode clicar em qualquer email para exibir os detalhes da atividade. Para um envio cancelado, a janela pop-up de detalhes será semelhante a:

   ![](assets/image2018-2-23-11-3a30-3a46.png)

>[!MORELIKETHIS]
>
>* [Noções Básicas sobre o Fuso Horário do Destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Agendar Programas de Email com Fuso Horário do Destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
