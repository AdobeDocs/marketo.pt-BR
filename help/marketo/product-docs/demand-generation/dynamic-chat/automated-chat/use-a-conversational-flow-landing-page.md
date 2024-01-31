---
description: Usar uma página de aterrissagem de fluxo de conversa - Documentação do Marketo - Documentação do produto
title: Usar uma página de aterrissagem de fluxo de conversa
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Usar uma página de aterrissagem de fluxo de conversa{#use-a-conversational-flow-landing-page}

Incorporar um fluxo de conversa de Dynamic Chat diretamente em uma página de aterrissagem de Marketo Engage permite que os visitantes agendem uma reunião por meio do Dynamic Chat sem precisar preencher um formulário ou interagir com um chatbot.

>[!PREREQUISITES]
>
>Criar uma [Fluxo de conversa](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) que contenha apenas um **Reserva da reunião** cartão.

## Páginas de aterrissagem guiadas {#guided-landing-pages}

Incorpore o seguinte código ao modelo de Página de aterrissagem guiada: `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Abra o modelo Página de aterrissagem guiada no editor e selecione o espaço reservado para Fluxo de conversa.

Clique no menu suspenso Fluxo de conversa e selecione o CF criado na Etapa 1.

Sempre manter Tipo de Entrega como **Em linha**. Clique em **Inserir**.

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

