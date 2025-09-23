---
unique-page-id: 3571833
description: Microsoft Dynamics Sync -Sincronização de contatos - Documentação do Marketo - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de contato
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Sincronização de [!DNL Microsoft Dynamics]: Sincronização de Contatos {#microsoft-dynamics-sync-contact-sync}

Você sabia que o Marketo sincroniza todo o seu banco de dados com o [!DNL Dynamics]? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente Contatos do [!DNL Dynamics].

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização de contatos é bidirecional. Se você fizer alterações em um contato do [!DNL Dynamics] ou em uma pessoa do Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se forem feitas alterações no mesmo campo, em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora isso seja raro, o Marketo vencerá para as pessoas e [!DNL Dynamics] para os contatos. Isso ocorre porque consideramos que o departamento de marketing tem autoridade para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM).

## Posso criar um contato usando o Marketo? {#can-i-create-a-contact-using-marketo}

Sim. [Veja como](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;Sincronizar Pessoa com o Microsoft&quot; (somente em uma campanha de acionador), o cliente potencial/contato será criado em tempo real no [!DNL Dynamics].

## Posso forçar manualmente uma sincronização de uma pessoa ou contato? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Não, a sincronização automática em segundo plano é a única maneira de sincronizar atualizações entre o Marketo e o [!DNL Dynamics]. A [Pessoa de Sincronização para o Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) não forçará uma sincronização do lead.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) durante a instalação. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do [!DNL Dynamics] tem acesso.

## O Marketo respeitará as regras de validação [!DNL Dynamics]? {#will-marketo-respect-the-dynamics-validation-rules}

Sim, se houver um conflito, ele registrará o resultado no Registro de atividades dos clientes potenciais.
