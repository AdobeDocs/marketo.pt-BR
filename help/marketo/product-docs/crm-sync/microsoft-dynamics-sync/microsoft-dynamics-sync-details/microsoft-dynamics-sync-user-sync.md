---
unique-page-id: 3571840
description: Saiba mais sobre como os dados do usuário são sincronizados do Microsoft Dynamics para o Marketo. Entenda quais campos do proprietário são sincronizados e como usá-los em Smart Lists e ações de fluxo.
title: Microsoft [!DNL Dynamics] Sync -User Sync
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/8H1bMdkhxcvyTuYtHHk00GUy4uycuQ1unsGbZ19AjCM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 160
ht-degree: 0%

---

# Sincronização do Microsoft [!DNL Dynamics]: Sincronização de Usuário {#microsoft-dynamics-sync-user-sync}

O Marketo sincroniza todo o banco de dados com o [!DNL Dynamics]. Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente contas do [!DNL Dynamics].

Você precisará de um usuário dedicado do CRM do Microsoft [!DNL Dynamics] para fins de integração. Chamamos esse usuário de Usuário de sincronização.

## Como os detalhes do usuário são mantidos em sincronia entre os dois sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

A sincronização do usuário é unidirecional - [!DNL Dynamics] para o Marketo. Se você fizer alterações em um usuário no [!DNL Dynamics], elas serão refletidas no Marketo.

## Posso criar um usuário usando o Marketo? {#can-i-create-an-user-using-marketo}

Não. O Marketo não pode criar usuários em [!DNL Dynamics].

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante a instalação. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do [!DNL Dynamics] tem acesso.
