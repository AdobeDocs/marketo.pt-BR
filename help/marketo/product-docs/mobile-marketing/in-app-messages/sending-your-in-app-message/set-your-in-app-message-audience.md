---
unique-page-id: 10617431
description: Definir a Audiência de mensagens no aplicativo - Documentos do Marketo - Documentação do produto
title: Definir a Audiência de mensagens no aplicativo
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Definir a Audiência de mensagens no aplicativo {#set-your-in-app-message-audience}

A primeira etapa é decidir quem deve receber sua mensagem no aplicativo. Você precisa configurar sua lista inteligente.

1. Clique em **Editar Lista inteligente**.

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. Na Lista inteligente, o acionador Tem Atividade de aplicativo móvel é preenchido automaticamente. Clique na lista suspensa e selecione o aplicativo no qual deseja colocar a mensagem.

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >Vários valores para o campo Aplicativo móvel não são suportados atualmente para programas de mensagem no aplicativo.

1. **Aplicativo** Abre a configuração padrão Ação, mas você pode selecionar qualquer evento personalizado que já tenha sido configurado.

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >O acionador padrão (App Open) e qualquer acionador personalizado adicionado ao código pelo seu desenvolvedor são exibidos automaticamente no seletor de Ação. Se um evento personalizado estiver faltando, verifique com seu desenvolvedor para garantir que ele adicionou os eventos personalizados ao aplicativo. Esteja ciente de que o processo de codificação e aprovação de eventos personalizados pode levar algum tempo para ser concluído. Consulte [este artigo](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md) para obter mais informações.

1. Há restrições disponíveis para o acionador **Has Mobile App Atividade**, se necessário.

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. Você pode adicionar filtros à sua lista inteligente para limitar quem recebe a mensagem no aplicativo. Neste exemplo, usando o filtro **Data de aquisição**, somente as pessoas adquiridas em 9 de junho de 2016 receberão a mensagem no aplicativo.

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. Retorne ao Painel de controle do Campaign de mensagem no aplicativo. Defina o limite de exibição no menu suspenso.

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >O limite de exibição padrão é **Uma vez por sessão**. Se desejar que a mensagem pare de ser exibida depois que o recipient responder, selecione **Toda vez até que toque**. Se for exibido sempre, não importa o que o recipient faça, escolha **Cada vez**.

   ![](assets/image2016-5-9-15-3a32-3a6.png)

Bom trabalho! Você tem a sua audiência. Você ganhou a barra azul e a marca de seleção verde.

Hora de [selecionar a mensagem no aplicativo](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)!
