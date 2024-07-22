---
unique-page-id: 14352482
description: Como O Rastreamento De Resposta Funciona - Documentação Do Marketo - Documentação Do Produto
title: Como funciona o rastreamento de resposta
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Como funciona o rastreamento de resposta {#how-reply-tracking-works}

O rastreamento de resposta é feito observando uma ID de mensagem que está em todos os emails enviados. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores controles de resposta disponíveis.

>[!PREREQUISITES]
>
>**Conexão com o Servidor de Email:** O Sales Connect deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta for recebida. É necessário ter sua conta do Sales Connect [conectada ao Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se você estiver usando o Outlook, precisaremos integrar com seu [servidor Exchange](https://toutapp.com/next#settings/exchange_settings).

Se o Sales Connect não puder acompanhar a resposta do seu cliente potencial ao email, ele não poderá interromper uma campanha com base na detecção de resposta ou registrar essa resposta ao Salesforce.  O que significa que qualquer endereço de email pode responder?

Isso significa que se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan enviar uma resposta, ele também detectará a resposta e encerrará a campanha.
