---
description: Verificação de email - Documentação do Marketo - Documentação do produto
title: Verificação de email
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: c5d5fd490fe2800dc7a34d02c73d728e115646a0
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Verificação de email {#email-verification}

As assinaturas do Adobe Marketo Engage exigem que todos os usuários que não sejam somente API, incluindo administradores de Marketo Engage, verifiquem seus endereços de email.

## Por Que Esse Recurso Foi Introduzido {#why-this-feature-was-introduced}

O Marketo Engage continua a implementação da Verificação de email como preparo para migrar clientes para a Plataforma comercial Adobe, incluindo a migração de usuários para IDs Adobe. Esse recurso melhora a segurança das contas de usuário Marketo Engage existentes. Para garantir que um usuário de Marketo Engage esteja associado ao Adobe ID adequado, os usuários existentes de Marketo Engage devem verificar seu endereço de email. Um usuário do Marketo Engage deve ter um endereço de email verificado para ser migrado para um Adobe ID. Se um usuário do Marketo Engage não verificar seu endereço de email, ele não poderá ser migrado para uma Adobe ID e perderá o acesso a uma assinatura do Marketo após a conclusão da migração do usuário para a assinatura.

## Convite de usuário {#user-invite}

Quando um Administrador convida um usuário, ele é automaticamente verificado depois que clica no link de convite.

>[!IMPORTANT]
>
>A exceção ao acima é, _em uma assinatura somente SSO_, Administradores receberão um novo convite de usuário, mas usuários não administradores não receberão. Os usuários que não são administradores ainda devem passar pelo processo de verificação de email para garantir a migração de seus registros. Os usuários podem enviar a si mesmos o link de verificação de email indo até **Admin** > **Minha Conta** > **Configurações da Conta** e clicando em **Reenviar Verificação**.

![](assets/email-verification-1.png)

## Email de verificação {#verification-email}

Os usuários receberão o email abaixo quando a verificação de email for ativada para uma assinatura ou se for acionada por um Administrador/usuário.

Uma sessão de usuário ativa é necessária para o sucesso da Verificação de email. O usuário deve primeiro fazer logon na assinatura do Marketo usando a URL do provedor de identidade (IdP). Depois que uma sessão for estabelecida, eles _e_ clicarão no link **Verificar endereço de email** no email.

![](assets/email-verification-2.png)

>[!TIP]
>
>Para reenviar um email de verificação para um usuário não verificado, basta selecionar seu registro e clicar no botão **[!UICONTROL Verificar Email]**.

## Alteração de um endereço de email {#changing-an-email-address}

Quando o endereço de email de um usuário é alterado, ele não é verificado. Um email será enviado a eles, permitindo que eles verifiquem novamente. Os usuários podem reenviar manualmente esse email clicando em **[!UICONTROL Reenviar Verificação]**.

![](assets/email-verification-3.png)

![](assets/email-verification-4.png)

## Usuários e funções {#users-and-roles}

Em **[!UICONTROL Administrador]** > **[!UICONTROL Usuários e funções]**, a coluna Status do Email mostra o status de verificação de cada usuário.

![](assets/email-verification-5.png)

## IDs de logon de vários usuários {#multiple-user-login-ids}

Somente uma conta de usuário pode ser associada a um único endereço de email. Se houver várias contas de usuário associadas a um único endereço de email, o Marketo Engage exigirá que o conflito seja resolvido e exibirá todos os logons de usuário associados ao endereço de email, bem como três opções de resolução:

* Usar o email atual para a ID de logon de usuário atual
* Usar um novo email para a ID de logon de usuário atual
* Atrasar a decisão até o próximo logon

  ![](assets/email-verification-6.png)

>[!NOTE]
>
>Embora uma conta de usuário precise ser associada a um único endereço, ela pode ser usada em várias assinaturas por meio da Universal ID.
