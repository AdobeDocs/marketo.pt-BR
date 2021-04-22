---
unique-page-id: 37356429
description: Criar tarefa na Microsoft - Documentação do Marketo - Documentação do produto
title: Criar tarefa na Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Criar tarefa na Microsoft {#create-task-in-microsoft}

Como comerciante, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para informá-las sobre o que devem fazer e quando devem fazê-lo.

Criar tarefa na Microsoft cria uma tarefa em Atividades relacionadas com a Pessoa (Cliente Potencial ou Contato) na Microsoft.

>[!NOTE]
>
>Esta etapa do fluxo **só funcionará quando for usada com acionadores**, não filtros, em sua campanha inteligente.

Por padrão, a etapa de fluxo terá esta aparência:

![](assets/msd1.png)

>[!NOTE]
>
>Quando o Usuário do Marketo Sync está criando tarefas, **Vencimento em** é um campo obrigatório para a tarefa ser criada na Microsoft. Por padrão, a Marketo inserirá cinco dias se nenhum valor for inserido.

Personalize todos os campos para criar a tarefa da maneira que desejar.

![](assets/msd2.png)

>[!NOTE]
>
>O campo &quot;Status&quot; especificado para a tarefa na Ação de fluxo atualiza o campo: &quot;Razão do Status&quot; na Microsoft.

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no **Assunto** e **Descrição**. Consulte [Tokens para Etapas de fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) para obter mais detalhes.
