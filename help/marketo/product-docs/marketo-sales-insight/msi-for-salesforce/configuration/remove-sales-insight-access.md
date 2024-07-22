---
description: Remover o acesso ao Sales Insight - Documentação do Marketo - Documentação do produto
title: Remover acesso ao Sales Insight
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 7%

---

# Remover acesso ao Sales Insight {#remove-sales-insight-access}

Use as etapas a seguir para remover o acesso aos recursos do Sales Insight no Salesforce. Aplicável ao Salesforce Classic e Lightning.

## Visão geral {#overview}

A permissão para os objetos mencionados abaixo, classes apex e páginas de força visual é necessária para acessar todos os recursos do Sales Insight. Remover esses itens removerá o acesso ao Sales Insight.

**Configurações do objeto**

<table> 
 <tbody> 
 <tr> 
   <td>BestBetsCache</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>Detalhes de melhores opções</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>Exibições de Melhores Opções</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>EmailActivityCache</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>GetMethodArgus</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>GroupedWebActivityCache</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>InterestingMomentsCache</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>Config. do Marketo Sales Insight</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>ScoringCache</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>Valores</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
  <tr> 
   <td>WebActivityCache</td> 
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td> 
  </tr> 
 </tbody> 
</table>

* Acesso à classe Apex: 159 classes Apex que começam com &quot;mkto_si&quot;
* Acesso à página do Visualforce: 64 páginas do Visualforce que começam com &quot;mkto_si&quot;
* Definições de configuração personalizada: mkto_si.Configurações do Marketo &amp; mkto_si.Preferências do usuário

## Remover o acesso ao Sales Insight {#removing-access-to-sales-insight}

1. Faça logon em sua conta do Salesforce.

1. Clique em **Instalação**.

   ![](assets/remove-sales-insight-access-1.png)

1. Em Administrador, clique em **Gerenciar usuários** e depois em **Perfis**.

1. Clique no perfil que você deseja atualizar e **Editar**.

1. Role para baixo até &quot;Configurações personalizadas da guia&quot; em Configurações da guia.

1. Selecione a opção &quot;Guia oculta&quot; no menu suspenso para Configuração do Marketo Sales Insight e Caixa de saída do MSI Marketo Sales.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Role para baixo até &quot;Permissões de objeto personalizado&quot;.

1. Remova o acesso &quot;Ler, Criar, Editar, Excluir&quot; dos seguintes objetos:

   * BestBetsCache
   * Detalhes de melhores opções
   * Exibições de Melhores Opções
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Config. do Marketo Sales Insight
   * ScoringCache
   * Valores
   * WebActivityCache

1. Role para baixo até a seção &quot;Acesso de classe Apex ativado&quot;. Clique em **Editar**.

1. Na seção &quot;Classes apex ativadas&quot;, selecione todas as classes que comecem com &quot;mkto_si&quot;. Isso deve somar até 159 classes.

1. Clique em **Remover** e depois em **Salvar**.

   ![](assets/remove-sales-insight-access-4.png)

1. Role para baixo até a seção &quot;Acesso ativado à página do Visualforce&quot;. Clique em **Editar**.

1. Na seção &quot;Páginas habilitadas do Visualforce&quot;, selecione todas as páginas que comecem com &quot;mkto_si&quot;. Isso deve somar até 64 páginas.

1. Clique em **Remover** e depois em **Salvar**.

   ![](assets/remove-sales-insight-access-5.png)

1. Role para baixo até a seção &quot;Acesso ativado às definições de configuração personalizada&quot;. Clique em **Editar**.

1. Selecione &quot;Configurações do Marketo Sales Insight.mkto_si.Marketo&quot; e &quot;Preferências do Marketo Sales Insight.mkto_si.User&quot;.

1. Clique em **Remover** e depois em **Salvar**.

   ![](assets/remove-sales-insight-access-6.png)

Pronto! Você removeu com êxito o acesso ao Sales Insight. Repita as mesmas etapas para qualquer outro perfil cujo acesso você queira remover.
