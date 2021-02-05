---
unique-page-id: 4720710
description: Configure o SPF e o DKIM para a entrega por email - Documentos do Marketing - Documentação do produto
title: Configure o SPF e o DKIM para sua entrega de email
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


# Configure o SPF e o DKIM para sua capacidade de entrega de email {#set-up-spf-and-dkim-for-your-email-deliverability}

Um método rápido para melhorar as taxas de delivery de email é incorporar **SPF** (Sender Policy Framework) e **DKIM** (Domain Keys Identified Mail) nas configurações de DNS. Com essa adição às entradas de DNS, você informa aos recipient que autorizou o Marketo a enviar emails em seu nome. Sem essa alteração, seu email tem mais chances de ser marcado como spam desde que o email foi endereçado de seu domínio, mas enviado de um endereço IP com um domínio Marketo.

>[!CAUTION]
>
>Você precisará do administrador da rede para fazer essa alteração no registro DNS.

## Configurar o SPF {#set-up-spf}

**Se você não tiver um registro SPF em seu domínio**

Peça ao administrador da rede para adicionar a seguinte linha às entradas DNS. Substitua [domain] pelo domínio principal do seu site (por exemplo, &quot;empresa.com&quot;) e [corpIP] com o endereço IP do seu servidor de correio eletrônico corporativo (por exemplo, &quot;255.255.255.255&quot;). Se você enviar emails de vários domínios por meio do Marketo, deverá adicioná-los a cada domínio (em uma linha).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se você TEM um registro SPF em seu domínio**

Se você já tiver um registro SPF em sua entrada DNS, adicione o seguinte a ele:

include:mktomail.com

## Configurar o DKIM {#set-up-dkim}

**O que é o DKIM? Por que quero configurar o DKIM?**

O DKIM é um protocolo de autenticação usado por destinatários de e-mail para determinar se uma mensagem de e-mail foi enviada por quem ela diz que foi enviada. O DKIM frequentemente melhora a entrega de emails para a caixa de entrada, já que um receptor pode estar confiante de que a mensagem não é falsa.

**Como funciona o DKIM?**

Depois que você configurar a chave pública no seu registro DNS e ativar o domínio de envio na seção Admin (A), nós ativaremos a assinatura DKIM personalizada para suas mensagens de saída, que incluirá uma assinatura digital criptografada com cada email que enviarmos para você (B). Os receptores poderão descriptografar a assinatura digital pesquisando a &quot;chave pública&quot; no DNS (C) do domínio de envio. Se a chave no e-mail corresponder à chave em seu registro DNS, o servidor de e-mail de recebimento terá maior probabilidade de aceitar o e-mail Marketo enviado em seu nome.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Como configurar o DKIM?**

Consulte [Configurar uma assinatura DKIM personalizada](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [Saiba mais sobre o SPF e como ele funciona](https://www.open-spf.org/Introduction/)
>* [Ferramentas de entrega de email do Marketo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [O meu SPF está configurado corretamente?](https://www.kitterman.com/spf/validate.html)
>* [Eu usei a sintaxe correta?](https://www.open-spf.org/SPF_Record_Syntax/)

