---
unique-page-id: 14352476
description: Campo de tipo de atividade no Tarefa (SFDC) - Documentos de marketing - Documentação do produto
title: Campo de tipo de atividade no Tarefa (SFDC)
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Campo Tipo de atividade no Tarefa (SFDC) {#activity-type-field-on-tasks-sfdc}

Com a ajuda do Sales Connect, você pode receber e-mails e chamadas registradas como uma atividade no Salesforce. Uma parte importante para ter dados valiosos no Salesforce é fazer com que o campo Tipo preencha o valor correto.

>[!NOTE]
>
>O registro de emails via BCC não será exibido na lista de seleção de tipo de Tarefa e preencherá automaticamente o campo de tipo como &quot;email&quot;, pois eles estão sendo entregues ao Salesforce por meio do seu endereço BCC.

## Requisitos {#requirements}

* Conexão com o Salesforce
* Nenhum valor de Tipo padrão selecionado na lista de opções Tipo de Tarefa
* A chamada, a resposta e o e-mail devem existir na lista de opções Tipo de Tarefa (questões de capitalização)
* Nenhuma ação de `Workflows` ou `Triggers` no valor do campo Tipo

## Configuração {#setup}

Primeiro verifique se você tem os valores corretos da lista de seleção em vigor. Você precisará da ajuda do administrador do Salesforce para fazer quaisquer alterações na sua lista de opções.

1. Navegue até [Salesforce.com](http://Salesforce.com) e clique em Configuração no canto superior direito.
1. Clique em Personalizar.
1. Clique em Atividade.
1. Clique em Campos de Tarefa.
1. Clique em Tipo.
1. Agora você está na Lista de opções de tipo de Tarefa. Verifique se não há um &#39;Padrão&#39; selecionado.
1. Verifique se há um valor de Tipo listado para Email, Chamada e Resposta.

Agora que isso está em vigor, você começará a ver o campo Tipo preenchendo o valor correspondente para e-mails, chamadas e respostas registrados. Esses valores serão **e não** preenchidos nas tarefas de lembrete do Sales Connect.

>[!NOTE]
>
>Se não vir &#39;Responder&#39; como um valor, adicione-o clicando em **Novo**. &#39;Reply&#39; não é um valor padrão no Salesforce.
