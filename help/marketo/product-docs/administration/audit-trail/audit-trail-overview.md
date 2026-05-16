---
unique-page-id: 11377945
description: Visão geral da Trilha de auditoria e como ela captura um histórico de seis meses de alterações e atividade de logon na instância do Marketo.
title: Visão geral da trilha de auditoria
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
TQID: https://experienceleague.adobe.com/4MTpv09ZFWkX6tirnq7ZIABSkfoz07qljcUUORwYNn8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 2%

---

# Visão geral da trilha de auditoria {#audit-trail-overview}

A Trilha de auditoria oferece a capacidade de obter um histórico completo (equivalente a seis meses) das alterações feitas na instância do Marketo.

>[!NOTE]
>
>O histórico de dados da trilha de auditoria começou em 14 de setembro de 2016.

![](assets/audit-trail-overview-1.png)

## O que é trilha de auditoria {#what-is-audit-trail}

A Trilha de auditoria captura em tempo real uma lista abrangente de ações e eventos que ocorrem em uma assinatura do Marketo. Ele inclui uma forma de autoatendimento para acessar um histórico de dados de seis meses para ajudar a responder a perguntas como:

&quot;O que aconteceu com esse ativo ou configuração e quem o atualizou pela última vez?&quot;

&quot;O que o usuário X tem feito?&quot;

&quot;Quem está fazendo logon em nossa conta?&quot;

## O que auditamos {#what-we-audit}

A Marketo audita as ações [criar, editar e excluir](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) para:

* Ativos do design studio
* Todos os programas do Marketo
* Campanhas inteligentes
* Listas (inteligente/estática)
* Usuários (admin)
* Funções e permissões (admin)
* Workspace e partições (admin)
* Histórico de logon do usuário

>[!NOTE]
>
>O Marketo _não_ está auditando alterações feitas no Web Personalization, Predictive Content ou Sales Insight no momento.

## Componentes da trilha de auditoria {#audit-trail-components}

A Trilha de auditoria consiste em três componentes.

**1) [Trilha de auditoria do ativo](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Consulte atividade realizada em ativos específicos.

**2) [Trilha de Auditoria do Administrador](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Monitore detalhes com base no usuário.

**3) [Histórico de Logon do Usuário](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Veja quem está fazendo logon na sua assinatura e quando (também inclui tentativas de logon com falha).

>[!TIP]
>
>Como há tanta coisa que você pode auditar usando a Trilha de Auditoria, [filtrar](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md) pode economizar muito tempo.

## Exportando dados {#exporting-data}

Você só poderá visualizar os dados correspondentes a 30 dias na sua instância. Para obter (até) seis meses, use a opção de exportação.

![](assets/two.png)

>[!NOTE]
>
>**Definição**
>
>**Desconhecido:** Em [!DNL Webhook], você pode ver o nome de usuário e o email listados como &quot;Desconhecido&quot;. Isso acontece quando você faz uma alteração nos valores da lista de seleção no CRM. Esses valores aparecem nos formulários e nas páginas de aterrissagem do Marketo. Essa atualização no lado do CRM rascunhará automaticamente as páginas de aterrissagem que fazem referência ao formulário. Em [!DNL Webhook], o Marketo captura que a página de aterrissagem foi rascunhada, mas o nome e email do usuário serão exibidos como &quot;Desconhecido&quot;, já que o Marketo não pode capturar as informações do usuário no lado do CRM.

>[!MORELIKETHIS]
>
>[Habilitar Trilha de Auditoria](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
