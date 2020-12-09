---
unique-page-id: 2359793
description: Usar emails em promoções sociais - Documentos do Marketing - Documentação do produto
title: Usar emails em promoções sociais
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---


# Usar emails em promoções sociais {#use-emails-in-social-promotions}

Ao criar uma oferta [de](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) referência ou um [sorteio](../../../../product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), você pode incluir emails para enviar quando a pessoa se inscrever e, novamente, quando a pessoa ganhar a recompensa.

>[!TIP]
>
>Para criar um email, consulte [Enviar uma explosão](../../../../getting-started/quick-wins/send-an-email.md)de email.

Nos emails, use estes tokens:

* **E-mail** de inscrição: Use **`{{social.Share Url}}`** para enviar a cada pessoa participante um link de compartilhamento personalizado.

* **E-mail** de disponibilização: Use **`{{social.Promo Code}}`** para enviar a cada vencedor um código [promocional](use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Antes de adicionar um email a um aplicativo social, ele deve estar *operacional* e *aprovado*. Consulte [Editar configurações para um email](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Vá para **Marketing Atividade**.

   ![](assets/ma.png)

1. Selecione o aplicativo e clique em **Editar rascunho**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. No editor de aplicativos sociais, vá até Configurações do **aplicativo > Detalhes** da Oferta (ou Detalhes **do** Sorteio).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Adicione o email de inscrição.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >O e-mail de confirmação é enviado automaticamente quando uma pessoa se inscreve.

1. Adicione o email de disponibilização.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Em uma oferta de referência, escolha se o e-mail de preenchimento é enviado automática ou manualmente.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Em sorteios, o e-mail de disponibilização é sempre enviado automaticamente quando você [seleciona o vencedor](../../../../product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definição**
>
>* **auto na meta**: O e-mail de disponibilização é enviado automaticamente conforme cada participante atinge a meta.
>* **enviar** manualmente: Quando as pessoas start atingirem a meta, retorne à sua oferta de referência para [enviar manualmente o e-mail](../../../../product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md)de conclusão.

>



>[!NOTE]
>
>**Artigos relacionados**
>
>Em seguida, você pode [escolher o URL](choose-the-share-url-for-a-social-app.md) de compartilhamento ou, na sua oferta de referência, pode [carregar os códigos](use-promo-codes-for-offer-fulfillment.md) promocionais que você enviará.

