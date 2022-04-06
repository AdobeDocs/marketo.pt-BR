---
description: Adicionar conjunto de permissões de insight de vendas - Documentos da Marketo - Documentação do produto
title: Adicionar Conjunto de Permissões de Insight de Vendas
hide: true
hidefromtoc: true
source-git-commit: 2ac0ef0b715eb2acd03fe2c5ad4cfee8daeef4f6
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# Adicionar Conjunto de Permissões de Insight de Vendas {#add-sales-insight-permission-set}

Use as etapas a seguir para adicionar acesso aos recursos do Sales Insight no Salesforce. Aplicável ao Salesforce Classic e ao Iluminação

>[!PREREQUISITES]
>
>[Atualize seu pacote do Sales Insight Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target=&quot;_blank&quot;} para a versão 1.8000 ou superior para usar esse recurso.

>[!IMPORTANT]
>
>Se você já concedeu acesso ao Sales Insight a todos os perfis e/ou implementou o Sales Insight para todos os usuários, é necessário [remover acesso de nível de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target=&quot;_blank&quot;} para usar esse conjunto de permissões.

## Visão geral {#overview}

A permissão &quot;Aplicativo Marketo&quot; é parte do pacote Sales Insight Salesforce . It includes access to the below mentioned objects, apex classes, and visualforce pages. These are required to access all Sales Insight features.

**Object Settings**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Read, Create, Edit, Delete, View All, Modify All</td> 
  </tr> 
  <tr> 
   <td>Detalhes de melhores opções</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>Melhores visualizações</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Read, Create, Edit, Delete, View All, Modify All</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>InterestingMomentsCache</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>Config. do Marketo Sales Insight</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>Valores</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Read, Create, Edit, Delete, View All, Modify All</td> 
  </tr> 
 </tbody> 
</table>

* Apex Class Access: 159 Apex Classes that being with “mkto_si”
* Visualforce Page Access: 64 Visualforce Pages that being with “mkto_si”
* Definições de Configuração Personalizada: mkto_si.Configurações do Marketo e mkto_si.Preferências do usuário

## Adicionar conjunto de permissões do aplicativo Marketo aos usuários {#adding-marketo-app-permission-set-to-users}

1. Faça logon em sua conta do Salesforce.

PICC

1. Clique em **Configuração**.

PICC

1. Em Administrador, clique em para desfazer **Gerenciar usuários**, em seguida **Usuários**.

PICC

1. Em Todos os usuários, selecione o usuário ao qual deseja fornecer acesso e clique em **Atribuições do Conjunto de Permissões**.

PICC

1. Clique em **Editar Atribuições**.

PICC

1. Selecionar **Acesso ao aplicativo Marketo** dos conjuntos de permissões disponíveis, em seguida **Adicionar**. Clique em **Salvar**.

PICC

1. Agora, ao rolar a página Detalhes do usuário, você verá &quot;Acesso ao aplicativo do Marketo&quot; em Atribuições do conjunto de permissões.

PICC

>[!NOTE]
>
>Os usuários que não têm acesso ao Sales Insight verão esta mensagem: &quot;Você não tem privilégios suficientes para acessar esta guia.&quot;

Pronto! Você adicionou com êxito o acesso ao Sales Insight. Repita as mesmas etapas para qualquer outro perfil que você queira adicionar acesso.
