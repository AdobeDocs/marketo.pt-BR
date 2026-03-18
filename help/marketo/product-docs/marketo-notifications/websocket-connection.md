---
description: Detalhes de notificação para usuários do Marketo Engage que receberam a notificação Não foi possível estabelecer uma conexão Websocket
title: Notificação - Conexão Websocket
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 30%

---

# Notificação: conexão Websocket {#notification-websocket-connection}

Este documento é para usuários do Marketo Engage que receberam a seguinte notificação em suas instâncias do Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Se você ou sua organização usarem configurações restritivas de firewall ou servidor proxy, talvez você ou o administrador de rede precisem incluir na lista de permissões determinados domínios e intervalos de endereço IP para garantir que o Adobe Marketo Engage funcione conforme esperado.

O Suporte da Marketo não está configurado para ajudar na implementação dos protocolos abaixo. Se precisar de assistência, compartilhe este documento com sua equipe de TI. Se eles restringirem o acesso à Web usando um incluo na lista de permissões, peça que eles adicionem os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets do Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
