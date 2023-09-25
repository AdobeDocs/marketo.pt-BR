---
description: Visão geral do Live Chat - Documentação do Marketo - Documentação do produto
title: Visão geral do bate-papo ao vivo
feature: Dynamic Chat
source-git-commit: 34545817fd35719290a848384e4bc9feba521305
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 3%

---

# Visão geral do bate-papo ao vivo {#live-chat-overview}

O bate-papo ao vivo permite que os visitantes do site se envolvam em conversas de bate-papo em tempo real com seus agentes de vendas.

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
