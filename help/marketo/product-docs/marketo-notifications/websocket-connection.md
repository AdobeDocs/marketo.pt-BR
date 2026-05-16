---
description: Detalhes de notificação para usuários do Marketo Engage que receberam a notificação Não foi possível estabelecer uma conexão Websocket
title: Notificação - Conexão Websocket
hide: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
TQID: https://experienceleague.adobe.com/NpcRnxQPi03CF8z77Urrfs2P2phkuRbh2pd5J1UquFk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 123
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
