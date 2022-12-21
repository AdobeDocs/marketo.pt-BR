---
unique-page-id: 14352476
description: Campo de tipo de atividade em tarefas (SFDC) - Documentos do Marketo - Documentação do produto
title: Campo Tipo de Atividade em Tarefas (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# Campo Tipo de Atividade em Tarefas (SFDC) {#activity-type-field-on-tasks-sfdc}

Com a ajuda do Sales Connect, você pode fazer seus emails e chamadas serem registrados como uma atividade no Salesforce. Uma parte importante para ter dados valiosos no Salesforce é fazer com que o campo Type preencha o valor correto.

>[!NOTE]
>
>O registro de emails via Cco não procurará a lista de seleção de tipo de tarefa e preencherá automaticamente o campo de tipo como &quot;email&quot;, pois eles estão sendo entregues ao Salesforce por meio de seu endereço CCO.

## Requisitos {#requirements}

* Conexão com o Salesforce
* Nenhum valor de Tipo Padrão selecionado na lista de opções de Tipo de Tarefa
* Chamada, Resposta e Email devem existir na lista de seleção Tipo de tarefa (questões de capitalização)
* Nenhum fluxo de trabalho ou acionador executando ações no valor do campo Tipo

## Configuração {#setup}

Primeiro verifique se você tem os valores corretos da lista de seleção em vigor. Você precisará da ajuda do administrador do Salesforce para fazer alterações na sua lista de opções.

1. Navegar para [Salesforce.com](https://salesforce.com) e clique em Configurar no canto superior direito.
1. Clique em Personalizar.
1. Clique em Atividades.
1. Clique em Campos da tarefa.
1. Tipo de clique.
1. Agora você está na Lista de opções do tipo de tarefa. Certifique-se de que não haja um &#39;Padrão&#39; selecionado.
1. Certifique-se de que há um valor de Tipo listado para Email, Chamada e Resposta.

Agora que isso está em vigor, você começará a ver o campo Type preenchido o valor correspondente para Emails, chamadas e respostas registradas. Esses valores **not** ser preenchida em tarefas de lembrete do Sales Connect.

>[!NOTE]
>
>Se você não vir &quot;Responder&quot; como um valor, adicione-o clicando em **Novo**. &#39;Reply&#39; não é um valor padrão no Salesforce.
