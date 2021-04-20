---
title: override-person-restriction-in-a-smart-campaign
description: Substituir restrições de pessoa em uma campanha inteligente
exl-id: efdd6c68-a95e-4b2a-9249-e2e1f550b628
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---

# Substituir restrições de pessoa em uma campanha inteligente

<br> 

O Marketo permite definir o número máximo de pessoas que podem se qualificar para uma campanha inteligente; isso ajuda a evitar o envio acidental de todo o banco de dados. Se quiser substituir esse limite, veja como.

>[!IMPORTANT]
>
>Certifique-se de [ativar restrições de pessoa para campanhas inteligentes](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) no Marketo [!UICONTROL Admin].

1. Encontre sua campanha inteligente e clique em **[!UICONTROL Schedule]**.

   ![Imagem Um](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Clique em **[!UICONTROL Regras de qualificação]**.

   ![Imagem dois](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >O limite padrão é aquele definido em Admin.

1. Ao lado de **[!UICONTROL Abortar campanha se os leads qualificados excederem]**, insira um novo limite.

   ![Imagem Três](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>A campanha inteligente não será executada se o número de pessoas que se qualificam exceder o limite definido.

>[!CAUTION]
>
>Tenha cuidado com esse recurso para não incluir muitas pessoas acidentalmente.
