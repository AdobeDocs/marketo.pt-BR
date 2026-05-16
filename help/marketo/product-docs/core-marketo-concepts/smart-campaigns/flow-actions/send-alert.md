---
unique-page-id: 1146958
description: Saiba como enviar um alerta em uma etapa do fluxo do Campaign inteligente. Notifique os usuários quando alguém entrar no fluxo ou atender aos critérios.
title: Enviar alerta
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/QOWt5ZiUVTAi5mqIrniwDrbkx-3keRxXvykkb6IuyA8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 166
ht-degree: 2%

---

# Enviar alerta {#send-alert}

A Marketo Engage pode enviar um alerta por email com informações pessoais para qualquer pessoa: o proprietário das vendas, um parceiro ou outra pessoa. Use a etapa de fluxo &quot;[!UICONTROL Enviar Alerta]&quot;.

![](assets/send-alert-1.png)

1. Localize e selecione o email que deseja enviar.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >Seu alerta de email deve conter todas as informações de cabeçalho e estar no estado **[!UICONTROL Aprovado]**.

1. Você pode clicar no ícone de visualização para garantir que selecionou o email correto.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Use o token &quot;[!UICONTROL Enviar Informações de Alerta]&quot; no seu email.

1. Selecione o destinatário do alerta. Você pode escolher [!UICONTROL Proprietário de vendas] ou [!UICONTROL Proprietário da conta].

   ![](assets/send-alert-4.png)

1. Como opção, adicione outros endereços de email desejados (separados por vírgula ou ponto e vírgula).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >Em campanhas de gatilho, você pode usar tokens em **[!UICONTROL Para Outros Emails]**, como `{{lead.Territory Owner}}` ou `{{my.Alert Recipient}}`, desde que os valores sejam endereços de email válidos. Os tokens em **[!UICONTROL Para outros emails]** não funcionarão em uma campanha em lote.

>[!MORELIKETHIS]
>
>[Criar um email](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
