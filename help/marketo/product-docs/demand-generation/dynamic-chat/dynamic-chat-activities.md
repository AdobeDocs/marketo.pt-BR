---
description: Atividades do Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Atividades Dynamic Chat
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: b1101617ec670d42aed8c35044b656ba5fa0f9f5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Atividades Dynamic Chat {#dynamic-chat-activities}

O Dynamic Chat oferece vários filtros e acionadores para uso nas suas Smart Lists.

![](assets/dynamic-chat-activities-1.png)

## Definições {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td><b>Acionado</b></td>
    <td>Um evento de acionador ocorre quando um visitante atende aos critérios de direcionamento para um Fluxo de diálogo ou de conversa e é mostrado na Caixa de diálogo.
    <br>Um evento de acionador por visitante, por sessão.</td>
  </tr>
  <tr>
    <td><b>Envolvido com um Fluxo de conversa/Caixa de diálogo</b></td>
    <td>Um engajamento ocorre na primeira vez que um visitante da Web clica em um prompt em um Fluxo de diálogo ou de conversa (clicando em uma opção de múltipla escolha, enviando informações, marcando uma reunião, abrindo um documento etc.). Se um visitante abrir um Fluxo de diálogo ou de conversa, mas não clicar em um prompt, um engajamento será <b>não</b> registrado. 
    <br>Um evento de engajamento por visitante, por sessão.</td>
  </tr>
   <tr>
    <td><b>Envolvido com um agente</b></td>
    <td>Ocorre quando um visitante é conectado com êxito a um agente de chat ao vivo.
    <br>Um envolvido com evento de agente por visitante, por sessão.</td>
  </tr>
  <tr>
    <td><b>Interagiu com o documento</b></td>
    <td>Ocorre quando um visitante clica em um documento em um cartão de documento.
    <br>Pode haver várias interações de documento por visitante, por sessão.</td>
  </tr>
  <tr>
    <td><b>Meta(s) atingida(s)</b></td>
    <td>Acontece quando um visitante atinge uma meta. <br>Pode haver vários eventos alcançados por meta por visitante, por sessão.</td>
  </tr>
  <tr>
    <td><b>Reunião Agendada</b></td>
    <td>Acontece quando um visitante reserva uma reunião com um agente de Dynamic Chat.
    <br>Pode haver vários eventos marcados para reuniões por visitante, por sessão.</td>
  </tr>
</tbody>
</table>

## Itens a Observar {#things-to-note}

* As condições são suportadas nas etapas de fluxo de Dynamic Chat
* As atividades do Dynamic Chat podem ser sincronizadas com o [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* É possível exibir atividades de Dynamic Chat individuais no Registro de atividade de um registro de pessoa
