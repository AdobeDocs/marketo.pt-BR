---
unique-page-id: 1147017
description: Criar tarefa - Documentação do Marketo - Documentação do produto
title: Criar tarefa
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Criar tarefa {#create-task}

Como profissional de marketing, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para que eles saibam o que devem fazer e quando devem fazê-lo.

![](assets/image2014-9-22-14-3a54-3a46.png)

>[!NOTE]
>
>Quando o usuário do Marketo Sync está criando tarefas, **Vencimento em** é um campo obrigatório para a tarefa a ser criada no Salesforce. O Marketo inserirá cinco dias por padrão se não houver valor.

Por padrão, a etapa de fluxo será semelhante a:

![](assets/image2014-9-22-14-3a54-3a49.png)

Personalize todos os campos para criar a tarefa da maneira que você desejar.

![](assets/image2014-9-22-14-3a54-3a52.png)

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no **Assunto** e **Descrição**. Consulte [Tokens para etapas de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) para obter mais detalhes.
