---
unique-page-id: 14352482
description: Como O Rastreamento De Resposta Funciona - Documentação Do Marketo - Documentação Do Produto
title: Como funciona o rastreamento de respostas
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 4%

---

# Como funciona o rastreamento de respostas {#how-reply-tracking-works}

O rastreamento de resposta é feito observando uma ID de mensagem que está em todos os emails enviados. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores controles de resposta disponíveis.

>[!PREREQUISITES]
>
>**Conexão com o Servidor de Email:** [!DNL Sales Connect] deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta for recebida. É necessário que a sua conta [!DNL Sales Connect] [esteja conectada ao Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Se você estiver usando o [!DNL Outlook], precisaremos integrar com seu [servidor exchange](https://toutapp.com/next#settings/exchange_settings).

Se [!DNL Sales Connect] não puder acompanhar a resposta do cliente potencial ao email, ele não poderá interromper uma campanha com base na detecção de resposta ou registrar essa resposta para [!DNL Salesforce].  O que significa que qualquer endereço de email pode responder?

Isso significa que, se você enviar um email para <flynn@flynnsarcade.com> e ele responder com <kevinf@flynnsarcade.com>, poderemos acompanhar a resposta. Além disso, se você enviar um email para <flynn@flynnsarcade.com> e CC <alan@encom.com>, e Alan lhe enviar uma resposta, ele também detectará a resposta e encerrará a campanha.
