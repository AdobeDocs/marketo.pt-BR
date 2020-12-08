---
unique-page-id: 4718683
description: Aprovação de estágios e atribuição de clientes potenciais a um modelo de receita - Documentos do marketing - Documentação do produto
title: Aprovação de estágios e atribuição de clientes potenciais a um modelo de receita
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---


# Aprovação de estágios e atribuição de clientes potenciais a um modelo de receita {#approving-stages-and-assigning-leads-to-a-revenue-model}

Coloque seu **Modelo** de receita **** em funcionamento adicionando clientes potenciais existentes, criando regras de atribuição para quaisquer novos clientes potenciais.

## Aprovação de estágios {#approving-stages}

Vamos aprovar as etapas do seu modelo antes de adicionar qualquer informação potencial.

1. Vá para a ** **área do Analytics.** **

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. Selecione o modelo cujas etapas você gostaria de aprovar.

   ![](assets/image2015-4-28-17-3a10-3a3.png)

1. Em Ações **** do modelo, selecione **Aprovar** **etapas**.

   ![](assets/image2015-4-28-17-3a12-3a37.png)

1. Você será recebido com um alerta. clique em **Atribuir clientes potenciais**.

   ![](assets/image2015-4-28-17-3a5-3a39.png)

Excelente! Vamos seguir em frente e atribuir essas pistas.

## Atribuindo Clientes Potenciais Existentes {#assigning-existing-leads}

[Crie uma Lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) inteligente para identificar os clientes potenciais de um estágio do seu modelo no banco de dados principal.

1. Depois de [criar sua Lista](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)inteligente, clique na guia **Clientes potenciais** .

   ![](assets/image2015-4-29-11-3a37-3a30.png)

1. Clique em **Selecionar tudo** para selecionar os clientes potenciais.

   ![](assets/image2015-4-29-11-3a39-3a39.png)

1. Abra o menu suspenso Ações **** principais e selecione **Especial**. Clique em **Alterar estágio** de receita.

   ![](assets/image2015-4-29-11-3a40-3a38.png)

1. Selecione o **Modelo** correto e o **Palco** correto. Clique em **Executar agora**.

   ![](assets/image2015-4-29-11-3a43-3a41.png)

1. Repita até que todos os clientes potenciais sejam atribuídos às várias etapas do modelo.

Ótimo! Para especificar como novos clientes potenciais são atribuídos a estágios, crie regras de atribuição.

>[!NOTE]
>
>Se o modelo estiver no estado Estágios Aprovados, você não verá nenhum evento Alterar Estágio da Receita nos registros de atividades do cliente potencial. Se o modelo for totalmente aprovado, essa etapa de fluxo será ignorada se você mover um cliente potencial para o mesmo estágio em que ele está atualmente.

## Novos clientes potenciais: Criar regras de atribuição  {#new-leads-create-assignment-rules}

1. Clique novamente em** Marketo Home* e selecione **Analytics**.

   ![](assets/image2015-4-28-17-3a8-3a8.png)

1. `Click your model in the tree, then the`**`Model Actions`**`menu, selecting`**`Assignment Rules`** `.`

   ![](assets/image2015-4-29-11-3a52-3a17.png)

1. `If your assignment rules contain more than just one default choice click **Stage, **make your selection, then click`**`Add Choice`**`.`

   ![](assets/image2015-4-29-12-3a5-3a46.png)

## Exemplo de regra de atribuição {#example-assignment-rule}

Crie uma regra de Pontuação de cliente potencial para atribuir os novos clientes potenciais com uma pontuação mínima a uma etapa apropriada.

1. Em **If**, selecione **Lead Score**. Em seguida, escolha pelo **menos**.
` ![](assets/image2015-4-29-13-3a27-3a8.png)

   `

1. Informe **40** no campo e selecione Lead **** Vendas como Estágio. Clique em **Salvar** para concluir.

   ![](assets/image2015-4-29-14-3a4-3a23.png)

>[!NOTE]
>
>**Artigos relacionados**
>
>Para aprovar seu modelo, leia nossa página de ajuda em ** [Aprovando e não aprovando um modelo](approve-unapprove-a-revenue-model.md)de receita**.

