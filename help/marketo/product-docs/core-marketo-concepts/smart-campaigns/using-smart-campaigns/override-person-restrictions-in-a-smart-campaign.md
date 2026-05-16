---
unique-page-id: 1147066
description: Saiba como substituir as restrições de pessoa em uma Campanha inteligente. Permitir que as pessoas executem mesmo que atinjam os limites de comunicação.
title: Substituir restrições de pessoa em uma campanha inteligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 9%

---

# Substituir restrições de pessoa em uma campanha inteligente {#override-person-restrictions-in-a-smart-campaign}

O Marketo Engage permite que você defina o número máximo de pessoas que podem se qualificar para uma Campanha inteligente; isso ajuda a evitar enviar um email para todo o banco de dados acidentalmente. Se você deseja _substituir_ esse limite, veja como.

>[!PREREQUISITES]
>
>Certifique-se de [habilitar as restrições de pessoa para Campanhas inteligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} no Marketo Admin.

1. Em **[!UICONTROL Atividades de marketing]**, vá para sua Campanha inteligente e clique em **[!UICONTROL Agendar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Em Configurações do Smart Campaign, clique em **[!UICONTROL Editar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >O limite padrão é o definido em Admin.

1. Insira um novo limite e clique em **[!UICONTROL Salvar]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   A Campanha inteligente não será executada se o número de pessoas qualificadas exceder o limite definido.

   >[!CAUTION]
   >
   >Tenha cuidado com esse recurso para que você não inclua muitas pessoas acidentalmente.
