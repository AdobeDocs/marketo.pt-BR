---
unique-page-id: 14352476
description: Campo Tipo de atividade em tarefas (SFDC) - Documentação do Marketo - Documentação do produto
title: Campo Tipo de atividade em tarefas (SFDC)
exl-id: b291e641-d3af-4667-a01c-cd491cd87add
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 6%

---

# Campo Tipo de atividade em tarefas (SFDC) {#activity-type-field-on-tasks-sfdc}

Com a ajuda do [!DNL Sales Connect], você pode registrar seus emails e chamadas como uma atividade no [!DNL Salesforce]. Uma parte chave para ter dados valiosos em [!DNL Salesforce] é ter o campo [!UICONTROL Tipo] preenchendo o valor correto.

>[!NOTE]
>
>O registro de emails via CCO não olhará para a lista de opções Tipo de Tarefa e, em vez disso, preencherá automaticamente o campo de tipo como &quot;email&quot;, pois eles estão sendo entregues para [!DNL Salesforce] por meio do endereço CCO.

## Requisitos {#requirements}

* Conexão com [!DNL Salesforce]
* Nenhum valor de Tipo Padrão selecionado na lista de opções de Tipo de Tarefa
* Chamada, Resposta e Email devem existir na lista de seleção Tipo de tarefa (questões de capitalização)
* Nenhum fluxo de trabalho ou acionador está executando ações no valor do campo Tipo

## Configuração {#setup}

Primeiro, verifique se você tem os valores corretos da lista de seleção em vigor. Você precisará da ajuda do seu administrador [!DNL Salesforce] para fazer quaisquer alterações na sua lista de opções.

1. Navegue até [Salesforce.com](https://salesforce.com) e clique em Configurar no canto superior direito.
1. Clique em **[!UICONTROL Personalizar]**.
1. Clique em **[!UICONTROL Atividades]**.
1. Clique em **[!UICONTROL Campos de tarefa]**.
1. Clique em **[!UICONTROL Tipo]**.
1. Você está agora na Lista de opções de tipos de tarefa. Verifique se não há um &#39;Padrão&#39; selecionado.
1. Verifique se há um valor de [!UICONTROL Tipo] listado para [!UICONTROL Email], [!UICONTROL Chamada] e [!UICONTROL Resposta].

Agora que isso foi feito, você começará a ver o campo Type preenchendo o valor correspondente para Emails, Chamadas e Respostas registrados. Esses valores _não_ serão preenchidos nas tarefas de lembrete do Sales Connect.

>[!NOTE]
>
>Se você não vir &#39;Responder&#39; como um valor, adicione-o clicando em **[!UICONTROL Novo]**. &#39;Responder&#39; não é um valor padrão em [!DNL Salesforce].
