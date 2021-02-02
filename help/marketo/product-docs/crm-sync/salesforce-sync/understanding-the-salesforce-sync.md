---
unique-page-id: 4719283
description: Como entender a sincronização do Salesforce - Documentos do Marketing - Documentação do produto
title: Como entender a sincronização do Salesforce
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Como entender a sincronização do Salesforce {#understanding-the-salesforce-sync}

O Marketo e a Salesforce se unem como ervilhas e cenouras. Mantemos seus dados de vendas e marketing sincronizados.

## Como a sincronização funciona {#how-sync-works}

O Marketo sincroniza com o Salesforce o dia todo, todos os dias. Cada sincronização leva algum tempo e, em seguida, pausa por 5 minutos e, em seguida, start novamente.

>[!NOTE]
>
>A primeira sincronização na sua subscrição pode levar horas ou até dias, porque o Marketo está copiando todo o banco de dados do Salesforce. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

![](assets/sync-illustration.png)

A sincronização entre Salesforce e Marketo é bidirecional somente para clientes potenciais, contatos e campanhas Salesforce. Nesses casos, sempre que você fizer alterações no Salesforce ou no Marketing, suas atualizações serão refletidas em ambos os sistemas. Todas as outras sincronizações são somente do Salesforce para o Marketo. Clique nos links abaixo para obter detalhes sobre cada um.

## O que é sincronizado entre o Marketo e o Salesforce? {#what-is-synced-between-marketo-and-salesforce}

* [Clientes potenciais](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
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

A sincronia de Marketo com Salesforce é a mais poderosa do gênero no mundo. Parece mágica. é feita uma mudança e o outro sistema estará em breve atualizado.
