---
description: Entendendo a  [!DNL Veeva] Sincronização do CRM - Documentação do Marketo - Documentação do produto
title: Compreendendo a  [!DNL Veeva] Sincronização do CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Compreendendo a Sincronização do CRM [!DNL Veeva] {#understanding-the-veeva-crm-sync}

Em algumas etapas fáceis, é fácil executar uma sincronização entre o Adobe Marketo Engage e o CRM [!DNL Veeva].

## Como a sincronização funciona {#how-the-sync-works}

O Marketo Engage sincroniza com o [!DNL Veeva] CRM todos os dias. Cada sincronização leva algum tempo, pausa por 5 minutos e começa novamente.

>[!NOTE]
>
>A primeira sincronização pode levar horas ou até mesmo dias porque o Marketo Engage está copiando todo o banco de dados de [!DNL Veeva]. Depois disso, cada sincronização normalmente leva minutos (algumas vezes segundos) e só sincroniza dados que foram alterados.

![](assets/understanding-the-veeva-sync-1.png)

A sincronização entre [!DNL Veeva] e o Marketo Engage é bidirecional somente para campos de Contato no objeto de conta de Pessoa. Nesses casos, sempre que você fizer alterações no [!DNL Veeva] ou no Marketo Engage, suas atualizações serão refletidas nos dois sistemas. Todas as outras sincronizações são somente do [!DNL Veeva] para o Marketo Engage. Clique nos links abaixo para obter detalhes sobre cada um deles.

## O que está sincronizado entre o Marketo Engage e o [!DNL Veeva] {#what-is-synced-between-marketo-engage-and-veeva}

* [Contas Pessoais](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Usuários
* [Chamar e Chamar Objetos de Chave](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Objetos Personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## O que você deve saber {#things-to-know}

* As [credenciais inseridas no Marketo Engage para [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

* O CRM do [!DNL Veeva] é baseado em force.com e a experiência avançada que o Marketo Engage tem com a plataforma é herdada para essa sincronização.

* O Veeva CRM mostra: lead, contato, contas, contas de negócios, oportunidade, campanha e atividade. No entanto, elas não são compatíveis com a sincronização com o Marketo Engage.
