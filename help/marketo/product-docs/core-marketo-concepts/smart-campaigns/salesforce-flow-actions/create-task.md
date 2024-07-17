---
unique-page-id: 1147017
description: Criar tarefa - Documentação do Marketo - Documentação do produto
title: Criar tarefa
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Criar tarefa {#create-task}

Como profissional de marketing, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para que eles saibam o que devem fazer e quando devem fazê-lo.

![](assets/create-task-1.png)

>[!NOTE]
>
>Quando o usuário do Marketo Sync está criando tarefas, **[!UICONTROL Vencimento em]** é um campo obrigatório para a tarefa a ser criada no Salesforce. O Marketo inserirá cinco dias por padrão se não houver valor.

Por padrão, a etapa de fluxo será semelhante a:

![](assets/create-task-2.png)

Personalize todos os campos para criar a tarefa da maneira que você desejar.

![](assets/create-task-3.png)

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no **[!UICONTROL Assunto]** e **[!UICONTROL Descrição]**. Consulte [Tokens para Etapas de Fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obter mais detalhes.
