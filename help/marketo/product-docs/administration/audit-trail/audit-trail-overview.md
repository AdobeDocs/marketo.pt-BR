---
unique-page-id: 11377945
description: Visão geral da trilha de auditoria - Documentos do marketing - Documentação do produto
title: Visão geral da trilha de auditoria
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---


# Visão geral da trilha de auditoria {#audit-trail-overview}

A Trilha de auditoria fornece a capacidade de obter um histórico completo (com seis meses de duração) das alterações feitas na sua instância de Marketo.

>[!NOTE]
>
>O histórico de dados de trilha de auditoria começou em 14 de setembro de 2016.

![](assets/one.png)

## O que é a Trilha de auditoria {#what-is-audit-trail}

A Trilha de auditoria captura, em tempo real, uma lista abrangente de ações e eventos que ocorrem em uma subscrição de marketing. Ele inclui uma forma de autoatendimento de acessar um histórico de dados de seis meses para ajudar a responder perguntas como:

O que aconteceu com esse ativo ou configuração e quem o atualizou pela última vez?

O que o usuário X está aprontando?

Quem está fazendo logon em nossa conta?

## O que nós auditamos {#what-we-audit}

O Marketo irá auditar as ações de [criação, edição e exclusão](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail) para:

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
>O Marketo **não** está auditando as alterações feitas na Personalização da Web, Conteúdo preditivo ou Insight de vendas no momento.

## Componentes de trilha de auditoria {#audit-trail-components}

A Trilha de auditoria é composta por três componentes.

**1) Trilha de auditoria de [ativos](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AssetAuditTrail)**

Consulte atividade feita para ativos específicos.

**2) Trilha de auditoria [do administrador](http://docs.marketo.com/display/DOCS/Change+Details+in+Audit+Trail#ChangeDetailsinAuditTrail-AdminAuditTrail)**

Monitore detalhes baseados no usuário.

**3) Histórico de logon [do usuário](http://docs.marketo.com/display/DOCS/User+Login+History)**

Veja quem tem feito logon na sua subscrição e quando. Também inclui tentativas de login com falha.

>[!TIP]
>
>Há tanto que você pode auditar usando a Trilha de auditoria, certifique-se de utilizar a [Filtragem](http://docs.marketo.com/display/DOCS/Filtering+in+Audit+Trail)!

## Exportação de dados {#exporting-data}

Você só pode visualização 30 dias de dados em sua instância. Para obter (até) o valor de seis meses, use a opção de exportação.

![](assets/two.png)

>[!NOTE]
>
>**Definição**
>
>**Desconhecido:** Na trilha de auditoria, você pode ver o nome e o email de um usuário listados como &quot;Desconhecido&quot;. Isso acontece quando você altera os valores da lista de opções no CRM. Esses valores aparecem nos formulários e landings page do Marketo. Ao fazer essa atualização no lado do CRM, as landings page serão automaticamente projetadas com referência ao formulário. Na trilha de auditoria, capturaremos que a landing page foi redigida, mas o nome e o email do usuário serão exibidos como &quot;Desconhecido&quot;, pois não conseguimos capturar as informações do usuário do lado do CRM.

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Ativar Trilha de Auditoria](enable-audit-trail.md)

>



