---
description: Saiba como criar tarefas no Veeva a partir do Marketo para informar às vendas o que fazer e quando. Use a etapa de fluxo Criar tarefa e personalize o assunto, a descrição e a data de vencimento.
title: Criar Tarefa em  [!DNL Veeva]
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
feature: Veeva CRM
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Criar Tarefa em [!DNL Veeva] {#create-task-in-veeva}

Como profissional de marketing, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para que eles saibam o que devem fazer e quando devem fazê-lo.

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Quando o Usuário de Sincronização do Marketo está criando tarefas, **[!UICONTROL Vencimento em]** é um campo obrigatório para a tarefa a ser criada em [!DNL Veeva]. O Marketo inserirá cinco dias por padrão se não houver valor.

Por padrão, a etapa de fluxo será semelhante a:

![](assets/create-task-in-veeva-2.png)

Personalize todos os campos para criar a tarefa da maneira que você desejar.

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no [!UICONTROL Assunto] e [!UICONTROL Descrição]. Consulte [Tokens para Etapas de Fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obter mais detalhes.
