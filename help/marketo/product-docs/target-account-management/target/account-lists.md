---
unique-page-id: 11378814
description: Listas de contas - Documentação do Marketo - Documentação do produto
title: Listas de contas
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Listas de contas {#account-lists}

Uma lista de contas é uma coleção de contas nomeadas que podem ser segmentadas juntas. As listas de contas permitem que você direcione contas nomeadas por setor, local ou tamanho da empresa.

Além das listas de contas, você também pode criar listas de contas dinâmicas geradas de Exibições de Contas públicas do CRM. Uma Exibição de conta do CRM é um conjunto de regras que atua como filtro ao exibir contas. Por exemplo, você pode usá-lo para encontrar contas em que o setor é da área de saúde *e* A receita é superior a US$ 100 milhões.

![](assets/one.png)

>[!NOTE]
>
>As listas de contas criadas no Gerenciamento de contas do Marketo Target estão disponíveis automaticamente ao criar listas inteligentes e campanhas da Web no [Personalização da Web](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Criar uma nova lista de contas {#create-a-new-account-list}

1. Clique em **Novo** e selecione **Criar nova lista de contas**.

   ![](assets/1a.png)

1. Dê um nome à sua lista e clique em **Criar**.

   ![](assets/three-0.png)

1. Depois de criar sua lista de contas, comece em [adicionar contas nomeadas a ele](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >O Marketo só exibirá insights para listas de contas com 2.000 contas nomeadas ou menos.

## Criar uma nova lista de contas dinâmicas {#create-a-new-dynamic-account-list}

1. Clique em **Novo** e selecione **Criar nova lista dinâmica**.

   ![](assets/1.png)

1. Na caixa de diálogo, selecione uma **Exibição da Conta do CRM** no menu suspenso ou digite o nome para pesquisá-lo.

   ![](assets/image2017-7-18-9-48-23.png)

1. Clique em **Criar**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >No Salesforce, certifique-se de fornecer permissões de Objeto de exibição de lista ao usuário de sincronização.

## Renomear uma lista de contas {#rename-an-account-list}

>[!NOTE]
>
>Essas etapas se aplicam somente às listas de contas. _Dinâmico_ As listas de contas usam o nome de suas Exibições de Contas do CRM associadas.

1. Selecione a conta que deseja renomear, clique no link **Ações da lista de contas** e selecione **Renomear lista de contas**.

   ![](assets/three.png)

1. Insira o novo nome e clique em **Renomear**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >A Exibição de conta do CRM é sincronizada com a lista de contas dinâmicas a cada 8 horas. Se ainda não estiverem sincronizados, o Marketo os sincronizará durante o próximo ciclo.

## Excluir uma lista de contas {#delete-an-account-list}

>[!NOTE]
>
>Essas etapas são as mesmas para listas de contas e listas de contas dinâmicas.

1. Selecione a conta que deseja excluir, clique no link **Ações da lista de contas** e selecione **Excluir lista de contas**.

   ![](assets/five.png)

1. Clique em **Excluir**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Adicionar uma conta nomeada existente a uma lista de contas](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Insights da lista de contas](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
