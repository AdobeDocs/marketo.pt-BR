---
unique-page-id: 10098625
description: Entendendo a  [!DNL Microsoft Dynamics] Sincronização - Documentação do Marketo - Documentação do produto
title: Como entender a sincronização do Microsoft Dynamics
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 2%

---

# Entendendo a sincronização [!DNL Microsoft Dynamics] {#understanding-the-microsoft-dynamics-sync}

Marketo e [!DNL Microsoft Dynamics] vão juntos. Mantemos seus dados de vendas e marketing sincronizados.

>[!CAUTION]
>
>No momento, não oferecemos suporte à atualização da sandbox para a sincronização [!DNL Marketo Dynamics]. Se precisar atualizar sua sandbox do CRM [!DNL Dynamics], uma nova sandbox da Marketo será necessária. Entre em contato com o Gerente de sucesso do cliente para obter mais detalhes.

## Como a sincronização funciona {#how-sync-works}

O Marketo sincroniza dados continuamente com o [!DNL Microsoft Dynamics] o dia todo, todos os dias. Isso é feito usando a sincronização em segundo plano, em lotes, não em tempo real.

>[!NOTE]
>
>A primeira sincronização na sua assinatura leva de minutos a horas, dependendo do tamanho do banco de dados. O Marketo copia todo o banco de dados de [!DNL Dynamics]. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

A sincronização entre o Marketo e o [!DNL Dynamics] é bidirecional para clientes potenciais e contatos. Se você fizer alterações no Marketo ou no [!DNL Dynamics], suas atualizações serão refletidas nos dois sistemas. Todos os outros campos, como contas e oportunidades, são sincronizados apenas unidirecionalmente, de [!DNL Dynamics] para Marketo.

## O que está sincronizado entre o Marketo e o [!DNL Microsoft Dynamics]? {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [Leads](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [Contatos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [Contas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [Usuários](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* Equipes (grupos de usuários do sistema)
* [Oportunidades](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [Entidades personalizadas](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

As [credenciais inseridas no Marketo para [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) são usadas para sincronizar dados.

>[!NOTE]
>
>A cópia da instância não terá suporte se a instância de origem estiver integrada com [!DNL Microsoft Dynamics].
