---
description: Configurações de gerenciamento de logon - Documentação do Marketo - Documentação do produto
title: Configurações de gerenciamento de logon
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Configurações de gerenciamento de logon {#login-management-settings}

As configurações do Gerenciamento de logon permitem que os administradores definam as preferências de autenticação para usuários de Ações do Sales Insight em nível global.

>[!NOTE]
>
>Por padrão, a opção Somente Salesforce será selecionada para instâncias de Ações de insight de vendas. Recomendamos essa configuração para que os usuários possam [fazer logon automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) do Salesforce.

## Atualizar Configurações de Gerenciamento de Logon {#update-login-management-settings}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Para atualizar suas preferências de gerenciamento de logon, siga estas etapas.

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/login-management-settings-1.png)

1. Em Configurações de administração, clique em **Geral**.

   ![](assets/login-management-settings-2.png)

1. Role para baixo até o cartão Gerenciamento de logon e selecione a configuração desejada (neste exemplo, estamos escolhendo Somente Salesforce). Clique em **Salvar** quando terminar.

   ![](assets/login-management-settings-3.png)

## Perguntas frequentes somente sobre o Salesforce {#salesforce-only-faq}

Salesforce Only significa que os usuários só podem autenticar para usar as Ações de insight de vendas com o Salesforce. É a seleção padrão para instâncias de Ações do Sales Insight, e é recomendada devido à sua capacidade de permitir que os usuários se autentiquem sem problemas sem precisar gerenciar um nome de usuário e senha.

### Como um novo usuário na minha instância ativa a conta dele quando &quot;Salesforce Only&quot; está selecionado? {#activate-when-salesforce-only-is-selected}

Ao clicar no botão **Introdução** no email de convite, novos usuários serão enviados para uma tela de ativação de conta, onde serão solicitados a conectar sua instância do Salesforce para ativar a conta de Ações de Insight de Vendas.

![](assets/login-management-settings-4.png)

### Com quais métodos de autenticação meus usuários podem realizar a autenticação quando a opção &quot;Somente Salesforce&quot; está selecionada? {#what-authentication-methods}

Ao navegar para nossa tela de logon, os usuários digitarão primeiro seu endereço de email. Em seguida, eles clicarão no botão Salesforce One Click Login, onde poderão se autenticar usando a conta do Salesforce à qual estão conectados.

>[!NOTE]
>
>Isso se refere apenas aos usuários que navegam diretamente para a tela de logon. Os usuários que estão acessando Ações do Salesforce serão conectados com [Logon automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Como a autenticação de usuário é tratada para Ações quando um usuário acessa um recurso Ações do Salesforce e &quot;Somente Salesforce&quot; é selecionado? {#how-is-user-authentication-handled}

Quando um usuário clica em uma das ações (Chamada, Email, Campanha, Tarefas, Lista de campanhas etc.), usamos a autenticação SFDC para conectá-lo automaticamente à conta de Ações de insights de vendas. Chamamos esta autenticação de [Logon automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Perguntas frequentes sobre todos os métodos de logon {#all-login-methods-faq}

### Como um novo usuário na minha instância ativa a conta dele quando &quot;Todos os métodos de logon&quot; é selecionado? {#activate-when-all-login-methods-is-selected}

Quando um novo usuário é convidado para uma instância, ele recebe um email de ativação de conta. Eles clicarão no botão que diz &quot;Introdução&quot;, que os levará a uma página que solicita que criem e confirmem uma senha. Depois de criado, a conta dele será ativada e eles serão transferidos para o fluxo de trabalho de integração.

![](assets/login-management-settings-6.png)

### Com o que os usuários da minha instância podem fazer logon quando a opção &quot;Todos os métodos de logon&quot; está selecionada? {#what-are-users-allowed-to-log-in-with-all-login}

Ao usar nossa página de logon, os usuários inserirão primeiro seu endereço de email. Em seguida, eles serão enviados para uma página que fornece todas as opções de logon (nome de usuário/senha, SFDC, Gmail, SSO) para autenticação.
