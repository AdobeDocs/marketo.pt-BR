---
description: Adicionar Conjunto De Permissões Do Sales Insight - Documentação Do Marketo - Documentação Do Produto
title: Adicionar Conjunto de Permissões do Sales Insight
exl-id: b93ddf2e-0f7b-41e0-ba88-7363f5e34970
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 4%

---

# Adicionar conjunto de permissões [!DNL Sales Insight] {#add-sales-insight-permission-set}

Use as etapas a seguir para adicionar acesso aos recursos do [!DNL Sales Insight] no [!DNL Salesforce]. Aplicável ao [!DNL Salesforce] Classic e Lighining

>[!PREREQUISITES]
>
>[Atualize seu [!DNL Sales Insight] [!DNL Salesforce] pacote](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} para a versão 1.8000 ou superior para usar este recurso.

>[!IMPORTANT]
>
>Se você já tiver concedido acesso de [!DNL Sales Insight] a todos os perfis e/ou implementado [!DNL Sales Insight] para todos os seus usuários, deverá [remover o acesso de nível de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} para usar este conjunto de permissões.

## Visão geral {#overview}

A permissão &quot;Aplicativo Marketo&quot; faz parte do pacote [!DNL Sales Insight] [!DNL Salesforce]. Inclui acesso aos objetos mencionados abaixo, classes apex e páginas de força visual. Eles são necessários para acessar todos os recursos do [!DNL Sales Insight].

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
   <td>Configuração do Marketo [!DNL Sales Insight]</td> 
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

## Adicionar o conjunto de permissões do aplicativo Marketo aos usuários {#adding-marketo-app-permission-set-to-users}

1. Faça logon em sua conta do [!DNL Salesforce].

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/add-sales-insight-permission-set-1.png)

1. Em Administrador, clique para desencaminhar **[!UICONTROL Gerenciar Usuários]** e depois **[!UICONTROL Usuários]**.

   ![](assets/add-sales-insight-permission-set-2.png)

1. Em Todos os usuários, selecione o usuário ao qual deseja fornecer acesso e clique em **[!UICONTROL Atribuições de conjunto de permissões]**.

   ![](assets/add-sales-insight-permission-set-3.png)

1. Clique em **[!UICONTROL Editar atribuições]**.

   ![](assets/add-sales-insight-permission-set-4.png)

1. Selecione **[!UICONTROL Acesso ao Aplicativo Marketo]** nos conjuntos de permissões disponíveis e **[!UICONTROL Adicionar]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/add-sales-insight-permission-set-5.png)

1. Agora, ao rolar para baixo na página Detalhes do usuário, você verá &quot;Acesso ao aplicativo Marketo&quot; em Atribuições de conjunto de permissões.

   ![](assets/add-sales-insight-permission-set-6.png)

>[!NOTE]
>
>Os usuários que não têm acesso a [!DNL Sales Insight] verão esta mensagem: &quot;Você não tem privilégios suficientes para acessar esta guia.&quot;

Pronto! Você adicionou com êxito o acesso de [!DNL Sales Insight]. Repita as mesmas etapas para qualquer outro perfil ao qual deseje adicionar acesso.
