---
unique-page-id: 3571840
description: Sincronização do Microsoft Dynamics - Sincronização do usuário - Documentos do Marketo - Documentação do produto
title: Sincronização do Microsoft Dynamics - Sincronização do usuário
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Sincronização do Microsoft Dynamics: Sincronização de Usuário {#microsoft-dynamics-sync-user-sync}

Você sabia que o Marketo sincroniza todo o banco de dados com o Dynamics? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente as contas dinâmicas.

Você precisará de um usuário dedicado do Microsoft Dynamics CRM para a finalidade da integração. Chamamos esse usuário de Usuário de Sincronização.

## Como os detalhes do usuário são mantidos em sincronia entre os dois sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

A sincronização do usuário é unidirecional - Dinâmica para o Marketo. Se você fizer alterações em um usuário no Dynamics, as alterações serão refletidas no Marketo.

## Posso criar um usuário usando o Marketo? {#can-i-create-an-user-using-marketo}

Nº O Marketo não pode criar usuários no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante a configuração. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.
