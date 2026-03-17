---
unique-page-id: 37356429
description: Saiba como criar uma tarefa no Microsoft Dynamics a partir de uma etapa de fluxo. Crie uma tarefa para o proprietário quando alguém entrar no fluxo.
title: Crie tarefa na Microsoft
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 3efcb529cd3e35027f35e51dfd91f95e94af9d61
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 4%

---

# Crie tarefa na Microsoft {#create-task-in-microsoft}

Como profissional de marketing, você tem informações que podem ajudar as vendas a fechar negócios. Você pode criar tarefas para que eles saibam o que devem fazer e quando devem fazê-lo.

Criar Tarefa no Microsoft cria uma tarefa em Atividades relacionadas à Pessoa (Cliente Potencial ou Contato) no [!DNL Microsoft].

>[!NOTE]
>
>Esta etapa do fluxo _só funcionará quando usada com acionadores_, não filtros, na sua campanha inteligente.

Por padrão, a etapa de fluxo será semelhante a:

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Quando o Usuário de Sincronização do Marketo está criando tarefas, **[!UICONTROL Vencimento em]** é um campo obrigatório para a tarefa a ser criada em [!DNL Microsoft]. O Marketo inserirá cinco dias por padrão se nenhum valor for inserido.

Personalize todos os campos para criar a tarefa da maneira que você desejar.

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>O campo &quot;Status&quot; especificado para a tarefa na Ação de Fluxo atualiza o campo: &quot;Motivo do Status&quot; em [!DNL Microsoft].

>[!TIP]
>
>Você pode usar `{{lead.tokens}}`, `{{company.tokens}}`, `{{campaign.tokens}}` e `{{system.tokens}}` no **[!UICONTROL Assunto]** e **[!UICONTROL Descrição]**. Consulte [Tokens para Etapas de Fluxo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"} para obter mais detalhes.
