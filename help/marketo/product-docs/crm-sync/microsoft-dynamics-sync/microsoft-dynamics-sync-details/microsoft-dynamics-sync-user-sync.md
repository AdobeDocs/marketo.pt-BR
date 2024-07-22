---
unique-page-id: 3571840
description: Microsoft Dynamics Sync — Sincronização de usuários — Documentação do Marketo — Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de usuários
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronização de usuários {#microsoft-dynamics-sync-user-sync}

Você sabia que o Marketo Engage sincroniza todo o banco de dados com o Dynamics? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketo trata especificamente contas do Dynamics.

Você precisará de um usuário dedicado do Microsoft Dynamics CRM para fins de integração. Chamamos esse usuário de Usuário de sincronização.

## Como os detalhes do usuário são mantidos em sincronia entre os dois sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

A sincronização do usuário é unidirecional - Dinâmica para o Marketo. Se você fizer alterações em um usuário no Dynamics, elas serão refletidas no Marketo.

## Posso criar um usuário usando o Marketo? {#can-i-create-an-user-using-marketo}

Nº O Marketo não pode criar usuários no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a instalação. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.
