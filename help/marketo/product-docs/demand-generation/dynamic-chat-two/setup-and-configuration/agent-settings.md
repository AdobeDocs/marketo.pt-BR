---
description: Configurações do agente - Documentação do Marketo - Documentação do produto
title: Configurações do agente
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 49421ecf7f8cec6fb94bc138969c0a43b8832537
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 2%

---

# Configurações do agente {#agent-settings}

Configure seu calendário e defina a disponibilidade da reunião/bate-papo ao vivo.

![](assets/agent-settings-1.png)

## Conectar calendário {#connect-calendar}

Na guia Configuração do calendário, conecte seu calendário do Outlook ou Gmail para uso na programação de compromissos no chatbot.

![](assets/agent-settings-2.png)

Assim que o calendário de um usuário for conectado ao Dynamic Chat, ele será adicionado à fila e seu calendário estará disponível para os visitantes do site agendarem compromissos no.

>[!NOTE]
>
>Você pode conectar um calendário por usuário. Se quiser receber reuniões em vários calendários, adicione vários usuários e faça com que cada um deles conecte seus calendários.

Os usuários também podem personalizar o corpo do convite enviado ao visitante ao agendar um compromisso no calendário do usuário. Eles também podem marcar a caixa de seleção na parte inferior para incluir um link Google Meet ou Microsoft Teams (dependendo de qual calendário foi conectado).

![](assets/agent-settings-3.png)

>[!TIP]
>
>Use o ícone de token (chaves) para personalizar emails de confirmação de reserva de reunião usando atributos de pessoa ou empresa.

### Permissões {#permissions}

A configuração com o Outlook concede as seguintes permissões ao Dynamic Chat:

* Acesso total aos seus calendários
* Fazer logon e ler seu perfil
* Manter acesso aos dados aos quais você concedeu acesso
* Ler as configurações da caixa de correio

A configuração com o Google concede as seguintes permissões ao Dynamic Chat:

* Criar, alterar ou excluir calendários
* Atualizar eventos de calendário individuais
* Alterar suas configurações, incluindo quem pode ver seus eventos
* Alterar com quem o calendário é compartilhado
* Acesso ao seu nome, endereço de email, preferência de idioma e imagem do perfil

## Disponibilidade de Reserva de Reunião {#meeting-booking-availability}

Defina o fuso horário e a disponibilidade de hora/dia da semana para receber reservas de reuniões.

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Duração da reunião</b></td>
   <td>Duração máxima da reunião. - O QUE ACONTECE? ENCERRAMENTO AUTOMÁTICO?</td>
  </tr> 
  <tr> 
   <td><b>Tempo de buffer entre reuniões</b></td>
   <td>Tempo definido como buffer após a reunião. Se você a marcar por 30 minutos, ninguém poderá marcar uma reunião com você até 31 minutos após o fim agendado de uma reunião em seu calendário. - 31 ou 30??????????</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>Você pode selecionar vários blocos de tempo no mesmo dia (por exemplo, sexta-feira das 8a-12p _e_ 1p-5p) clicando no link **+** assine à direita.

## Disponibilidade do bate-papo ao vivo {#live-chat-availability}

Defina seu fuso horário e disponibilidade de hora/dia da semana para receber bate-papos ao vivo.

![](assets/agent-settings-5.png)

Se você estiver conectado ao aplicativo, receberá uma notificação no aplicativo de um chat recebido. Se você não estiver conectado, receberá uma notificação do navegador.

>[!IMPORTANT]
>
>A variável [alternância de disponibilidade](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md#availability-toggle){target="_blank"} na Caixa de entrada do agente **substituirá** o que você insere na guia Disponibilidade do chat ao vivo. Portanto, se você estiver programado como disponível de 1p a 5p, mas precisar fazer uma pausa rápida em 3p, não será necessário alterar as configurações do agente. O status de alternância de disponibilidade permanecerá até que você o alterne manualmente ou até que o próximo bloco de tempo em sua disponibilidade seja atingido.

>[!TIP]
>
>Você pode selecionar vários blocos de tempo no mesmo dia (por exemplo, sexta-feira das 8a-12p _e_ 1p-5p) clicando no link **+** assine à direita.
