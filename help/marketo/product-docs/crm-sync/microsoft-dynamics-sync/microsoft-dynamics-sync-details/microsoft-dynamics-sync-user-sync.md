---
unique-page-id: 3571840
description: Microsoft [!DNL Dynamics] Sync -User Sync - Documentação do Marketo - Documentação do produto
title: Microsoft [!DNL Dynamics] Sync -User Sync
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---

# Sincronização do Microsoft [!DNL Dynamics]: Sincronização de Usuário {#microsoft-dynamics-sync-user-sync}

Você sabia que o Marketo sincroniza todo o seu banco de dados com o [!DNL Dynamics]? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente contas do [!DNL Dynamics].

Você precisará de um usuário dedicado do CRM do Microsoft [!DNL Dynamics] para fins de integração. Chamamos esse usuário de Usuário de sincronização.

## Como os detalhes do usuário são mantidos em sincronia entre os dois sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

A sincronização do usuário é unidirecional - [!DNL Dynamics] para o Marketo. Se você fizer alterações em um usuário no [!DNL Dynamics], elas serão refletidas no Marketo.

## Posso criar um usuário usando o Marketo? {#can-i-create-an-user-using-marketo}

Não. O Marketo não pode criar usuários em [!DNL Dynamics].

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante a instalação. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do [!DNL Dynamics] tem acesso.
