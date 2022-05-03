---
description: Noções básicas sobre a sincronização do Veeva CRM - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre a sincronização do Veeva CRM
hide: true
hidefromtoc: true
source-git-commit: 93e6bb881e10cda26b3a33569dc67627d628a178
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Noções básicas sobre a sincronização do Veeva CRM {#understanding-the-veeva-crm-sync}

Em alguns passos fáceis, é fácil executar uma sincronização entre o Adobe Marketo Engage e o CRM Veeva.

## Como a sincronização funciona {#how-the-sync-works}

O Marketo Engage sincroniza com Veeva CRM o dia todo, todos os dias. Cada sincronização leva algum tempo, é pausada por 5 minutos e começa novamente.

>[!NOTE]
>
>A primeira sincronização pode levar horas ou até dias, porque o Marketo Engage está copiando todo o banco de dados de Veeva. Depois disso, cada sincronização normalmente leva minutos (algumas vezes segundos) e sincroniza apenas os dados que foram alterados.

![](assets/understanding-the-veeva-sync-1.png)

A sincronização entre Veeva e Marketo Engage é bidirecional somente para campos de Contato no objeto de conta Pessoa. Nesses casos, sempre que você fizer alterações no Veeva ou no Marketo Engage, suas atualizações serão refletidas em ambos os sistemas. Todas as outras sincronizações são de Veeva somente para Marketo Engage. Clique nos links abaixo para obter detalhes sobre cada um.

## O que é sincronizado entre o Marketo Engage e Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* Contas de pessoa
* Usuários
* Chamar e chamar objetos-chave
* Objetos personalizados

## O que saber {#things-to-know}

* As credenciais inseridas no Marketo Engage para Veeva são usadas para sincronizar dados. Somente os dados aos quais essas credenciais têm acesso serão incluídos.

* Todo CRM é baseado em force.com e a rica experiência que o Marketo Engage tem com a plataforma é herdada nesta sincronização.

* O CRM de Veeva mostra: Cliente Potencial, Contato, Contas (Contas Comerciais, Oportunidade, Campanha e Atividade). No entanto, eles não são compatíveis na sincronização com o Marketo Engage.
