---
unique-page-id: 4720710
description: Configurar o SPF e o DKIM para entrega de e-mail - Documentos do Marketo - Documentação do produto
title: Configurar SPF e DKIM para sua capacidade de delivery de email
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: de32becbfe74c2a88c53de8af8be4ee022782114
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Configurar SPF e DKIM para sua capacidade de delivery de email {#set-up-spf-and-dkim-for-your-email-deliverability}

Um método rápido para melhorar as taxas de delivery de email é incorporar **SPF** (Estrutura de Política do Remetente) e **DKIM** (Chaves de domínio identificadas) nas configurações de DNS. Com essa adição às entradas de DNS, você informa aos recipients que autorizou o Marketo a enviar emails em seu nome. Sem essa alteração, seu email tem maior chance de ser marcado como spam desde que o email foi endereçado de seu domínio, mas enviado de um endereço IP com um domínio Marketo.

>[!CAUTION]
>
>Você precisará do administrador da rede para fazer essa alteração no registro DNS.

## Configurar SPF {#set-up-spf}

**Se você NÃO tiver um registro SPF em seu domínio**

Peça ao administrador de rede para adicionar a seguinte linha às suas entradas de DNS. Substituir [domínio] com o domínio principal de seu site (por exemplo, &quot;company.com&quot;) e [corpIP] com o endereço IP do servidor de email corporativo (por exemplo, &quot;255.255.255.255&quot;). Se você enviar emails de vários domínios pelo Marketo, deverá adicioná-los a cada domínio (em uma linha).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se você tiver um registro SPF em seu domínio**

Se você já tiver um registro SPF em sua entrada DNS, adicione o seguinte a ele:

include:mktomail.com

## Configurar DKIM {#set-up-dkim}

**O que é o DKIM? Por que quero configurar o DKIM?**

O DKIM é um protocolo de autenticação usado por destinatários de email para determinar se uma mensagem de email foi enviada por quem ela diz que foi enviada. O DKIM geralmente melhora a capacidade de delivery de emails para a caixa de entrada, pois um receptor pode ter certeza de que a mensagem não é uma falsificação.

**Como funciona o DKIM?**

Depois de configurar a chave pública no registro DNS e ativar o domínio de envio na seção de administração (A), ativaremos a assinatura DKIM personalizada para suas mensagens de saída, que incluirá uma assinatura digital criptografada com cada email que enviarmos para você (B). Os recipients poderão descriptografar a assinatura digital pesquisando a &quot;chave pública&quot; no DNS (C) do domínio de envio. Se a chave no email corresponder à chave em seu registro DNS, o servidor de email de recebimento terá maior probabilidade de aceitar o email Marketo enviado em seu nome.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Como configurar o DKIM?**

Consulte [Configurar uma assinatura DKIM personalizada](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [Saiba mais sobre o SPF e como ele funciona](http://www.open-spf.org/Introduction/)
>* [Ferramentas de capacidade de entrega de email do Marketo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [O meu SPF está configurado corretamente?](https://www.kitterman.com/spf/validate.html)
>* [Eu usei a sintaxe correta?](http://www.open-spf.org/SPF_Record_Syntax/)

