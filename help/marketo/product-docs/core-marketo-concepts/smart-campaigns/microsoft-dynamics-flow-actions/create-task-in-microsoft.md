---
unique-page-id: 37356429
description: Criar Tarefa na Microsoft - Documentos do Marketing - Documentação do produto
title: Criar Tarefa na Microsoft
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---


# Criar Tarefa no Microsoft {#create-task-in-microsoft}

Como comerciante, você tem informações que podem auxiliar as vendas a fechar negócios. Você pode criar tarefas para informá-los sobre o que eles devem fazer e quando eles devem fazer isso.

Criar Tarefa na Microsoft cria uma tarefa em Atividades relacionadas à Pessoa (cliente potencial ou contato) na Microsoft.

>[!NOTE]
>
>Esta etapa de fluxo **só funcionará quando for usada com acionadores**, não filtros, na sua campanha inteligente.

Por padrão, a etapa de fluxo terá a seguinte aparência:

![](assets/msd1.png)

>[!NOTE]
>
>Quando o usuário de sincronização de marketing está criando o tarefa, **Vencimento em** é um campo obrigatório para a tarefa ser criada na Microsoft. Por padrão, o Marketo inserirá cinco dias se nenhum valor for inserido.

Personalize todos os campos para criar a tarefa da maneira que desejar.

![](assets/msd2.png)

>[!NOTE]
>
>O campo &quot;Status&quot; especificado para a tarefa na Ação de Fluxo atualiza o campo: &quot;Motivo do status&quot; na Microsoft.

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` nas **Assunto** e **Descrição**. Consulte [Tokens para Etapas de Fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md) para obter mais detalhes.
