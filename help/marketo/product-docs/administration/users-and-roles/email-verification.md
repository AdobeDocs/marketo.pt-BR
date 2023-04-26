---
description: Verificação de email - Documentação da Marketo - Documentação do produto
title: Verificação de email
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: c45b3ab94b806b53768891613f15b8e9b694a440
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# Verificação de email {#email-verification}

As assinaturas do Adobe Marketo Engage exigem que todos os usuários que não usam API, incluindo Administradores do Marketo Engage, verifiquem seu endereço de email. Usuários de Logon Único (SSO) que não recebem uma função de Administrador ou que recebem uma função com a permissão &#39;Ignorar SSO&#39; terão seu email verificado automaticamente quando sua assinatura for habilitada com o recurso Verificação de Email.

**Convite de usuário**

Quando um Administrador convida um usuário, ele é verificado automaticamente assim que ele clicar no link do convite. Os usuários do SSO, que não têm a função de Administrador, são verificados automaticamente.

**Alterar um endereço de email**

Quando o endereço de email de um usuário é alterado, ele se torna não verificado. Um email será enviado para eles permitindo a verificação novamente. Os usuários podem reenviar manualmente esse email clicando em **Reenviar verificação**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

**Usuários e funções**

Em Admin > Usuários e funções, a coluna Status de email mostra o status de verificação de cada usuário.

![](assets/email-verification-3.png)

Para reenviar um email de verificação para um usuário não verificado, basta selecionar o registro e clicar no botão **Verificar Email** botão.
