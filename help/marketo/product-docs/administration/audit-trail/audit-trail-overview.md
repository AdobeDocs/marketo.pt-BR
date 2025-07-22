---
unique-page-id: 11377945
description: Trilha de auditoria] Visão geral - Documentação do Marketo - Documentação do produto
title: Visão geral da trilha de auditoria
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
feature: Audit Trail
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Visão geral da trilha de auditoria {#audit-trail-overview}

A Trilha de auditoria oferece a capacidade de obter um histórico completo (equivalente a seis meses) das alterações feitas na instância do Marketo.

>[!NOTE]
>
>O histórico de dados da trilha de auditoria começou em 14 de setembro de 2016.

![](assets/audit-trail-overview-1.png)

## O que é trilha de auditoria {#what-is-audit-trail}

A Trilha de auditoria captura em tempo real uma lista abrangente de ações e eventos que ocorrem em uma assinatura do Marketo. Ele inclui uma forma de autoatendimento para acessar um histórico de dados de seis meses para ajudar a responder a perguntas como:

O que aconteceu com esse ativo ou configuração e quem o atualizou pela última vez?

O que o usuário X tem feito?

Quem está fazendo login em nossa conta?

## O que auditamos {#what-we-audit}

A Marketo auditará as [ações de criação, edição e exclusão](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) para:

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

Veja quem está fazendo logon na sua assinatura e quando. Também inclui tentativas de logon com falha.

>[!TIP]
>
>Há tanta coisa que você pode auditar usando a Trilha de Auditoria; certifique-se de utilizar a [Filtragem](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Exportando dados {#exporting-data}

Você só poderá visualizar os dados correspondentes a 30 dias na sua instância. Para obter (até) seis meses, use a opção de exportação.

![](assets/two.png)

>[!NOTE]
>
>**Definição**
>
>**Desconhecido:** Em [!DNL Webhook], você pode ver o nome de usuário e o email listados como &quot;Desconhecido&quot;. Isso acontece quando você faz uma alteração nos valores da lista de seleção no CRM. Esses valores aparecem nos formulários e nas páginas de aterrissagem do Marketo. Essa atualização no lado do CRM rascunhará automaticamente as páginas de aterrissagem que fazem referência ao formulário. Em [!DNL Webhook], capturaremos que a página de aterrissagem foi rascunhada, mas o nome do usuário e o email serão exibidos como &quot;Desconhecido&quot;, pois não poderemos capturar as informações do usuário no lado do CRM.

>[!MORELIKETHIS]
>
>[Habilitar Trilha de Auditoria](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
