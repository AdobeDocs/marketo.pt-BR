---
unique-page-id: 10098625
description: Noções básicas sobre a sincronização do Microsoft Dynamics - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre a sincronização do Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 2%

---

# Noções básicas sobre a sincronização do Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

O Marketo Engage e o Microsoft Dynamics vão juntos. Mantemos seus dados de vendas e marketing sincronizados.

>[!NOTE]
>
>No momento, o Marketo só oferece suporte a certificados SSL compatíveis com o Java 7.

>[!CAUTION]
>
>No momento, não oferecemos suporte à atualização de sandbox para o Marketo Dynamics Sync. Se você precisar atualizar sua sandbox do Dynamics CRM, uma nova sandbox do Marketo será necessária. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

## Como a sincronização funciona {#how-sync-works}

A Marketo sincroniza dados continuamente com o Microsoft Dynamics todos os dias. Isso é feito usando a sincronização em segundo plano, em lotes, não em tempo real.

>[!NOTE]
>
>A primeira sincronização na sua assinatura leva de minutos a horas, dependendo do tamanho do banco de dados. O Marketo copia todo o banco de dados do Dynamics. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

A sincronização entre o Marketo e o Dynamics é bidirecional para clientes potenciais e contatos. Se você fizer alterações no Marketo ou no Dynamics, suas atualizações serão refletidas nos dois sistemas. Todos os outros campos, como contas e oportunidades, são sincronizados apenas de uma maneira, do Dynamics para o Marketo.

## O que é sincronizado entre o Marketo e o Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Contas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuários](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipes (grupos de usuários do sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

A variável [credenciais inseridas no Marketo for Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) são usados para sincronizar dados.

>[!NOTE]
>
>A cópia de instância não terá suporte se a instância de origem estiver integrada ao Microsoft Dynamics.
