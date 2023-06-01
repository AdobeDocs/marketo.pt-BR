---
description: Verificação de email - Documentação do Marketo - Documentação do produto
title: Verificação de email
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: e104a8bd41d61451202ba089512dc688680292ce
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Verificação de email {#email-verification}

As assinaturas do Adobe Marketo Engage exigem que todos os usuários que não sejam somente API, incluindo administradores de Marketo Engage, verifiquem seus endereços de email. Os usuários de Logon único (SSO) que não recebem uma função de Administrador ou que recebem uma função com a permissão &#39;Ignorar SSO&#39; terão seu email verificado automaticamente quando sua assinatura for habilitada com o recurso de Verificação de email.

## Convite de usuário {#user-invite}

Quando um Administrador convida um usuário, ele é automaticamente verificado depois que clica no link de convite. Os usuários do SSO, sem a função de Administrador atribuída, são automaticamente verificados.

## Email de verificação {#verification-email}

Os usuários convidados receberão o seguinte email:

![](assets/email-verification-1.png)

>[!NOTE]
>
>Para reenviar um email de verificação a um usuário não verificado, basta selecionar o registro e clicar no link **Verificar email** botão.

## Alteração de um endereço de email {#changing-an-email-address}

Quando o endereço de email de um usuário é alterado, ele não é verificado. Um email será enviado a eles, permitindo que eles verifiquem novamente. Os usuários podem reenviar manualmente esse email clicando em **Reenviar verificação**.

![](assets/email-verification-2.png)

![](assets/email-verification-3.png)

## Usuários e funções {#users-and-roles}

Entrada **Admin** > **Usuários e funções**, a coluna Status de email mostra o status de verificação de cada usuário.

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
