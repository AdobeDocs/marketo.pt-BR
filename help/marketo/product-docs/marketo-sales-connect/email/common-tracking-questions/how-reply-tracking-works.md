---
unique-page-id: 14352482
description: Como o rastreamento de resposta funciona - Documentos do Marketo - Documentação do produto
title: Como o rastreamento de resposta funciona
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Como o rastreamento de resposta funciona {#how-reply-tracking-works}

O Rastreamento de resposta é feito observando uma ID de mensagem que está em cada email enviado. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores rastreamentos de resposta.

>[!PREREQUISITES]
>
>**Conexão com o Servidor de email:** a Conexão de vendas deve estar conectada à sua caixa de entrada para que saibamos quando uma nova resposta chegou. Você precisará ter sua conta do Sales Connect [conectada ao Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se você estiver usando o Outlook, precisaremos fazer a integração com seu [servidor do exchange](https://toutapp.com/next#settings/exchange_settings).

Se o Sales Connect não conseguir rastrear a resposta do seu prospecto ao seu email, ele não poderá parar uma campanha com base na detecção de resposta ou registrar a resposta ao Salesforce.  O que queremos dizer com qualquer endereço de email que possa responder?

Isso significa que se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan escrever de volta, ele também detectará a resposta e encerrará a campanha.
