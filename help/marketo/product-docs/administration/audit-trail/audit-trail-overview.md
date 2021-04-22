---
unique-page-id: 11377945
description: Visão geral da trilha de auditoria - Documentos do Marketo - Documentação do produto
title: Visão geral da trilha de auditoria
exl-id: e8aff7b7-72ca-4d4e-9159-56ff65f6345c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Visão geral da trilha de auditoria {#audit-trail-overview}

A Trilha de auditoria fornece a capacidade de obter um histórico completo (com seis meses) das alterações feitas em sua instância do Marketo.

>[!NOTE]
>
>O histórico de dados da trilha de auditoria começou a partir de 14 de setembro de 2016.

![](assets/one.png)

## O que é a Trilha de Auditoria {#what-is-audit-trail}

A Trilha de auditoria captura, em tempo real, uma lista abrangente de ações e eventos que ocorrem em uma assinatura do Marketo. Ele inclui uma maneira de autoatendimento para acessar um histórico de seis meses de dados que ajudam a responder perguntas como:

O que aconteceu com esse ativo ou configuração e quem o atualizou pela última vez?

O que o usuário X está aprontando?

Quem está fazendo logon em nossa conta?

## O que auditamos {#what-we-audit}

A Marketo auditará as ações [criar, editar e excluir](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) para:

* Projetar ativos do estúdio
* Todos os programas Marketo
* Campanhas inteligentes
* Listas (inteligentes/estáticas)
* Usuários (administrador)
* Funções e permissões (administrador)
* Espaço de trabalho e partições (administrador)
* Histórico de logon do usuário

>[!NOTE]
>
>O Marketo é _e não_ alterações de auditoria feitas dentro da Personalização da Web, Conteúdo preditivo ou Insight de vendas no momento.

## Componentes da trilha de auditoria {#audit-trail-components}

A Trilha de auditoria consiste em três componentes.

**1) Trilha de auditoria de  [ativos](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#asset-audit-trail)**

Consulte atividade feita para ativos específicos.

**2) Trilha de auditoria  [do administrador](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md#admin-audit-trail)**

Monitore detalhes com base no usuário.

**3) Histórico de logon  [do usuário](/help/marketo/product-docs/administration/audit-trail/user-login-history.md)**

Veja quem tem feito logon em sua assinatura e quando. Também inclui tentativas com falha de logon.

>[!TIP]
>
>Há tanto que você pode auditar usando a Trilha de auditoria, certifique-se de utilizar [Filtragem](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md)!

## Exportando dados {#exporting-data}

Você só pode visualizar dados correspondentes a 30 dias na sua instância. Para obter (até) seis meses, use a opção de exportação.

![](assets/two.png)

>[!NOTE]
>
>**Definição**
>
>**Desconhecido:** na trilha de auditoria, você pode ver o nome e o email de um usuário listados como &quot;Desconhecido&quot;. Isso acontece quando você faz uma alteração nos valores da lista de opções no seu CRM. Esses valores são exibidos nos formulários Marketo e nas páginas de aterrissagem. Fazer essa atualização no lado do CRM criará automaticamente suas landing pages que fazem referência ao formulário. Na trilha de auditoria, capturaremos que a landing page foi redigida, mas o nome do usuário e o email serão exibidos como &quot;Desconhecido&quot;, pois não podemos capturar as informações do usuário do lado do CRM.

>[!MORELIKETHIS]
>
>[Ativar Trilha de Auditoria](/help/marketo/product-docs/administration/audit-trail/enable-audit-trail.md)
