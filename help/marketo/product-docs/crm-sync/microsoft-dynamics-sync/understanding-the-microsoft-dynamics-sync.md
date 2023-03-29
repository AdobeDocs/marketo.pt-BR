---
unique-page-id: 10098625
description: Noções básicas sobre a sincronização dinâmica do Microsoft - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre a sincronização do Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Noções básicas sobre a sincronização do Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

O Marketo e o Microsoft Dynamics estão juntos. Mantemos seus dados de vendas e marketing sincronizados.

>[!NOTE]
>
>O Marketo só oferece suporte a certificados SSL compatíveis com o Java 7 no momento.

>[!CAUTION]
>
>No momento, não oferecemos suporte à atualização da caixa de proteção para a Sincronização do Marketo Dynamics. Se você precisar atualizar a caixa de proteção do Dynamics CRM, será necessária uma nova caixa de proteção do Marketo. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

## Como a sincronização funciona {#how-sync-works}

O Marketo sincroniza dados continuamente com o Microsoft Dynamics o dia todo, todos os dias. É feito usando sincronização em segundo plano, em lotes, não em tempo real.

>[!NOTE]
>
>A primeira sincronização na assinatura demora minutos a horas, dependendo do tamanho do banco de dados. O Marketo copia todo o banco de dados do Dynamics. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

A sincronização entre o Marketo e o Dynamics é bidirecional para clientes potenciais e contatos. Se você fizer alterações no Marketo ou no Dynamics, suas atualizações serão refletidas em ambos os sistemas. Todos os outros campos, como contas e oportunidades, são sincronizados apenas de uma maneira, do Dynamics ao Marketo.

## O que é sincronizado entre o Marketo e o Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Contas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuários](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipes (grupos de usuários do sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

O [credenciais inseridas no Marketo para o Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) são usadas para sincronizar dados.

>[!NOTE]
>
>A cópia da instância não é suportada se a instância de origem estiver integrada ao Microsoft Dynamics.
