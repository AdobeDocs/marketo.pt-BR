---
description: '[!DNL Dynamic Chat] Atividades - Documentação do Marketo - Documentação do produto'
title: '[!DNL Dynamic Chat] atividades'
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 4%

---

# [!DNL Dynamic Chat] atividades {#dynamic-chat-activities}

O [!DNL Dynamic Chat] oferece vários filtros e acionadores para uso nas suas Smart Lists.

![](assets/dynamic-chat-activities-1.png)

## Definições {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>Acionado</b></td>
    <td>Um evento de acionador ocorre quando um visitante atende aos critérios de direcionamento para um Fluxo de diálogo ou de conversa e é mostrado na Caixa de diálogo.
    <br>Um evento de acionador por visitante, por sessão.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Envolvido com um Fluxo de conversa/Caixa de diálogo</b></td>
    <td>Um engajamento ocorre na primeira vez que um visitante da Web clica em um prompt em um Fluxo de diálogo ou de conversa (clicando em uma opção de múltipla escolha, enviando informações, marcando uma reunião, abrindo um documento etc.). Se um visitante abrir uma caixa de diálogo ou um fluxo de conversa, mas não clicar em um prompt, um envolvimento será <b>não</b> registrado.
    <br>Um evento de envolvimento por visitante, por sessão.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Engajado com um agente</b></td>
    <td>Ocorre quando um visitante é conectado com êxito a um agente de chat ao vivo.
    <br>Um usuário envolvido com um evento de agente por visitante, por sessão.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Interagiu com o documento</b></td>
    <td>Ocorre quando um visitante clica em um documento em um cartão de documento.
    <br>Pode haver várias interações de documento por visitante, por sessão.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Meta(s) atingida(s)</b></td>
    <td>Acontece quando um visitante atinge uma meta. <br>Pode haver vários eventos de meta atingida por visitante, por sessão.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Reunião agendada</b></td>
    <td>Acontece quando um visitante agenda uma reunião com um agente do Dynamic Chat.
    <br>Pode haver vários eventos marcados para reunião por visitante, por sessão.</td>
  </tr>
</tbody>
</table>

## Itens a Observar {#things-to-note}

* As condições são suportadas nas etapas de fluxo [!DNL Dynamic Chat]
* [!DNL Dynamic Chat] atividades podem ser sincronizadas com [[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* Você pode exibir [!DNL Dynamic Chat] atividades individuais no Log de atividades de um registro de Pessoa
