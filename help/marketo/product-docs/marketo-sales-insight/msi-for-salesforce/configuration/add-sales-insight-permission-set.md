---
description: Adicionar conjunto de permissões de insight de vendas - Documentos da Marketo - Documentação do produto
title: Adicionar Conjunto de Permissões de Insight de Vendas
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
source-git-commit: d9876d73561d63dea4e46b0dfd191082f262baf6
workflow-type: tm+mt
source-wordcount: '379'
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

A permissão &quot;Aplicativo Marketo&quot; é parte do pacote Sales Insight Salesforce . Ele inclui acesso aos objetos mencionados abaixo, às classes de ápice e às páginas de força visual. Eles são necessários para acessar todos os recursos do Sales Insight.

**Configurações do objeto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
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
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
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
   <td>Ler, Criar, Editar, Excluir, Exibir todos, Modificar tudo</td> 
  </tr> 
 </tbody> 
</table>

* Acesso à classe do anexo: 159 Classes Apex que estão sendo com &quot;mkto_si&quot;
* Forçar acesso à página: 64 Páginas de força de visita que estão sendo usadas com &quot;mkto_si&quot;
* Definições de Configuração Personalizada: mkto_si.Configurações do Marketo e mkto_si.Preferências do usuário

## Adicionar conjunto de permissões do aplicativo Marketo aos usuários {#adding-marketo-app-permission-set-to-users}

1. Faça logon em sua conta do Salesforce.

1. Clique em **Configuração**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Em Administrador, clique em para desfazer **Gerenciar usuários**, em seguida **Usuários**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Em Todos os usuários, selecione o usuário ao qual deseja fornecer acesso e clique em **Atribuições do Conjunto de Permissões**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Clique em **Editar Atribuições**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Selecionar **Acesso ao aplicativo Marketo** dos conjuntos de permissões disponíveis, em seguida **Adicionar**. Clique em **Salvar**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Agora, ao rolar a página Detalhes do usuário, você verá &quot;Acesso ao aplicativo do Marketo&quot; em Atribuições do conjunto de permissões.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Os usuários que não têm acesso ao Sales Insight verão esta mensagem: &quot;Você não tem privilégios suficientes para acessar esta guia.&quot;

Pronto! Você adicionou com êxito o acesso ao Sales Insight. Repita as mesmas etapas para qualquer outro perfil que você queira adicionar acesso.
