---
unique-page-id: 4720710
description: Configurar o SPF e o DKIM para sua capacidade de entrega de email - Documentação do Marketo - Documentação do produto
title: Configurar o SPF e o DKIM para a capacidade de entrega de email
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 4%

---

# Configurar o SPF e o DKIM para a capacidade de entrega de email {#set-up-spf-and-dkim-for-your-email-deliverability}

Um método rápido para melhorar as taxas de entrega de email é incorporar o **SPF** (Estrutura de Política de Remetente) e o **DKIM** (Domain Keys Identified Mail) às configurações de DNS. Com essa adição às entradas de DNS, você informa aos destinatários que autorizou o Marketo a enviar emails em seu nome. Sem essa alteração, seu email tem uma chance maior de ser marcado como spam, pois foi endereçado do seu domínio, mas enviado de um endereço IP com um domínio Marketo.

>[!CAUTION]
>
>Você precisará que o administrador de rede faça essa alteração no registro DNS.

## Configurar SPF {#set-up-spf}

**Se você NÃO tiver um registro SPF em seu domínio**

Peça ao administrador de rede para adicionar a seguinte linha às suas entradas de DNS. Substitua [domínio] pelo domínio principal do seu site (por exemplo, &quot;company.com&quot;) e [corpIP] com o endereço IP do servidor de email corporativo (por exemplo, 255.255.255.255). Se você enviar emails de vários domínios por meio do Marketo, adicione isso a cada domínio (em uma linha).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se você TIVER UM registro SPF em seu domínio**

Se você já tiver um registro SPF na sua entrada DNS, adicione o seguinte a ele:

include:mktomail.com

## Configurar o DKIM {#set-up-dkim}

**O que é o DKIM? Por que quero configurar o DKIM?**

O DKIM é um protocolo de autenticação usado pelos destinatários de email para determinar se uma mensagem de email foi enviada por quem diz que foi enviada. O DKIM geralmente melhora a capacidade de entrega de emails para a caixa de entrada, pois um destinatário pode ter certeza de que a mensagem não é uma falsificação.

**Como funciona o DKIM?**

Depois que você configurar a chave pública em seu registro DNS e ativar o domínio de envio na seção Admin (A), ativaremos a assinatura personalizada do DKIM para suas mensagens de saída, que incluirão uma assinatura digital criptografada com cada email que enviamos para você (B). Os receptores poderão descriptografar a assinatura digital procurando a &quot;chave pública&quot; no DNS (C) do domínio de envio. Se a chave no email corresponder à chave no seu registro DNS, o servidor de email de recebimento terá mais probabilidade de aceitar o Marketo de email enviado em seu nome.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Como configurar o DKIM?**

Consulte [Configurar uma Assinatura DKIM Personalizada](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Saiba mais sobre o SPF e como ele funciona`: http://www.open-spf.org/Introduction/`
>* Meu SPF está configurado corretamente?: `https://www.kitterman.com/spf/validate.html`
>* Eu usei a sintaxe correta?: `http://www.open-spf.org/SPF_Record_Syntax/`
