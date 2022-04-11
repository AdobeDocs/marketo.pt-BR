---
description: Remover o acesso ao insight de vendas - Documentos da Marketo - Documentação do produto
title: Remover Acesso ao Insight de Vendas
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
source-git-commit: cccea2e9b7e1d0017e9be071ec85051f71e737bd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Remover Acesso ao Insight de Vendas {#remove-sales-insight-access}

Use as etapas a seguir para remover o acesso aos recursos do Sales Insight no Salesforce. Aplicável ao Salesforce Classic e Lightning.

## Visão geral {#overview}

É necessária permissão para acessar todos os recursos do Sales Insight. A remoção desses eventos removerá o acesso ao Sales Insight.

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

* Acesso à classe do anexo: 159 Classes de Apex que começam com &quot;mkto_si&quot;
* Forçar acesso à página: 64 Páginas de força de visita que começam com &quot;mkto_si&quot;
* Definições de Configuração Personalizada: mkto_si.Configurações do Marketo e mkto_si.Preferências do usuário

## Removendo o acesso ao insight de vendas {#removing-access-to-sales-insight}

1. Faça logon em sua conta do Salesforce.

1. Clique em **Configuração**.

   ![](assets/remove-sales-insight-access-1.png)

1. Em Administrador, clique em **Gerenciar usuários**, em seguida **Perfis**.

1. Clique no perfil que deseja atualizar e, em seguida, **Editar**.

1. Role para baixo até &quot;Configurações personalizadas de guia&quot;, em Configurações da guia.

1. Selecione a opção &quot;Guia oculta&quot; no menu suspenso da Configuração do Marketo Sales Insight e Caixa de saída de vendas do MSI Marketo.

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Role para baixo até &quot;Permissões de objeto personalizado&quot;.

1. Remova o acesso &quot;Ler, Criar, Editar, Excluir&quot; dos seguintes objetos:

   * MelhorCache
   * Detalhes de melhores opções
   * Melhores visualizações
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InteressanteMomentsCache
   * Config. do Marketo Sales Insight
   * ScoringCache
   * Valores
   * WebActivityCache

1. Role para baixo até a seção &quot;Acesso ativado à classe do Apex&quot;. Clique em **Editar**.

1. Na seção &quot;Classes de Apex Ativadas&quot;, selecione todas as classes que começam com &quot;mkto_si&quot;. Isso deve somar até 159 classes.

1. Clique em **Remover**, em seguida **Salvar**.

   ![](assets/remove-sales-insight-access-4.png)

1. Role para baixo até a seção &quot;Ativado acesso à página por força de visita&quot;. Clique em **Editar**.

1. Na seção &quot;Páginas de força de visita ativadas&quot;, selecione todas as páginas que começam com &quot;mkto_si&quot;. Isso deve adicionar até 64 páginas.

1. Clique em **Remover**, em seguida **Salvar**.

   ![](assets/remove-sales-insight-access-5.png)

1. Role para baixo até a seção &quot;Acesso ativado às definições de configuração personalizada&quot;. Clique em **Editar**.

1. Selecione &quot;Marketo Sales Insight.mkto_si.Marketo Settings&quot; e &quot;Marketo Sales Insight.mkto_si.User Preferences&quot;.

1. Clique em **Remover**, em seguida **Salvar**.

   ![](assets/remove-sales-insight-access-6.png)

Pronto! Você removeu com êxito o acesso ao Sales Insight. Repita as mesmas etapas para qualquer outro perfil que você queira remover o acesso.
