---
unique-page-id: 37356429
description: Criar tarefa no Microsoft - Documentação do Marketo - Documentação do produto
title: Criar tarefa no Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Criar tarefa no Microsoft {#create-task-in-microsoft}

Como profissional de marketing, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para que eles saibam o que devem fazer e quando devem fazê-lo.

Criar tarefa na Microsoft cria uma tarefa em Atividades relacionadas à pessoa (cliente potencial ou contato) no [!DNL Microsoft].

>[!NOTE]
>
>Esta etapa do fluxo _trabalhar somente quando usado com acionadores_, não filtros, na sua campanha inteligente.

Por padrão, a etapa de fluxo será semelhante a:

![](assets/msd1.png)

>[!NOTE]
>
>Quando o usuário do Marketo Sync está criando tarefas, **[!UICONTROL Vencimento em]** é um campo obrigatório para a tarefa a ser criada em [!DNL Microsoft]. O Marketo inserirá cinco dias por padrão se nenhum valor for inserido.

Personalize todos os campos para criar a tarefa da maneira que você desejar.

![](assets/msd2.png)

>[!NOTE]
>
>O campo &quot;Status&quot; especificado para a tarefa na Ação de fluxo atualiza o campo: &quot;Motivo do status&quot; em [!DNL Microsoft].

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no **[!UICONTROL Assunto]** e **[!UICONTROL Descrição]**. Consulte [Tokens para etapas de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obter mais detalhes.
