---
unique-page-id: 3571836
description: Sincronização do Microsoft Dynamics - Sincronização de contas - Documentos do Marketo - Documentação do produto
title: Sincronização do Microsoft Dynamics - Sincronização de contas
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Sincronização do Microsoft Dynamics: Sincronização de conta {#microsoft-dynamics-sync-account-sync}

Você sabia que o Marketo sincroniza todo o banco de dados com o Dynamics? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente as contas dinâmicas.

## Como as informações são sincronizadas? {#which-way-does-the-information-sync}

Apenas uma maneira: do Dynamics para Marketo.

## Como funcionam as atualizações? {#how-do-the-updates-work}

Se você atualizar um campo Conta para um contato no Marketo, ele alterará os valores de todos os contatos pertencentes a essa conta no Marketo. Ele não sincroniza com o Dynamics. No entanto, na próxima vez que a conta for atualizada no Dynamics, as alterações substituirão todas as informações da conta no Marketo.

## Posso criar uma conta usando o Marketo? {#can-i-create-an-account-using-marketo}

Nº O Marketo não pode criar contas no Dynamics.

## Quais campos serão sincronizados com o Marketo? {#which-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) durante a configuração. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.

## Uma alteração em um campo de conta no Dynamics resulta em um log de atividade de alteração de valor de dados para cada contato?  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

Na maioria das vezes, sim. No entanto, se uma conta tiver mais de 5.000 contatos e um campo nessa conta for alterado no Dynamics, sincronizaremos a alteração, mas não registraremos a atividade para mais de 5.000 contatos.
