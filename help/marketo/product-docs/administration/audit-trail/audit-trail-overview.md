---
unique-page-id: 11377945
description: Visão geral da trilha de auditoria - Documentos do marketing - Documentação do produto
title: Visão geral da trilha de auditoria
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Visão Geral da Trilha de Auditoria {#audit-trail-overview}

A Trilha de auditoria fornece a capacidade de obter um histórico completo (com seis meses de duração) das alterações feitas na sua instância de Marketo.

>[!NOTE]
>
>O histórico de dados de trilha de auditoria começou em 14 de setembro de 2016.

![](assets/one.png)

## O que é a Trilha de Auditoria {#what-is-audit-trail}

A Trilha de auditoria captura, em tempo real, uma lista abrangente de ações e eventos que ocorrem em uma subscrição de marketing. Ele inclui uma forma de autoatendimento de acessar um histórico de dados de seis meses para ajudar a responder perguntas como:

O que aconteceu com esse ativo ou configuração e quem o atualizou pela última vez?

O que o usuário X está aprontando?

Quem está fazendo logon em nossa conta?

## O que nós auditamos {#what-we-audit}

O Marketo irá auditar as ações [criar, editar e eliminar](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) para:

* Projetar ativos de estúdio
* Todos os programas de marketing
* Campanhas inteligentes
* Lista (inteligente/estático)
* Usuários (administrador)
* Funções e permissões (administrador)
* Área de trabalho e partições (administrador)
* Histórico de login do usuário

>[!NOTE]
>
>O Marketo é _e não_ alterações de auditoria feitas na Personalização da Web, Conteúdo Preditivo ou Insight de Vendas no momento.

## Componentes de trilha de auditoria {#audit-trail-components}

A Trilha de auditoria é composta por três componentes.

**1) Trilha de auditoria de  [ativos](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Consulte atividade feita para ativos específicos.

**2) Trilha de auditoria  [do administrador](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Monitore detalhes baseados no usuário.

**3) Histórico de logon  [do usuário](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Veja quem tem feito logon na sua subscrição e quando. Também inclui tentativas de login com falha.

>[!TIP]
>
>Há tanto que você pode auditar usando a Trilha de auditoria, certifique-se de utilizar [Filtragem](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Exportando dados {#exporting-data}

Você só pode visualização 30 dias de dados em sua instância. Para obter (até) o valor de seis meses, use a opção de exportação.

![](assets/two.png)

>[!NOTE]
>
>**Definição**
>
>**Desconhecido:** Na trilha de auditoria, você pode ver o nome e o email de um usuário listados como &quot;Desconhecido&quot;. Isso acontece quando você altera os valores da lista de opções no CRM. Esses valores aparecem nos formulários e landings page do Marketo. Ao fazer essa atualização no lado do CRM, as landings page serão automaticamente projetadas com referência ao formulário. Na trilha de auditoria, capturaremos que a landing page foi redigida, mas o nome e o email do usuário serão exibidos como &quot;Desconhecido&quot;, pois não conseguimos capturar as informações do usuário do lado do CRM.

>[!MORELIKETHIS]
>
>[Ativar Trilha de Auditoria](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
