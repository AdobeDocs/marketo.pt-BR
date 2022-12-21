---
unique-page-id: 14352482
description: Como o rastreamento de resposta funciona - Documentos do Marketo - Documentação do produto
title: Como o rastreamento de resposta funciona
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Como o rastreamento de resposta funciona {#how-reply-tracking-works}

O Rastreamento de resposta é feito observando uma ID de mensagem que está em cada email enviado. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores rastreamentos de resposta.

>[!PREREQUISITES]
>
>**Conexão com o Servidor de email:** O Sales Connect deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta chega. Você precisará ter sua conta do Sales Connect [conectado ao Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se você estiver usando o Outlook, precisaremos fazer a integração com seu [servidor exchange](https://toutapp.com/next#settings/exchange_settings).

Se o Sales Connect não conseguir rastrear a resposta do seu prospecto ao seu email, ele não poderá parar uma campanha com base na detecção de resposta ou registrar a resposta ao Salesforce.  O que queremos dizer com qualquer endereço de email que possa responder?

Isso significa que se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan escrever de volta, ele também detectará a resposta e encerrará a campanha.
