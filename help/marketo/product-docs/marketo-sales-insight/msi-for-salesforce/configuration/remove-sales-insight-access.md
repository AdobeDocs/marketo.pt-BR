---
description: Remover o acesso ao Sales Insight - Documentação do Marketo - Documentação do produto
title: Remover acesso ao Insight de vendas
exl-id: 3cda112a-524e-469b-a222-c0192b2f5301
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 8%

---

# Remover acesso de [!DNL Sales Insight] {#remove-sales-insight-access}

Use as etapas a seguir para remover o acesso aos recursos do [!DNL Sales Insight] no [!DNL Salesforce]. Aplicável ao [!DNL Salesforce] Classic e Lightning.

## Visão geral {#overview}

A permissão para os objetos mencionados abaixo, classes apex e páginas de força visual é necessária para acessar todos os recursos [!DNL Sales Insight]. A remoção destes itens removerá o acesso a [!DNL Sales Insight].

**Configurações do objeto**

<table>
 <tbody>
 <tr>
   <td>BestBetsCache</td>
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td>
  </tr>
  <tr>
   <td>[!DNL Best Bets] Exibir detalhes</td>
   <td>Ler, Criar, Editar, Deletar, Exibir Tudo, Modificar Tudo</td>
  </tr>
  <tr>
   <td>[!DNL Best Bets] Exibições</td>
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
   <td>[!DNL Marketo Sales Insight] Configuração</td>
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

## Removendo Acesso a [!DNL Sales Insight] {#removing-access-to-sales-insight}

1. Faça logon em sua conta do [!DNL Salesforce].

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/remove-sales-insight-access-1.png)

1. Em [!UICONTROL Administrador], clique em **[!UICONTROL Gerenciar Usuários]** e depois em **[!UICONTROL Perfis]**.

1. Clique no perfil que você deseja atualizar e **[!UICONTROL Editar]**.

1. Role para baixo até &quot;[!UICONTROL Configurações de Guia Personalizadas]&quot; em [!UICONTROL Configurações de Guia].

1. Selecione a opção &quot;[!UICONTROL Tab Hidden]&quot; no menu suspenso para Configuração [!DNL Marketo Sales Insight] e Caixa de Saída MSI [!DNL Marketo Sales].

   ![](assets/remove-sales-insight-access-2.png)

   ![](assets/remove-sales-insight-access-3.png)

1. Role para baixo até &quot;[!UICONTROL Permissões de objetos personalizados].&quot;

1. Remova o acesso &quot;Ler, Criar, Editar, Excluir&quot; dos seguintes objetos:

   * BestBetsCache
   * [!DNL Best Bets] Exibir detalhes
   * [!DNL Best Bets] Visualizações
   * EmailActivityCache
   * GetMethodArgus
   * GroupedWebActivityCache
   * InterestingMomentsCache
   * Configuração de [!DNL Marketo Sales Insight]
   * ScoringCache
   * Valores
   * WebActivityCache

1. Role para baixo até a seção &quot;[!UICONTROL Acesso de classe apex habilitado]&quot;. Clique em **[!UICONTROL Editar]**.

1. Na seção &quot;[!UICONTROL Classes Apex Habilitadas]&quot;, selecione todas as classes que comecem com &quot;mkto_si&quot;. Isso deve somar até 159 classes.

1. Clique em **[!UICONTROL Remover]** e depois em **[!UICONTROL Salvar]**.

   ![](assets/remove-sales-insight-access-4.png)

1. Role para baixo até a seção &quot;[!UICONTROL Acesso à página do Visualforce habilitado]&quot;. Clique em **[!UICONTROL Editar]**.

1. Na seção &quot;[!UICONTROL Páginas do Visualforce habilitadas]&quot;, selecione todas as páginas que comecem com &quot;mkto_si&quot;. Isso deve somar até 64 páginas.

1. Clique em **[!UICONTROL Remover]** e depois em **[!UICONTROL Salvar]**.

   ![](assets/remove-sales-insight-access-5.png)

1. Role para baixo até a seção &quot;[!UICONTROL Acesso Habilitado a Definições de Configuração Personalizadas]&quot;. Clique em **[!UICONTROL Editar]**.

1. Selecione &quot;Configurações do Marketo Sales Insight.mkto_si.Marketo&quot; e &quot;Preferências do Marketo Sales Insight.mkto_si.User.&quot;

1. Clique em **[!UICONTROL Remover]** e depois em **[!UICONTROL Salvar]**.

   ![](assets/remove-sales-insight-access-6.png)

Pronto! Você removeu com êxito o acesso de [!DNL Sales Insight]. Repita as mesmas etapas para qualquer outro perfil cujo acesso você queira remover.
