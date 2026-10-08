---
unique-page-id: 2360243
description: Defina um número máximo de pessoas que podem se qualificar para uma Campanha inteligente para evitar o envio acidental por email de todo o banco de dados.
title: Habilitar restrições de pessoa para campanhas inteligentes
exl-id: 45bdaf3f-874c-493f-9746-440f7703713c
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/6VwkOwN9nTqSyNcXvzyggPTk0Um5x1GPXIp2DBf2kww'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 11%
---
# Habilitar restrições de pessoa para campanhas inteligentes {#enable-person-restrictions-for-smart-campaigns}

Há um recurso no Marketo para limitar o número _máximo_ de pessoas que podem se qualificar para uma Campanha Inteligente. Isso evita enviar acidentalmente um email para todo o banco de dados.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!CAUTION]
>
>Isso se aplica somente a campanhas em lote e programas de email.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-1.png)

1. Clique em **[!UICONTROL Campanha Inteligente]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-2.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-3.png)

   >[!CAUTION]
   >
   >Se o número de pessoas qualificadas para executar uma Campanha inteligente exceder o limite definido, ela não será executada.

1. Insira um limite e clique em **[!UICONTROL Salvar]**.

   ![](assets/enable-person-restrictions-for-smart-campaigns-4.png)

   >[!TIP]
   >
   >Desative esse recurso deixando esse campo em branco.

   >[!CAUTION]
   >
   >Esse limite é aplicado a todas as Campanhas inteligentes, mas pode ser substituído no nível da campanha. Saiba como [substituir restrições de pessoa em uma Campanha Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md).

>[!MORELIKETHIS]
>
>[Substituir restrições de pessoa em uma campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/override-person-restrictions-in-a-smart-campaign.md)
