---
unique-page-id: 4720710
description: Configure o SPF e o DKIM para a entrega por email - Documentos do Marketing - Documentação do produto
title: Configure o SPF e o DKIM para sua entrega de email
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Configure o SPF e o DKIM para sua entrega de email {#set-up-spf-and-dkim-for-your-email-deliverability}

Um método rápido para melhorar as taxas de delivery de email é incorporar o **SPF** (Sender Policy Framework) e o **DKIM** (Domain Keys Identified Mail) às configurações de DNS. Com essa adição às entradas de DNS, você informa aos recipient que autorizou o Marketo a enviar emails em seu nome. Sem essa alteração, seu email tem mais chances de ser marcado como spam desde que o email foi endereçado de seu domínio, mas enviado de um endereço IP com um domínio Marketo.

>[!CAUTION]
>
>Você precisará do administrador da rede para fazer essa alteração no registro DNS.

## Configurar SPF {#set-up-spf}

**Se você não tiver um registro SPF em seu domínio**

Peça ao administrador da rede para adicionar a seguinte linha às entradas DNS. Substitua o [domínio] pelo domínio principal do seu site (por exemplo, &quot;empresa.com&quot;) e [corpIP] com o endereço IP do seu servidor de e-mail corporativo (por exemplo, &quot;255.255.255.255&quot;). Se você enviar emails de vários domínios por meio do Marketo, deverá adicioná-los a cada domínio (em uma linha).
[domínio] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all\
Se você TEM um registro SPF em seu domínio

Se você já tiver um registro SPF em sua entrada DNS, adicione o seguinte a ele:

include:mktomail.com

## Configurar o DKIM {#set-up-dkim}

### O que é o DKIM? Por que quero configurar o DKIM? {#what-is-dkim-why-do-i-want-to-set-up-dkim}

O DKIM é um protocolo de autenticação usado por destinatários de e-mail para determinar se uma mensagem de e-mail foi enviada por quem ela diz que foi enviada. O DKIM frequentemente melhora a entrega de emails para a caixa de entrada, já que um receptor pode estar confiante de que a mensagem não é falsa.

Como funciona o DKIM?

Depois que você configurar a chave pública no seu registro DNS e ativar o domínio de envio na seção Admin (A), nós ativaremos a assinatura DKIM personalizada para suas mensagens de saída, que incluirá uma assinatura digital criptografada com cada email que enviarmos para você (B). Os receptores poderão descriptografar a assinatura digital pesquisando a &quot;chave pública&quot; no DNS (C) do domínio de envio. Se a chave no e-mail corresponder à chave em seu registro DNS, o servidor de e-mail de recebimento terá maior probabilidade de aceitar o e-mail Marketo enviado em seu nome.

![](assets/image2015-1-12-13-3a56-3a55.png)

Como configurar o DKIM?

Consulte [Configurar uma assinatura](set-up-a-custom-dkim-signature.md)DKIM personalizada.

>[!MORELIKETHIS]
>
>* [Saiba mais sobre o SPF e como ele funciona](http://www.open-spf.org/Introduction/)
>* [Ferramentas de entrega de email do Marketo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [O meu SPF está configurado corretamente?](http://www.kitterman.com/spf/validate.html)
>* [Eu usei a sintaxe correta?](http://www.open-spf.org/SPF_Record_Syntax/)

>



