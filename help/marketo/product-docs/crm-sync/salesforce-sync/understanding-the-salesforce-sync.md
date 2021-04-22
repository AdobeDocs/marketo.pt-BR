---
unique-page-id: 4719283
description: Noções básicas sobre a sincronização do Salesforce - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre a sincronização do Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Noções básicas sobre a sincronização do Salesforce {#understanding-the-salesforce-sync}

Marketo e Salesforce se unem como ervilhas e cenouras. Mantemos seus dados de vendas e marketing sincronizados.

## Como a sincronização funciona {#how-sync-works}

O Marketo sincroniza com o Salesforce o dia todo, todos os dias. Cada sincronização leva algum tempo e, em seguida, é pausada por 5 minutos, em seguida, é iniciada novamente.

>[!NOTE]
>
>A primeira sincronização na assinatura pode levar horas ou até dias, pois a Marketo está copiando todo o banco de dados do Salesforce. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

![](assets/sync-illustration.png)

A sincronização entre o Salesforce e o Marketo é bidirecional apenas para campanhas de leads, contatos e Salesforce. Nesses casos, sempre que você fizer alterações no Salesforce ou no Marketo, suas atualizações serão refletidas em ambos os sistemas. Todas as outras sincronizações são somente do Salesforce para o Marketo. Clique nos links abaixo para obter detalhes sobre cada um.

## O que é sincronizado entre o Marketo e o Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Leads](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [Contatos](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [Contas](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [Usuários](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [Oportunidades](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Campanhas do Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [Objetos personalizados](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [Atividade](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>As credenciais [inseridas no Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

A sincronização Marketo com Salesforce é a mais poderosa do seu tipo no mundo. Parece mágica. é feita uma mudança e o outro sistema está em breve atualizado.
