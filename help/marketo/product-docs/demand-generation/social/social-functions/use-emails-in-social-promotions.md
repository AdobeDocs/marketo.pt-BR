---
unique-page-id: 2359793
description: Usar emails em promoções sociais - Documentos do Marketo - Documentação do produto
title: Usar emails em promoções sociais
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Usar emails em promoções sociais {#use-emails-in-social-promotions}

Ao criar um [oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) ou [sorteio](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), você pode incluir emails para enviar quando a pessoa se inscrever e novamente quando a pessoa tiver ganhado a recompensa.

>[!TIP]
>
>Para criar um email, consulte [Enviar uma explosão de email](/help/marketo/getting-started/quick-wins/send-an-email.md).

Nos emails, use estes tokens:

* **Email de inscrição**: Use **`{{social.Share Url}}`** para enviar a cada pessoa participante um link de compartilhamento personalizado.

* **Email de preenchimento**: Use **`{{social.Promo Code}}`** para enviar um [código promocional](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Antes de adicionar um email a um aplicativo social, ele deve ser _operacional_ e _aprovado_. Consulte [Editar configurações de um email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Ir para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione o aplicativo e clique em **Editar rascunho**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. No editor de aplicativos sociais, acesse **Configurações do aplicativo > Detalhes da oferta** ou **Detalhes do sorteio**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Adicione o email de inscrição.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >O email de confirmação é enviado automaticamente quando uma pessoa se inscreve.

1. Adicione o email de preenchimento.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Em uma oferta de referência, escolha se o email de preenchimento é enviado automaticamente ou manualmente.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Em um sorteio, o email de cumprimento é sempre enviado automaticamente quando você [selecione o vencedor](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definição**
>
>* **meta automática**: O email de conclusão é enviado automaticamente conforme cada participante atinge a meta.
>* **enviar manualmente**: Quando as pessoas começarem a atender à meta, retorne à oferta de referência para [enviar o email de preenchimento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>


>[!MORELIKETHIS]
>
>Em seguida, você pode [escolha o URL de compartilhamento](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) ou, em sua oferta de referência, você pode [fazer upload dos códigos promocionais](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) você vai enviar.
