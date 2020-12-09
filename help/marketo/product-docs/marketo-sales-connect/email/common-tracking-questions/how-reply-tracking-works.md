---
unique-page-id: 14352482
description: Como o rastreamento de resposta funciona - Documentos de marketing - Documentação do produto
title: Como o rastreamento de resposta funciona
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Como o rastreamento de resposta funciona {#how-reply-tracking-works}

O rastreamento de resposta é feito observando uma ID de mensagem que está em cada email enviado. Cada email contém uma ID de mensagem exclusiva que nos permite ter alguns dos melhores rastreamentos de resposta.

>[!PREREQUISITES]
>
>**Conexão com o Servidor de email:** O Sales Connect deve estar conectado à sua caixa de entrada para que possamos saber quando uma nova resposta chegou. Você precisará ter sua conta do Sales Connect [conectada ao Gmail](http://docs.marketo.com/x/kYMOAQ). Se você estiver usando o Outlook, precisaremos fazer a integração com seu servidor [](http://toutapp.com/next#settings/exchange_settings)Exchange.

Se o Sales Connect não conseguir rastrear a resposta do prospecto ao seu email, ele não poderá parar uma campanha com base na detecção de resposta ou registrar a resposta ao Salesforce.  O que queremos dizer com qualquer endereço de email que possa responder?

Isso significa que se você enviar um email [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) e ele responder com [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad), nós poderemos rastrear a resposta. Além disso, se você enviar emails [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) e CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153)e o Alan escrever de volta, ele também detectará a resposta e encerrará a campanha.
