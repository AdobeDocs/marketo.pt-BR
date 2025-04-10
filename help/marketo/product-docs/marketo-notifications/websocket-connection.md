---
description: Notificação - Conexão Websocket - Documentação do Marketo - Documentação do produto
title: Notificação - Conexão Websocket
hide: true
hidefromtoc: true
exl-id: 00c754f8-3850-4209-803d-5cdb108dc6dc
source-git-commit: eb3e7983f7521d025dff1f5d79b8caeaeb0f622c
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notificação: Conexão Websocket {#notification-websocket-connection}

Este documento é para usuários do Marketo Engage que receberam a seguinte notificação em suas instâncias do Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are currently connected to. Please work with your IT Team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Incluir na lista de permissões Se você ou sua organização usarem configurações restritivas de firewall ou servidor proxy, talvez você ou o administrador de rede precise pesquisar determinados domínios e intervalos de endereço IP para garantir que o Adobe Marketo Engage funcione conforme esperado.

O Suporte da Marketo não está configurado para ajudar na implementação dos protocolos abaixo. Se precisar de assistência, compartilhe este documento com sua equipe de TI. Se eles restringirem o acesso à Web usando um incluo na lista de permissões, peça que eles adicionem os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets do Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
