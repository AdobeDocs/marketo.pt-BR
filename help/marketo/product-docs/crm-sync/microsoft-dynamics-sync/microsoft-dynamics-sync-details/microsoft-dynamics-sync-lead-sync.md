---
unique-page-id: 3571848
description: Microsoft Dynamics Sync — Sincronização De Clientes Potenciais — Documentação Do Marketo — Documentação Do Produto
title: Microsoft Dynamics Sync - Sincronização De Clientes Potenciais
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Microsoft Dynamics Sync: sincronização de clientes potenciais {#microsoft-dynamics-sync-lead-sync}

A sincronização do Marketo Engage para o Dynamics é superpoderosa. Aqui estão os detalhes.

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional. Se você fizer alterações em um cliente potencial no Dynamics ou em uma pessoa no Marketo, sua atualização será refletida em ambos os sistemas.

>[!NOTE]
>
>As exclusões nem sempre são sincronizadas em ambas as direções automaticamente. Consulte [Excluindo um Cliente Potencial ou Contato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## E se forem feitas alterações no mesmo campo, em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, o Marketo vencerá para as pessoas (clientes potenciais) e o Dynamics vencerá para os contatos. Isso ocorre porque consideramos que o departamento de marketing tem autoridade para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM).

## Posso criar um cliente potencial no Dynamics usando o Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sim, use o [Sincronizar pessoa com o Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} ação de fluxo. Isso criará um cliente potencial no Dynamics se o cliente potencial não existir. Se o lead existir, a etapa de fluxo não executará nenhuma ação.

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;Sincronizar pessoa com o Microsoft&quot; (somente em uma campanha de acionador), o lead/contato será criado em tempo real no Dynamics.

## Posso forçar manualmente uma sincronização de uma pessoa do Marketo para um cliente potencial no Dynamics? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Não, a sincronização automática em segundo plano é a única maneira de sincronizar atualizações entre o Marketo e o Dynamics. A variável [Sincronizar pessoa com o Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} a ação de fluxo não forçará uma sincronização do lead.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a configuração.

## O Marketo respeitará as regras de validação do Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou se faltarem informações de campo obrigatórias. O Marketo registrará o resultado no Registro de atividades da pessoa se isso acontecer.
