---
description: Notificação - Conexão Websocket - Documentação do Marketo - Documentação do produto
title: Notificação - Conexão Websocket
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 10fe526c672867b93b54e99e492e59c0541c3f36
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 0%

---

# Notificação: Conexão Websocket {#notification-websocket-connection}

Este artigo é para usuários do Marketo Engage que receberam a seguinte notificação em suas instâncias do Marketo: `"We were unable to establish a websocket connection to <some-server.adobe.net>. We are ending support of the servers you are connected to now on March 3, 2024. Please work with your IT team to allowlist required Marketo Engage and Adobe domains and ports to prevent access disruptions."`

Incluir na lista de permissões Se você ou sua organização usarem configurações restritivas de firewall ou servidor proxy, talvez você ou o administrador de rede precise pesquisar determinados domínios e intervalos de endereço IP para garantir que o Adobe Marketo Engage funcione conforme esperado.

O Suporte da Marketo não está configurado para ajudar na implementação dos protocolos abaixo. Se precisar de assistência, compartilhe este artigo com sua equipe de TI. Se eles restringirem o acesso à Web usando um incluo na lista de permissões, peça que eles adicionem os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets do Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`
