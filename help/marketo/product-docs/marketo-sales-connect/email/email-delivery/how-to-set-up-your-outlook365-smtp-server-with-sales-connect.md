---
unique-page-id: 14352600
description: Como configurar seu servidor SMTP Outlook365 com o Sales Connect - Documentos do Marketing - Documentação do produto
title: Como configurar seu servidor SMTP Outlook365 com o Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Como configurar seu servidor SMTP Outlook365 com o Sales Connect {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Se sua organização usar o Outlook e você estiver tentando configurar um canal de delivery de email com o Marketing to Sales Connect, recomendamos conectar-se ao servidor Exchange [usando nosso recurso](http://docs.marketo.com/x/Z4AOAQ)de conexão de email.

Para configurar um servidor [SMTP](http://docs.marketo.com/x/zYTS) personalizado como um canal alternativo, o ToutApp exige que você utilize alguma forma de autenticação para fins de segurança. Você pode configurar qualquer servidor SMTP na página [de configuração](http://toutapp.com/next#settings/email-servers/smtp/configure)SMTP. Para configurar um servidor SMTP do Office365, a Microsoft recomenda a seguinte configuração:\
**Servidor** SMTP: smtp.office365.com\
**Porta** do servidor: Porta 587 - Segura\
**Método** de autenticação: Logon (SSL/TLS)\
**Nome de usuário ou logon**: seu endereço de email do Office365\
**Senha**: sua senha de e-mail do Office365\
**Seu domínio**: seu domínio de empresa

Se você ainda tiver problemas ao configurar seu servidor SMTP, entre em contato com seu administrador do Exchange para garantir que as credenciais certas estejam sendo usadas.

>[!NOTE]
>
>Ao enviar pelo seu SMTP do Office365, a Microsoft impõe um limite de 10.000 recipient `limit of 30 messages sent per minute`por dia. Além disso, `each member` da sua equipe que desejar enviar emails por meio do servidor SMTP do Office365 precisará configurá-los com seu próprio endereço de email e senha nas configurações do Sales Connect. Marcar a caixa para a configuração &quot; `Make this deliverability channel to all my team members` `" will not work` desta configuração, de acordo com as políticas de conta do Office365 da Microsoft.

