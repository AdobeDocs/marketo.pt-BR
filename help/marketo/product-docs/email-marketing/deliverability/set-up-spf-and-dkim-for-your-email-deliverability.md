---
unique-page-id: 4720710
description: Configurar o SPF e o DKIM para sua capacidade de entrega de email - Documentação do Marketo - Documentação do produto
title: Configurar o SPF e o DKIM para a capacidade de entrega de emails
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Configurar o SPF e o DKIM para a capacidade de entrega de emails {#set-up-spf-and-dkim-for-your-email-deliverability}

Um método rápido para melhorar as taxas de delivery de email é incorporar **SPF** (Estrutura de Política do Remetente) e **DKIM** (Domain Keys Identified Mail) nas configurações de DNS. Com essa adição às entradas de DNS, você informa aos destinatários que autorizou o Marketo a enviar emails em seu nome. Sem essa alteração, seu email tem uma chance maior de ser marcado como spam, pois foi endereçado do seu domínio, mas enviado de um endereço IP com um domínio Marketo.

>[!CAUTION]
>
>Você precisará que o administrador de rede faça essa alteração no registro DNS.

## Configurar SPF {#set-up-spf}

**Se você NÃO tiver um registro SPF em seu domínio**

Peça ao administrador de rede para adicionar a seguinte linha às suas entradas de DNS. Substituir [domínio] com o domínio principal do seu site (por exemplo, &quot;company.com&quot;) e [corpIP] com o endereço IP do seu servidor de email corporativo (por exemplo, &quot;255.255.255.255&quot;). Se você enviar emails de vários domínios por meio do Marketo, adicione isso a cada domínio (em uma linha).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se você TIVER UM REGISTRO SPF em seu domínio**

Se você já tiver um registro SPF na sua entrada DNS, adicione o seguinte a ele:

incluir:mktomail.com

## Configurar DKIM {#set-up-dkim}

**O que é DKIM? Por que eu quero configurar o DKIM?**

O DKIM é um protocolo de autenticação usado pelos destinatários de email para determinar se uma mensagem de email foi enviada por quem diz que foi enviada. O DKIM geralmente melhora a capacidade de entrega de emails para a caixa de entrada, pois um destinatário pode ter certeza de que a mensagem não é uma falsificação.

**Como funciona o DKIM?**

Depois que você configurar a chave pública em seu registro DNS e ativar o domínio de envio na seção Admin (A), ativaremos a assinatura DKIM personalizada para suas mensagens de saída, que incluirão uma assinatura digital criptografada com cada email que enviamos para você (B). Os receptores poderão descriptografar a assinatura digital procurando a &quot;chave pública&quot; no DNS (C) do domínio de envio. Se a chave no email corresponder à chave no seu registro DNS, o servidor de email de recebimento terá mais probabilidade de aceitar o Marketo de email enviado em seu nome.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Como configurar o DKIM?**

Consulte [Configurar uma assinatura DKIM personalizada](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Saiba mais sobre o SPF e como ele funciona](http://www.open-spf.org/Introduction/){target="_blank"}
>* [Meu SPF está configurado corretamente?](https://www.kitterman.com/spf/validate.html){target="_blank"}
>* [Eu usei a sintaxe correta?](http://www.open-spf.org/SPF_Record_Syntax/){target="_blank"}
