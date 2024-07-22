---
unique-page-id: 2359793
description: Usar emails em promoções sociais - Documentação do Marketo - Documentação do produto
title: Usar emails em promoções sociais
exl-id: 633ad86e-d085-420f-8e28-9b722e345852
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Usar emails em promoções sociais {#use-emails-in-social-promotions}

Ao criar uma [oferta de referência](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md) ou um [sorteio](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), você pode incluir emails a serem enviados quando a pessoa se inscrever e novamente quando ela tiver ganho a recompensa.

>[!TIP]
>
>Para criar um email, consulte [Enviar um Email Blast](/help/marketo/getting-started/quick-wins/send-an-email.md).

Nos emails, use estes tokens:

* **Email de inscrição**: use **`{{social.Share Url}}`** para enviar a cada pessoa participante um link de compartilhamento personalizado.

* **Email de preenchimento**: use **`{{social.Promo Code}}`** para enviar a cada vencedor um [código promocional](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md).

>[!PREREQUISITES]
>
>Antes de adicionar um email a um aplicativo social, ele deve ser _operacional_ e _aprovado_. Consulte [Editar Configurações de um Email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

1. Vá para **Atividades de marketing**.

   ![](assets/ma.png)

1. Selecione o aplicativo e clique em **Editar rascunho**.

   ![](assets/image2014-9-19-16-3a12-3a33.png)

1. No editor de aplicativos sociais, vá para **Configurações do Aplicativo > Detalhes da Oferta** (ou **Detalhes do Sweepstakes**).

   ![](assets/image2014-9-19-16-3a12-3a41.png)

1. Adicione o email de inscrição.

   ![](assets/image2014-9-19-16-3a12-3a49.png)

   >[!NOTE]
   >
   >O email de confirmação é enviado automaticamente quando uma pessoa se inscreve.

1. Adicione o email de preenchimento.

   ![](assets/image2014-9-19-16-3a15-3a26.png)

1. Em uma oferta de referência, escolha se o email de preenchimento será enviado automática ou manualmente.

   ![](assets/image2014-9-19-16-3a15-3a36.png)

>[!NOTE]
>
>Em um sorteio, o email de preenchimento é sempre enviado automaticamente quando você [seleciona o vencedor](/help/marketo/product-docs/demand-generation/social/sweepstakes/select-sweepstakes-winners.md).

>[!NOTE]
>
>**Definição**
>
>* **automático na meta**: o email de preenchimento é enviado automaticamente quando cada participante atinge a meta.
>* **enviar manualmente**: assim que as pessoas começarem a atingir a meta, retorne à sua oferta de referência para [enviar manualmente o email de preenchimento](/help/marketo/product-docs/demand-generation/social/referral-offers/send-referral-offer-fulfillment-email.md).
>

>[!MORELIKETHIS]
>
>Em seguida, você pode [escolher a URL de compartilhamento](/help/marketo/product-docs/demand-generation/social/social-functions/choose-the-share-url-for-a-social-app.md) ou, na sua oferta de referência, você pode [carregar os códigos promocionais](/help/marketo/product-docs/demand-generation/social/social-functions/use-promo-codes-for-offer-fulfillment.md) que enviará.
