---
description: Verificação de email - Documentação do Marketo - Documentação do produto
title: Verificação de email
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
feature: Users and Roles
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '417'
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
>A exceção ao acima é que, em uma assinatura somente SSO, os administradores receberão um novo convite do usuário, mas os não administradores não receberão. Os não administradores devem passar pelo processo de verificação de email para garantir a migração de seus registros de usuário. Um Administrador pode enviar o link de verificação de email clicando no link **Reenviar verificação de email** ao lado do nome de usuário.

## Email de verificação {#verification-email}

Os usuários receberão o seguinte email quando a verificação de email for ativada para uma assinatura ou se for acionada por um Administrador/usuário:

![](assets/email-verification-1.png)

>[!NOTE]
>
>Para reenviar um email de verificação a um usuário não verificado, basta selecionar o registro e clicar no link **[!UICONTROL Verificar email]** botão.

## Alteração de um endereço de email {#changing-an-email-address}

Quando o endereço de email de um usuário é alterado, ele não é verificado. Um email será enviado a eles, permitindo que eles verifiquem novamente. Os usuários podem reenviar manualmente esse email clicando em **[!UICONTROL Reenviar verificação]**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## Usuários e funções {#users-and-roles}

Entrada **[!UICONTROL Admin]** > **[!UICONTROL Usuários e funções]**, a coluna Status de email mostra o status de verificação de cada usuário.

![](assets/email-verification-4.png)

## IDs de logon de vários usuários {#multiple-user-login-ids}

Somente uma conta de usuário pode ser associada a um único endereço de email. Se houver várias contas de usuário associadas a um único endereço de email, o Marketo Engage exigirá que o conflito seja resolvido e exibirá todos os logons de usuário associados ao endereço de email, bem como três opções de resolução:

* Usar o email atual para a ID de logon de usuário atual
* Usar um novo email para a ID de logon de usuário atual
* Atrasar a decisão até o próximo logon

  ![](assets/email-verification-5.png)

>[!NOTE]
>
>Embora uma conta de usuário precise ser associada a um único endereço, ela pode ser usada em várias assinaturas por meio da Universal ID.
