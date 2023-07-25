---
unique-page-id: 4719283
description: Noções básicas sobre a sincronização do Salesforce - Documentação do Marketo - Documentação do produto
title: Como entender a sincronização do Salesforce
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Como entender a sincronização do Salesforce {#understanding-the-salesforce-sync}

Marketo e Salesforce se juntam como ervilhas e cenouras. Mantemos seus dados de vendas e marketing sincronizados.

## Como a sincronização funciona {#how-sync-works}

O Marketo sincroniza com o Salesforce o dia todo, todos os dias. Cada sincronização leva algum tempo, pausa por 5 minutos e começa novamente.

>[!NOTE]
>
>A primeira sincronização na sua assinatura pode levar horas ou até mesmo dias, pois o Marketo está copiando todo o banco de dados do Salesforce. Depois disso, cada sincronização normalmente leva segundos ou minutos e sincroniza apenas os dados que foram alterados.

![](assets/sync-illustration.png)

A sincronização entre o Salesforce e o Marketo é bidirecional somente para clientes potenciais, contatos e campanhas do Salesforce. Nesses casos, sempre que você fizer alterações no Salesforce ou no Marketo, suas atualizações serão refletidas nos dois sistemas. Todas as outras sincronizações são somente do Salesforce para o Marketo. Clique nos links abaixo para obter detalhes sobre cada um deles.

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
>A variável [credenciais inseridas no Marketo para Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) são usados para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

A sincronização da Marketo com o Salesforce é a mais poderosa desse tipo no mundo. Parece mágica, muda-se e logo o outro sistema se atualiza.
