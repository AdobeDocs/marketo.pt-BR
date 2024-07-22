---
unique-page-id: 4718683
description: Aprovação de estágios e atribuição de leads a um modelo de receita - Documentação do Marketo - Documentação do produto
title: Aprovando Estágios e Atribuindo Clientes Potenciais a um Modelo de Receita
exl-id: 0c93dfe4-8950-444c-a65b-080620816ba2
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Aprovando Estágios e Atribuindo Clientes Potenciais a um Modelo de Receita {#approving-stages-and-assigning-leads-to-a-revenue-model}

Coloque seu **Modelo de Receita** em funcionamento adicionando clientes potenciais existentes, criando regras de atribuição para quaisquer novos clientes potenciais.

## Aprovando estágios {#approving-stages}

Vamos aprovar os estágios do seu modelo antes de adicionar qualquer cliente em potencial.

1. Vá para a área **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Selecione o modelo cujos estágios você deseja aprovar.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Em **Ações de Modelo**, selecione **Aprovar Estágios**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Você receberá um alerta; clique em **Atribuir clientes em potencial**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Excelente! Vamos seguir em frente e atribuir esses leads.

## Atribuição de Clientes Potenciais Existentes {#assigning-existing-leads}

[Crie uma Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para identificar os clientes potenciais de um estágio do seu modelo no Banco de Dados de Clientes Potenciais.

1. Depois de [criar sua Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md), clique na guia **Clientes Potenciais**.

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Clique em **Selecionar tudo** para selecionar os clientes potenciais.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Abra o menu suspenso **Ações de cliente potencial** e selecione **Especial**. Clique em **Alterar estágio de receita**.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Selecione o **Modelo** correto e o **Estágio** correto. Clique em **Executar Agora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Repita até que todos os clientes em potencial sejam atribuídos aos vários estágios do modelo.

Ótimo! Para especificar como os novos leads são atribuídos aos estágios, crie regras de atribuição.

>[!NOTE]
>
>Se o modelo estiver no estado Estágios aprovados, você não verá eventos de Alterar estágio de receita nos logs de atividade dos clientes potenciais. Se seu modelo for totalmente aprovado, esta etapa do fluxo será ignorada se você mover um cliente em potencial para o mesmo estágio em que ele está no momento.

## Novos Clientes Potenciais: Criar Regras De Atribuição  {#new-leads-create-assignment-rules}

1. Clique novamente em **Marketo Home** e selecione **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Clique no modelo na árvore e, em seguida, no menu **Ações de Modelo**, selecionando **Regras de Atribuição**.

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. Se suas regras de atribuição contiverem mais de uma opção padrão, clique em **Estágio**, faça a seleção e clique em **Adicionar Escolha**.

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exemplo de regra de atribuição {#example-assignment-rule}

Crie uma regra de Pontuação de lead para atribuir os novos leads com uma pontuação mínima a uma etapa apropriada.

1. Em **Se**, selecione **Pontuação de lead**. Escolha **pelo menos**.

   ![](assets/image2015-4-29-13-3a27-3a8.png)

1. Insira **40** no campo e selecione **Vendas Potenciais** como Estágio. Clique em **Salvar** para concluir.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!MORELIKETHIS]
>
>Para aprovar seu modelo, leia nossa página de ajuda em **[Aprovando e Desaprovando um Modelo de Receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)**.
