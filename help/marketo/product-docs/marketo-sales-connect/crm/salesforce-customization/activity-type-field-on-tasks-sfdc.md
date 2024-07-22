---
unique-page-id: 14352476
description: Campo de tipo de atividade em tarefas (SFDC) - Documentação do Marketo - Documentação do produto
title: Campo Tipo de atividade em tarefas (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Campo Tipo de atividade em tarefas (SFDC) {#activity-type-field-on-tasks-sfdc}

Com a ajuda do Sales Connect, você pode ter seus emails e chamadas registrados como uma atividade no Salesforce. Uma parte essencial para ter dados valiosos no Salesforce é fazer com que o campo Tipo preencha o valor correto.

>[!NOTE]
>
>O registro de emails via CCO não olhará para a lista de opções Tipo de tarefa e preencherá automaticamente o campo tipo como &quot;email&quot;, pois estão sendo entregues ao Salesforce por meio do endereço CCO.

## Requisitos {#requirements}

* Conexão com o Salesforce
* Nenhum valor de Tipo Padrão selecionado na lista de opções de Tipo de Tarefa
* Chamada, Resposta e Email devem existir na lista de seleção Tipo de tarefa (questões de capitalização)
* Nenhum fluxo de trabalho ou acionador está executando ações no valor do campo Tipo

## Configuração {#setup}

Primeiro, verifique se você tem os valores corretos da lista de seleção em vigor. Você precisará da ajuda de seu administrador do Salesforce para fazer alterações na lista de opções.

1. Navegue até [Salesforce.com](https://salesforce.com) e clique em Configurar no canto superior direito.
1. Clique em Personalizar.
1. Clique em Atividades.
1. Clique em Campos de tarefa.
1. Clique em Tipo.
1. Você está agora na Lista de opções de tipos de tarefa. Verifique se não há um &#39;Padrão&#39; selecionado.
1. Verifique se há um valor de Tipo listado para Email, Chamada e Resposta.

Agora que isso foi feito, você começará a ver o campo Type preenchendo o valor correspondente para Emails, Chamadas e Respostas registrados. Esses valores _não_ serão preenchidos nas tarefas de lembrete do Sales Connect.

>[!NOTE]
>
>Se você não vir &#39;Responder&#39; como um valor, adicione-o clicando em **Novo**. &quot;Resposta&quot; não é um valor padrão no Salesforce.
