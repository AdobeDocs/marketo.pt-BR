---
unique-page-id: 10098625
description: Noções Gerais da Microsoft Dynamics Sync - Documentos do Marketing - Documentação do produto
title: Como entender o Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Noções Gerais da Sincronização do Microsoft Dynamics {#understanding-the-microsoft-dynamics-sync}

O Marketo e o Microsoft Dynamics estão juntos. Mantemos seus dados de vendas e marketing sincronizados.

>[!NOTE]
>
>O Marketo suporta somente certificados SSL compatíveis com o Java 7 no momento.

## Como a sincronização funciona {#how-sync-works}

O Marketo sincroniza dados continuamente com o Microsoft Dynamics o dia todo, todos os dias. É feito usando sincronização em segundo plano, em lotes, não em tempo real.

>[!NOTE]
>
>A primeira sincronização na sua subscrição leva minutos a horas, dependendo do tamanho do banco de dados. O Marketo copia todo o banco de dados do Dynamics. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

A sincronização entre o Marketing e o Dynamics é bidirecional para clientes potenciais e contatos. Se você fizer alterações no Marketo ou no Dynamics, suas atualizações serão refletidas em ambos os sistemas. Todos os outros campos, como contas e oportunidades, são sincronizados apenas de uma maneira, da Dinâmica ao Mercado.

## O que é sincronizado entre o Marketo e o Microsoft Dynamics? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Clientes potenciais](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatos](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Contas](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuários](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipes (grupos de SystemUsers)
* [Oportunidades](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>As credenciais [inseridas no Marketo para Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) são usadas para sincronizar dados.

Há muitas nuances e recursos sobre a sincronização do Dynamics. Confira os detalhes na seção [Detalhes do Microsoft Dynamics Sync](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details).

>[!CAUTION]
>
>No momento, não oferecemos suporte à atualização da caixa de proteção para a Sincronização Dinâmica do Marketing. Se precisar atualizar sua caixa de proteção do Dynamics CRM, uma nova caixa de proteção do Marketo será necessária. Entre em contato com o Gerente de sucesso do cliente para obter mais detalhes.

>[!MORELIKETHIS]
>
>* [Sincronizar configuração](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Detalhes da Sincronização do Microsoft Dynamics](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

