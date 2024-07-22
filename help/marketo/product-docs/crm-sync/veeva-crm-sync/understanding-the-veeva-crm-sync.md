---
description: Noções básicas sobre a sincronização do Veeva CRM - Documentação do Marketo - Documentação do produto
title: Como entender a sincronização do Veeva CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Como entender a sincronização do Veeva CRM {#understanding-the-veeva-crm-sync}

Em algumas etapas fáceis, é fácil executar uma sincronização entre o Adobe Marketo Engage e o Veeva CRM.

## Como a sincronização funciona {#how-the-sync-works}

O Marketo Engage sincroniza com o Veeva CRM o dia todo, todos os dias. Cada sincronização leva algum tempo, pausa por 5 minutos e começa novamente.

>[!NOTE]
>
>A primeira sincronização pode levar horas ou até dias porque o Marketo Engage está copiando todo o banco de dados do Veeva. Depois disso, cada sincronização normalmente leva minutos (algumas vezes segundos) e só sincroniza dados que foram alterados.

![](assets/understanding-the-veeva-sync-1.png)

A sincronização entre Veeva e Marketo Engage é bidirecional somente para campos de Contato no objeto de conta Pessoa. Nesses casos, sempre que você fizer alterações no Veeva ou no Marketo Engage, suas atualizações serão refletidas em ambos os sistemas. Todas as outras sincronizações são apenas de Veeva para Marketo Engage. Clique nos links abaixo para obter detalhes sobre cada um deles.

## O que é sincronizado entre o Marketo Engage e o Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* [Contas Pessoais](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Usuários
* [Chamar e Chamar Objetos de Chave](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Objetos Personalizados](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## O que você deve saber {#things-to-know}

* As [credenciais inseridas no Marketo Engage para Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

* O Veeva CRM é baseado em force.com e a Marketo Engage de experiência avançada com a plataforma é herdada para essa sincronização.

* O Veeva CRM mostra: lead, contato, contas, contas de negócios, oportunidade, campanha e atividade. No entanto, eles não são compatíveis na sincronização com o Marketo Engage.
