---
unique-page-id: 1147066
description: Substituir restrições de pessoa em uma campanha inteligente - Documentação do Marketo - Documentação do produto
title: Substituir restrições de pessoa em uma campanha inteligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Substituir restrições de pessoa em uma campanha inteligente {#override-person-restrictions-in-a-smart-campaign}

O Marketo Engage permite que você defina o número máximo de pessoas que podem se qualificar para uma Campanha Inteligente; isso ajuda a evitar enviar um email para todo o banco de dados acidentalmente. Se você deseja _substituir_ esse limite, veja como.

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
