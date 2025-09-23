---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Sincronização de clientes potenciais - Documentação do Marketo - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de clientes em potencial
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Sincronização de [!DNL Microsoft Dynamics]: Sincronização de Cliente Potencial {#microsoft-dynamics-sync-lead-sync}

A sincronização do Marketo com o [!DNL Dynamics] é super poderosa. Veja os detalhes:

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional. Se você fizer alterações em um cliente potencial no [!DNL Dynamics] ou em uma pessoa no Marketo, sua atualização será refletida em ambos os sistemas.

>[!NOTE]
>
>As exclusões nem sempre são sincronizadas em ambas as direções automaticamente. Consulte [Excluindo um cliente potencial ou contato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## E se forem feitas alterações no mesmo campo, em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, o Marketo vencerá para as pessoas (clientes potenciais) e o [!DNL Dynamics] vencerá para os contatos. Isso ocorre porque consideramos que o departamento de marketing tem autoridade para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM).

## Posso criar um cliente em potencial no [!DNL Dynamics] usando o Marketo? {#can-i-create-a-lead-in-dynamics-using-marketo}

Sim, use a ação de fluxo [[!UICONTROL Sincronizar Pessoa com o Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md). Isso criará um cliente em potencial em [!DNL Dynamics] se ele não existir. Se o lead existir, a etapa de fluxo não executará nenhuma ação.

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;[!UICONTROL Sincronizar Pessoa com o Microsoft]&quot; (somente em uma campanha de disparador), o cliente potencial/contato será criado em tempo real no [!DNL Dynamics].

## Posso forçar manualmente uma sincronização de uma pessoa do Marketo para um cliente potencial no [!DNL Dynamics]? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Não, a sincronização automática em segundo plano é a única maneira de sincronizar atualizações entre o Marketo e o [!DNL Dynamics]. A ação de fluxo [[!UICONTROL Sincronizar Pessoa com Microsoft]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) não forçará a sincronização do cliente potencial.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a instalação.

## O Marketo respeitará as regras de validação [!DNL Dynamics]? {#will-marketo-respect-the-dynamics-validation-rules}

Sim. A sincronização falhará se o formato de dados estiver incorreto ou se faltarem informações de campo obrigatórias. O Marketo registrará o resultado no Registro de atividades da pessoa se isso acontecer.
