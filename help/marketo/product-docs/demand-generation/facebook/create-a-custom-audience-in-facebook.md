---
unique-page-id: 4720275
description: Saiba como criar um público-alvo personalizado no Facebook pelo Marketo. Envie listas do Marketo para o Facebook para campanhas publicitárias direcionadas.
title: Criar um público-alvo personalizado no Facebook
exl-id: a2c8d89c-16b3-44f6-a2c6-c52fe78ab39c
feature: Integrations
TQID: https://experienceleague.adobe.com/ktHiQqaTsZpEm71dLScrC73Pskn-SGIz88iAjgiv14c
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 0%

---

# Criar um Público-alvo Personalizado em [!DNL Facebook] {#create-a-custom-audience-in-facebook}

>[!PREREQUISITES]
>
>* [Adicionar [!DNL Facebook] Públicos-alvo personalizados como um Serviço do LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md){target="_blank"} na seção de Administrador.
>* [Aceite os Termos de Públicos-alvo personalizados](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} do  [!DNL Facebook] na sua conta do [!DNL Facebook].

>[!TIP]
>
>Saiba mais sobre [públicos-alvo personalizados em [!DNL Facebook]](https://www.facebook.com/help/341425252616329){target="_blank"}.

1. Localize e selecione a lista inteligente ou estática que contém os leads dos quais você deseja criar o público-alvo.

   ![](assets/create-a-custom-audience-in-facebook-1.png)

1. Selecione a guia **[!UICONTROL Clientes Potenciais]** e clique no ícone **Enviar por meio de anúncio Bridge** na parte inferior.

   ![](assets/create-a-custom-audience-in-facebook-2.png)

1. Selecione **[!UICONTROL Facebook]** e clique em **[!UICONTROL Avançar]**.

   ![](assets/create-a-custom-audience-in-facebook-3.png)

1. Clique no menu suspenso **[!UICONTROL Público-alvo]** e selecione **[!UICONTROL + Novo Público-alvo]**.

   ![](assets/create-a-custom-audience-in-facebook-4.png)

   >[!IMPORTANT]
   >
   >A API do Facebook permite até 500 públicos-alvo personalizados por conta de anúncio do Facebook.

1. Digite um **[!UICONTROL Nome de público-alvo]**. Clique em **[!UICONTROL Atualizar]**.

   ![](assets/create-a-custom-audience-in-facebook-5.png)

   >[!NOTE]
   >
   >Se você tiver várias Contas publicitárias [!DNL Facebook], verá uma lista suspensa adicional, que permite escolher em qual Conta publicitária esse público-alvo será criado.

   >[!TIP]
   >
   >Para trocar um novo público por um público existente que esteja associado a um conjunto ou grupo de anúncios, marque a caixa de seleção **[!UICONTROL Substituir um público existente]**. Isso **não** excluirá o público-alvo que está sendo substituído.

1. Quando terminar, a caixa de diálogo de status será atualizada.

   ![](assets/create-a-custom-audience-in-facebook-6.png)

   No Facebook, você verá o novo público em **Ads Manager** > **Audiences**.

   ![](assets/create-a-custom-audience-in-facebook-7.png)

   >[!NOTE]
   >
   >Todas as listas que você enviar por push para [!DNL Facebook] se tornam estáticas. As listas inteligentes no Marketo não atualizarão automaticamente a lista de públicos-alvo em [!DNL Facebook] para refletir quaisquer alterações feitas após a transferência.

   >[!MORELIKETHIS]
   >
   >[Adicionar clientes em potencial a um público-alvo personalizado em [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/add-leads-to-a-custom-audience-in-facebook.md)
