---
description: Visão geral do Live Chat - Documentação do Marketo - Documentação do produto
title: Visão geral do bate-papo ao vivo
feature: Dynamic Chat
exl-id: f6563e73-4b6e-437d-bf8b-ec72a9b8bcb3
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 2%

---

# Visão geral do bate-papo ao vivo {#live-chat-overview}

O bate-papo ao vivo permite que os visitantes do site se envolvam em conversas de bate-papo em tempo real com seus agentes de vendas.

## Adicionar agentes de bate-papo ao vivo {#add-live-chat-agents}

Para começar a usar o chat ao vivo, será necessário adicionar seus agentes de chat ao vivo como [usuários na Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Depois disso, você pode adicionar um [chat ao vivo](#using-the-live-chat-card) para uma caixa de diálogo nova ou existente.

Quando os visitantes solicitarem o chat com um agente por meio da Caixa de diálogo, os agentes terão vários [opções de notificação](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} onde eles podem começar a conversar com o visitante.

## Usar o cartão de chat ao vivo {#using-the-live-chat-card}

Use o cartão de chat ao vivo no [Designer de fluxo](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} quando quiser que os visitantes conversem com um agente em tempo real.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>O cartão de chat ao vivo deve ser sempre o último cartão na ramificação. Se a placa for colocada em um ponto aleatório na ramificação, o visitante poderá se surpreender ao conectá-la repentinamente a um agente.

### Práticas recomendadas {#best-practices}

* Use um cartão de perguntas antes do cartão de chat ao vivo perguntando ao visitante se ele deseja se conectar.
* Depois que o visitante concordar em se conectar, use o cartão de captura de informações para coletar algumas informações, como nome/sobrenome, endereço de email, cargo etc. (é recomendável solicitar pelo menos o nome e o endereço de email).

## Opções de Cartão de Bate-papo ao Vivo {#live-chat-card-options}

Clicar no cartão de chat ao vivo no stream permite escolher como o visitante é roteado. Escolha entre round robin, um agente, regras personalizadas ou uma equipe.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round Robin</b></td>
   <td>Os bate-papos são atribuídos aos agentes em ordem sequencial.</td>
  </tr> 
  <tr> 
   <td><b>Agente</b></td>
   <td>Escolha um agente específico para receber o chat.</td>
  </tr>
    <tr> 
   <td><b>Regras personalizadas</b></td>
   <td>Todas as regras personalizadas serão percorridas ao considerar para onde encaminhar o visitante. Se o visitante não se qualificar para nenhuma regra personalizada, ele receberá a <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">mensagem de fallback do chat ao vivo</a>.</td>
  </tr> 
  <tr> 
   <td><b>Equipe</b></td>
   <td>Escolha uma equipe específica para receber o chat. Se essa opção for escolhida, ela será atribuída em rodízio dentro dessa equipe.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Caixa de entrada do agente](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
