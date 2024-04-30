---
description: Funções de retorno de chamada - Documentação do Marketo - Documentação do produto
title: Funções de retorno de chamada
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 30deeb59cd70b42af38cd1e047833394f9341a5c
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 7%

---

# Funções de retorno de chamada {#callback-functions}

Você pode usar funções de retorno de chamada de widget do Dynamic Chat para enviar eventos de conversação para qualquer plataforma de terceiros.

## Introdução {#getting-started}

Esse evento indica que o widget de Dynamic Chat está pronto para uso e é acionado quando todos os scripts relacionados ao Dynamic Chat são carregados na página da Web.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    // code here will execute when chatbot scripts are loaded in a webpage 
});
```

## Eventos de conversa {#conversation-events}

Esses eventos estão relacionados a uma conversa direcionada em uma página específica para um visitante específico.

### Conversa Acionada

Uma conversa (por exemplo, uma caixa de diálogo) direcionada a um visitante do site é resolvida e o chatbot é exibido para ele.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 

    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
// code here will execute when chatbot is loaded for a visitor 
   });
});
```

### Conversa engajada {#conversation-engaged}

Visitante envolvido (por exemplo, forneceu sua primeira resposta) com o chatbot.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_ENGAGED, (event) => { 
 // code here will execute when visitor engages with chatbot 
    });
});
```

### Conversa concluída {#conversation-completed}

O visitante chegou ao fim da conversa.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_COMPLETED, (event) => { 
 // code here will execute when conversation is completed 
    });
});
```

### Conversa encerrada

O visitante encerrou a conversa antes de chegar ao fim.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_CLOSED, (event) => { 
 // code here will execute when conversation is closed 
    });
});
```

O argumento &#39;event&#39; no evento é um objeto com metadados relacionados à conversa. É possível acessar os metadados por event.data

Abaixo estão alguns valores de metadados principais que você pode acessar:

<table>
<thead>
  <tr>
    <th style="width:75%">Metadados</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome da conversa</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificador da conversa</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversa (fluxo de diálogo/conversa)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interface do usuário (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de Sessão</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Eventos de entrada do visitante

Esses eventos são acionados quando um visitante que está participando de uma conversa fornece suas informações de contato (por exemplo, número de telefone ou endereço de email). Abaixo estão os eventos que se enquadram nessa categoria.

### Número de telefone {#phone-number}

Esse evento é acionado quando um visitante fornece seu número de telefone durante a conversa.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_INPUT_PHONE, (event) => { 
  // code here will execute when a visitor provides their phone number 
    }); 
}); 
```

### ID do e-mail {#email-id}

Esse evento é acionado quando um visitante fornece seu endereço de email durante a conversa.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_INPUT_EMAIL, (event) => { 
 // code here will execute when a visitor provides their email address 
    }); 
});
```

O argumento &#39;event&#39; no evento é um objeto com metadados relacionados à conversa. É possível acessar os metadados por event.data

Abaixo estão alguns valores de metadados principais que você pode acessar.

<table>
<thead>
  <tr>
    <th style="width:75%">Metadados</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome da conversa</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificador da conversa</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversa (fluxo de diálogo/conversa)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interface do usuário (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de Sessão</td>
    <td>payload.sid</td>
  </tr>
</tbody>
</table>

## Eventos de Reserva de Reunião {#meeting-booking-events}

Esses eventos são acionados quando um visitante agenda uma reunião com seu representante de negócios.

Abaixo estão os eventos que se enquadram nessa categoria.

### Reunião marcada {#meeting-booked}

Esse evento é acionado quando um visitante agenda uma reunião no calendário de um agente.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_MEETING_BOOKED, (event) => { 
 // code here will execute when a meeting is booked 
    }); 
});
```

O argumento &#39;event&#39; no evento é um objeto com metadados relacionados à conversa. É possível acessar os metadados por event.data

Abaixo estão alguns valores de metadados principais que você pode acessar.

<table>
<thead>
  <tr>
    <th style="width:75%">Metadados</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome da conversa</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificador da conversa</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversa (fluxo de diálogo/conversa)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interface do usuário (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de Sessão</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nome do agente</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Identificador do agente</td>
    <td>payload.agentID</td>
  </tr>
  <tr>
    <td>Informações da Reunião</td>
    <td>payload.meetingInfo</td>
  </tr>
</tbody>
</table>

## Eventos de bate-papo ao vivo {#live-chat-events}

Esses eventos são acionados quando um visitante se conecta com um agente ativo durante o envolvimento com o chatbot.

Abaixo estão os eventos que se enquadram nessa categoria.

### Chat ao vivo solicitado {#live-chat-requested}

Esse evento é acionado quando um visitante seleciona a opção para conversar com um agente ativo e um agente disponível está sendo resolvido.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUESTED, (event) => { 
 // code here will execute when a visitor requests for live chat 
    }); 
});
```

### Chat ao vivo iniciado {#live-chat-initiated}

Esse evento é acionado quando um visitante seleciona a opção para conversar com um agente ao vivo e um agente aceita o bate-papo.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_INITIATED, (event) => { 
 // code here will execute after a live agent accepted the chat 
    }); 
});
```

### Chat ao vivo encerrado {#live-chat-ended}

Esse evento é acionado quando uma conversa entre um visitante e o agente ativo é encerrada.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_ENDED, (event) => { 
 // code here will execute when a live chat is ended 
    }); 
});
```

### Tempo limite do bate-papo ao vivo {#live-chat-timeout}

Esse evento é acionado quando uma conversa de chat ao vivo atinge o tempo limite porque o visitante para de responder ou é descartado.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_LIVE_CHAT_REQUEST_TIMEOUT, (event) => { 
 // code here will execute when a visitor abandoned live chat 
    }); 
});
```

O argumento &#39;event&#39; no evento é um objeto com metadados relacionados à conversa. É possível acessar os metadados por event.data

Abaixo estão alguns valores de metadados principais que você pode acessar.

<table>
<thead>
  <tr>
    <th style="width:75%">Metadados</th>
    <th style="width:25%">Atributos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Nome da conversa</td>
    <td>payload.name</td>
  </tr>
  <tr>
    <td>Identificador da conversa</td>
    <td>payload.id</td>
  </tr>
  <tr>
    <td>Tipo de conversa (fluxo de diálogo/conversa)</td>
    <td>payload.type</td>
  </tr>
  <tr>
    <td>Tipo de interface do usuário (pop-up/chatbot/inline)</td>
    <td>payload.uiType</td>
  </tr>
  <tr>
    <td>ID de Sessão</td>
    <td>payload.sid</td>
  </tr>
  <tr>
    <td>Nome do agente</td>
    <td>payload.agentName</td>
  </tr>
  <tr>
    <td>Identificador do agente</td>
    <td>payload.agentID</td>
  </tr>
</tbody>
</table>

Se você quiser enviar qualquer um desses eventos para uma plataforma de terceiros, como Adobe Analytics ou Google Analytics, será necessário adicionar a respectiva chamada de rastreamento dentro desses eventos Dynamic Chat. Seria algo parecido com o exemplo abaixo.

```javascript
window.addEventListener('adobedx.conversations.ready', () => { 
    addListener(Enum.Events.CONVERSATION_TRIGGERED, (event) => { 
 // Enter Adobe Analytics or Google Analytics function here 
    ga('send', 'event', { 
      eventCategory: Dynamic Chat Conversations', 
      eventAction: 'Conversation Triggered', 
      eventLabel: event.data.payload.id, 
    }); 
    }); 
});
```
