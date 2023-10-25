---
unique-page-id: 3571833
description: Microsoft Dynamics Sync -Sincronização De Contato - Documentação Do Marketo - Documentação Do Produto
title: Microsoft Dynamics Sync - Sincronização de contato
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Microsoft Dynamics Sync: Sincronização de Contatos {#microsoft-dynamics-sync-contact-sync}

Você sabia que o Marketo Engage sincroniza todo o banco de dados com o Dynamics? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketo trata especificamente Contatos do Dynamics.

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização de contatos é bidirecional. Se você fizer alterações em um contato no Dynamics ou em uma pessoa no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se forem feitas alterações no mesmo campo, em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, o Marketo vencerá para as pessoas e o Dynamics vencerá para os contatos. Isso ocorre porque consideramos que o departamento de marketing tem autoridade para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM).

## Posso criar um contato usando o Marketo? {#can-i-create-a-contact-using-marketo}

Sim. [Veja como](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;Sincronizar pessoa com o Microsoft&quot; (somente em uma campanha de acionador), o lead/contato será criado em tempo real no Dynamics.

## Posso forçar manualmente uma sincronização de uma pessoa ou contato? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Não, a sincronização automática em segundo plano é a única maneira de sincronizar atualizações entre o Marketo e o Dynamics. A variável [Sincronizar pessoa com o Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} não forçará uma sincronização do lead.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a configuração. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.

## O Marketo respeitará as regras de validação do Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sim, se houver um conflito, ele registrará o resultado no Registro de atividades dos clientes potenciais.
