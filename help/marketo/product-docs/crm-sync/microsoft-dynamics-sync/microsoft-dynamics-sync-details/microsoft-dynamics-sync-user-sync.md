---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Sincronização do Usuário - Documentos do Marketing - Documentação do Produto
title: Microsoft Dynamics Sync - Sincronização do Usuário
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização do usuário {#microsoft-dynamics-sync-user-sync}

Você sabia que o Marketo sincroniza todo seu banco de dados com o Dynamics? Sincroniza, então aguarda 5 minutos e sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketing trata especificamente as contas dinâmicas.

Você precisará de um usuário dedicado do Microsoft Dynamics CRM para a finalidade da integração. Chamamos esse usuário de Usuário de Sincronização.

## Como os detalhes do usuário são mantidos em sincronia entre os dois sistemas? {#how-are-user-details-kept-in-sync-between-the-two-systems}

A sincronização do usuário é unidirecional - Dinâmica para o Marketing. Se você fizer alterações em um usuário no Dynamics, as alterações serão refletidas no Marketo.

## É possível criar um usuário usando o Marketo? {#can-i-create-an-user-using-marketo}

Não. O Marketo não pode criar usuários no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronizar](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante a configuração. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.
