---
unique-page-id: 3571836
description: Microsoft Dynamics Sync - Sincronização de Conta - Documentos do Marketing - Documentação do Produto
title: Microsoft Dynamics Sync - Sincronização de Conta
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização de conta {#microsoft-dynamics-sync-account-sync}

Você sabia que o Marketo sincroniza todo seu banco de dados com o Dynamics? Sincroniza, então aguarda 5 minutos e sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketing trata especificamente as contas dinâmicas.

## De que forma as informações são sincronizadas? {#which-way-does-the-information-sync}

Apenas de uma maneira: da Dinâmica para o Marketo.

## Como as atualizações funcionam? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, ele alterará os valores de todos os contatos que pertencem a essa conta no Marketo. Não sincroniza com o Dynamics. No entanto, na próxima vez que a conta for atualizada no Dynamics, as alterações substituirão todas as informações da conta no Marketo.

## É possível criar uma conta usando o Marketo? {#can-i-create-an-account-using-marketo}

Não. O Marketo não pode criar contas no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante a configuração. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.

## Uma alteração em um campo de conta no Dynamics resulta em um log de Atividade de valores de dados de alteração para cada contato?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Na maioria das vezes, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no Dynamics, nós sincronizaremos a alteração, mas não registraremos a atividade dos mais de 5.000 contatos.
