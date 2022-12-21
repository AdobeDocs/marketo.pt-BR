---
unique-page-id: 37356429
description: Criar tarefa no Microsoft - Documentos do Marketo - Documentação do produto
title: Criar tarefa no Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Criar tarefa no Microsoft {#create-task-in-microsoft}

Como comerciante, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para informá-las sobre o que devem fazer e quando devem fazê-lo.

Criar tarefa no Microsoft cria uma tarefa em Atividades relacionadas à Pessoa (Cliente Potencial ou Contato) no Microsoft.

>[!NOTE]
>
>Esta etapa de fluxo irá **funcionam somente quando usados com acionadores**, não filtros, em sua campanha inteligente.

Por padrão, a etapa de fluxo terá esta aparência:

![](assets/msd1.png)

>[!NOTE]
>
>Quando o usuário do Marketo Sync está criando tarefas, **Em** é um campo obrigatório para a tarefa ser criada no Microsoft. Por padrão, a Marketo inserirá cinco dias se nenhum valor for inserido.

Personalize todos os campos para criar a tarefa da maneira que desejar.

![](assets/msd2.png)

>[!NOTE]
>
>O campo &quot;Status&quot; especificado para a tarefa na Ação de fluxo atualiza o campo: &quot;Motivo do status&quot; no Microsoft.

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no **Assunto** e **Descrição**. Consulte [Tokens para etapas do fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) para obter mais detalhes.
