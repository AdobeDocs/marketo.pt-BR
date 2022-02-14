---
description: Configurações de gerenciamento de logon - Documentação do Marketo - Documentação do produto
title: Configurações de gerenciamento de logon
hide: true
hidefromtoc: true
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
source-git-commit: 984a6dbd19d88db942d9d10bde4880a79feabcc7
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Configurações de gerenciamento de logon {#login-management-settings}

As configurações de Gerenciamento de logon permitem que os administradores definam as preferências de autenticação para usuários de Ações de insight de vendas em um nível global.

>[!NOTE]
>
>Por padrão, a opção Somente Salesforce será selecionada para instâncias de Ações de Insight de Vendas. Recomendamos essa configuração para que os usuários possam [logon automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) do Salesforce.

## Atualizar configurações de gerenciamento de logon {#update-login-management-settings}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Siga estas etapas para atualizar suas preferências de gerenciamento de logon.

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/login-management-settings-1.png)

1. Em Configurações de administração, clique em **Geral**.

   ![](assets/login-management-settings-2.png)

1. Role para baixo até o cartão Gerenciamento de logon e selecione a configuração desejada (neste exemplo, estamos escolhendo Somente Salesforce). Clique em **Salvar** quando concluído.

   ![](assets/login-management-settings-3.png)

## Perguntas frequentes somente sobre o Salesforce {#salesforce-only-faq}

Somente Salesforce significa que os usuários só podem se autenticar para usar as Ações de insight de vendas com o Salesforce. É a seleção padrão para instâncias de Ações de insight de vendas e é recomendada por causa de sua capacidade de permitir que os usuários se autenticem sem precisar gerenciar um nome de usuário e senha.

### Como um novo usuário da minha instância ativa sua conta quando &quot;Somente Salesforce&quot; é selecionado? {#activate-when-salesforce-only-is-selected}

Ao clicar no botão **Introdução** no email de convite, novos usuários serão enviados a uma tela de ativação de conta, onde serão solicitados a conectar a instância do Salesforce para ativar a conta de Ações de insight de vendas.

![](assets/login-management-settings-4.png)

### Com quais métodos de autenticação meus usuários têm permissão para autenticar quando &quot;Somente Salesforce&quot; é selecionado? {#what-authentication-methods}

Ao navegar até nossa tela de logon, os usuários primeiro inserirão seu endereço de email. Em seguida, eles clicarão no botão Logon do Salesforce One Click , onde poderão autenticar usando a conta do Salesforce na qual estão conectados.

>[!NOTE]
>
>Isso se aplica somente aos usuários que navegam diretamente para a tela de logon. Os usuários que acessam Ações do Salesforce serão conectados com [Logon automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Como a autenticação de usuário é tratada para Ações quando um usuário acessa um recurso de Ações do Salesforce e &quot;Somente Salesforce&quot; é selecionado? {#how-is-user-authentication-handled}

Quando um usuário clica em uma das ações (Chamada, Email, Campanha, Tarefas, Lista de campanhas etc..), usamos a autenticação SFDC para fazer logon automaticamente em sua conta de Ações de insight de vendas. Chamamos essa autenticação [Logon automático](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Perguntas frequentes sobre todos os métodos de logon {#all-login-methods-faq}

### Como um novo usuário da minha instância ativa sua conta quando a opção &quot;Todos os métodos de logon&quot; é selecionada? {#activate-when-all-login-methods-is-selected}

Quando um novo usuário é convidado para uma instância, ele receberá um email de ativação da conta. Eles clicarão no botão &quot;Introdução&quot;, que os levará a uma página que solicita a criação e confirmação de uma senha. Depois que isso for criado, sua conta será ativada e elas serão executadas por meio do fluxo de trabalho de integração.

![](assets/login-management-settings-6.png)

### Com que usuários da minha instância podem fazer logon quando &quot;Todos os métodos de logon&quot; é selecionado? {#what-are-users-allowed-to-log-in-with-all-login}

Ao usar nossa página de logon, os usuários primeiro inserirão seu endereço de email. Em seguida, serão enviadas para uma página que oferece todas as opções de logon (nome de usuário/senha, SFDC, Gmail, SSO) para autenticação.
