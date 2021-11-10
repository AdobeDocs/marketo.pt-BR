---
description: Visão geral do rastreamento de email - Documentos do Marketo - Documentação do produto
title: Visão geral do rastreamento de email
hide: true
hidefromtoc: true
source-git-commit: 8789ed464f532bbe76c2cb456374d9c0f505ece0
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Visão geral do rastreamento de email {#email-tracking-overview}

## Como o rastreamento de resposta funciona {#how-reply-tracking-works}

O Rastreamento de resposta é feito observando uma ID de mensagem que está em cada email enviado. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores rastreamentos de resposta.

>[!PREREQUISITES]
>
>Conexão com o Servidor de email: O Sales Connect deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta chega. Você precisará ter sua conta do Sales Connect conectada ao Gmail. Se você estiver usando o Outlook, precisaremos fazer a integração com seu servidor do Exchange.

Se o Sales Connect não conseguir rastrear a resposta do seu prospecto ao seu email, ele não poderá parar uma campanha com base na detecção de resposta ou registrar a resposta ao Salesforce. O que queremos dizer com qualquer endereço de email que possa responder?

Isso significa que, se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan escrever de volta, ele também detectará a resposta e encerrará a campanha.

## Como o rastreamento de resposta funciona {#how-reply-tracking-works}

texto

## Como rastrear seus anexos de email {#how-to-track-your-email-attachments}

