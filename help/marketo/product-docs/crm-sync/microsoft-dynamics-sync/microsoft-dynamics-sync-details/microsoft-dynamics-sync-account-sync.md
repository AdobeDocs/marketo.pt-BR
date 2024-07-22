---
unique-page-id: 3571836
description: Microsoft Dynamics Sync — Sincronização de conta — Documentação do Marketo — Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de conta
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronização de Conta {#microsoft-dynamics-sync-account-sync}

Você sabia que o Marketo Engage sincroniza todo o banco de dados com o Dynamics? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketo trata especificamente contas do Dynamics.

## De que forma as informações são sincronizadas? {#which-way-does-the-information-sync}

Somente uma maneira: do Dynamics para o Marketo.

## Como funcionam as atualizações? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, os valores de todos esses contatos que pertencem a essa conta serão alterados no Marketo. Ele não é sincronizado com o Dynamics. No entanto, na próxima vez que a conta for atualizada no Dynamics, as alterações substituirão todas as informações da conta no Marketo.

## Posso criar uma conta usando o Marketo? {#can-i-create-an-account-using-marketo}

Nº O Marketo não pode criar contas no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a instalação. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.

## Uma alteração em um campo de conta no Dynamics resulta em um log de atividade Alterar valor de dados para cada contato?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Principalmente, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no Dynamics, sincronizaremos a alteração, mas não registraremos a atividade para os mais de 5.000 contatos.
