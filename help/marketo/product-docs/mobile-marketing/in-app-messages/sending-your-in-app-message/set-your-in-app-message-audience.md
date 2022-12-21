---
unique-page-id: 10617431
description: Definir o público das mensagens no aplicativo - Documentos do Marketo - Documentação do produto
title: Definir o público das mensagens no aplicativo
exl-id: 696ae5b6-7063-41bc-bcef-27879182ff1e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Definir o público das mensagens no aplicativo {#set-your-in-app-message-audience}

O primeiro passo é decidir quem deve receber a mensagem no aplicativo. Você precisa configurar sua lista inteligente.

1. Clique em **Editar Lista Inteligente**.

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. Na Smart List, o acionador Has Mobile App Activity é preenchido automaticamente. Clique no menu suspenso e selecione o aplicativo no qual deseja colocar a mensagem.

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >No momento, vários valores para o campo Aplicativo móvel não são compatíveis com programas de mensagens no aplicativo.

1. **Abertura do aplicativo** é a configuração padrão Ação , mas é possível selecionar qualquer evento personalizado que já tenha sido configurado.

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >O acionador padrão (Abertura do aplicativo) e qualquer acionador personalizado adicionado ao código pelo desenvolvedor são exibidos automaticamente no seletor de Ação. Se um evento personalizado estiver ausente, verifique com seu desenvolvedor se ele adicionou os eventos personalizados ao aplicativo. Esteja ciente de que o processo de codificação e aprovação de eventos personalizados pode levar algum tempo para ser concluído. Consulte [este artigo](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md) para obter mais informações.

1. As restrições estão disponíveis para a variável **Possui atividade de aplicativo móvel** acione se precisar.

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. Você pode adicionar filtros à sua lista inteligente para limitar quem recebe a mensagem no aplicativo. Neste exemplo, usando o **Data de aquisição** , somente as pessoas adquiridas em 9 de junho de 2016 receberão a mensagem no aplicativo.

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. Retorne à mensagem no aplicativo Painel de controle do Campaign. Defina o limite de exibição no menu suspenso .

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >O limite de exibição padrão é **Uma vez por sessão**. Se desejar que a mensagem pare de ser exibida depois que o recipient responder, selecione **Todas as vezes até tocar**. Se for exibido todas as vezes, independentemente do que o recipient faz, selecione **Todas as vezes**.

   ![](assets/image2016-5-9-15-3a32-3a6.png)

Bom trabalho! Você tem seu público-alvo definido. Você ganhou a barra azul e a marca de seleção verde.

Hora de [selecione a mensagem no aplicativo](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)!
