---
description: Saiba como incorporar um Fluxo de conversa em uma página de aterrissagem do Marketo. Permitir que os visitantes agendem reuniões por meio do Dynamic Chat sem preencher um formulário.
title: Usar uma página de aterrissagem de fluxo de conversa
hide: true
hidefromtoc: 'yes'
feature: Dynamic Chat
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 2%
---
# Usar uma página de aterrissagem de fluxo de conversa{#use-a-conversational-flow-landing-page}

Incorporar um fluxo de conversa do Dynamic Chat diretamente em uma página de aterrissagem do Marketo Engage permite que os visitantes agendem uma reunião por meio do Dynamic Chat sem precisar preencher um formulário ou interagir com um chatbot.

>[!PREREQUISITES]
>
>Crie um [Fluxo de Conversação](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) simples que contenha apenas um cartão **Reserva de reunião**.

## Páginas de destino guiadas {#guided-landing-pages}

Incorpore o seguinte código no modelo de Página de Aterrissagem Guiada: `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Abra o modelo Página de aterrissagem guiada no editor e selecione o espaço reservado para Fluxo de conversa.

Clique no menu suspenso Fluxo de conversa e selecione o CF criado na Etapa 1.

Sempre manter o Tipo de Entrega como **Em linha**. Clique em **Inserir**.

O Fluxo de conversa que você acabou de inserir será exibido como um Elemento à direita.

CAPTURA DE TELA

>[!NOTE]
>
>Nesse momento, o Fluxo de conversa não aparecerá na janela de pré-visualização principal.

## Páginas de aterrissagem de forma livre {#free-form-landing-pages}

Texto

ANOTAÇÕES DA REUNIÃO DO STEVE

lp guiado, novo id div para modelo, escolher fluxo conv

lp de forma livre, ícone de trazer - advertência: adicione observação - quando você colocar o cf no editor, ele não mostrará uma visualização (nenhum espaço reservado também) - &quot;você não verá uma visualização&quot; - na barra lateral, eles verão que o cf está na página - o lp guiado o lista como um elemento - use &quot;neste momento&quot; ao explicar - o recurso entra em funcionamento talvez na semana de 22
