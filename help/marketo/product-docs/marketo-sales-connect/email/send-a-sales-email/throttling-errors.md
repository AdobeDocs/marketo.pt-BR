---
unique-page-id: 14352581
description: Erros de limitação - Documentos de marketing - Documentação do produto
title: Erros de limitação
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Erros de limitação {#throttling-errors}

## Limite de arquivo atingido {#file-limit-reached}

Se você estiver enviando seu próprio servidor, ele terá limitações para o número de emails que você pode enviar simultaneamente. Ao enviar pelo Sales Connect, você pode enviar muitos e-mails, mas tentamos enviá-los todos ao mesmo tempo. Portanto, se você estiver ciente de que seu servidor vai cortar você em 100 emails por minuto, você precisará enviar apenas 100 emails pelo aplicativo [](http://toutapp.com/login)web. Caso contrário, os e-mails podem chegar aqui devido aos e-mails serem reduzidos no seu servidor.

## Erro de autenticação {#authentication-error}

Isso significa que não foi possível autenticar a conexão com seu servidor SMTP. Provavelmente, sua senha foi alterada recentemente e você só precisa autenticar suas novas credenciais.

Para fazer isso, acesse suas Configurações [SMTP](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

Acesse seus Delivery com falha para tentar reenviar esses emails.
