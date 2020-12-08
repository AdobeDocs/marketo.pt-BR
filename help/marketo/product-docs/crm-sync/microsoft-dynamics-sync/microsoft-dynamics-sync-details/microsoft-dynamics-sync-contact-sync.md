---
unique-page-id: 3571833
description: Microsoft Dynamics Sync - Sincronização de Contato - Documentos do Marketing - Documentação do Produto
title: Microsoft Dynamics Sync - Sincronização de Contato
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização de contato {#microsoft-dynamics-sync-contact-sync}

Você sabia que o Marketo sincroniza todo seu banco de dados com o Dynamics? Sincroniza, então aguarda 5 minutos e sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como o Marketing trata especificamente os Contatos Dinâmicos.

## Como os detalhes são mantidos em sincronia entre os dois sistemas? {#how-are-details-kept-in-sync-between-the-two-systems}

A sincronização de contato é bidirecional. Se você fizer alterações em um contato no Dynamics ou em uma pessoa no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se forem feitas alterações no mesmo campo em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora seja raro, o Marketo ganhará por pessoas e o Dynamics ganhará por contatos. Isso porque consideramos o departamento de marketing autoritativo para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM).

## É possível criar um contato usando o Marketo? {#can-i-create-a-contact-using-marketo}

Sim. [Veja como](microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md).

>[!NOTE]
>
>Ao usar a ação de fluxo &quot;Sincronizar Pessoa com a Microsoft&quot; (somente em uma campanha de disparo), o cliente potencial/contato será criado em tempo real no Dynamics.

## Posso forçar manualmente uma sincronização de uma pessoa ou de um contato? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Não, a sincronização em segundo plano automatizada é a única maneira de sincronizar atualizações entre o Marketo e o Dynamics. A Pessoa de [sincronização com a Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) não forçará uma sincronização do cliente potencial.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

É possível [selecionar campos para sincronização](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante a configuração. Mas o Marketo só sincronizará os campos aos quais o usuário de sincronização do Dynamics tem acesso.

## O Marketo respeitará as regras de validação do Dynamics? {#will-marketo-respect-the-dynamics-validation-rules}

Sim, se houver um conflito, registrará o resultado no Registro de Atividades de clientes potenciais.
