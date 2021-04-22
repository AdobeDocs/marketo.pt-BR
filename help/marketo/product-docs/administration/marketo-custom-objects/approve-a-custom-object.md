---
unique-page-id: 10094188
description: Aprovar um objeto personalizado - Documentos do Marketo - Documentação do produto
title: Aprovar um objeto personalizado
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Aprovar um objeto personalizado {#approve-a-custom-object}

Você deve aprovar um objeto personalizado antes de usá-lo. O processo é um pouco diferente para novos objetos personalizados e os que você editou.

## Aprovar um novo objeto personalizado {#approve-a-new-custom-object}

Você criou um novo objeto personalizado. Aqui está como aprová-lo.

1. Em Admin, clique em **Marketo Custom Objects** e selecione um objeto que esteja em um estado de Rascunho.

   ![](assets/one.png)

1. Clique no menu suspenso **Custom Object Actions** e selecione **Approve Object**.

   ![](assets/two.png)

1. O estado é alterado para Approved.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Um objeto personalizado usado em uma _estrutura one-to-many_ deve ter pelo menos um campo de dedupe, um campo de link, um nome de objeto vinculado e um nome de campo vinculado a ser aprovado.
   >
   >Um objeto personalizado usado em uma _estrutura de muitos para muitos_ **não** precisa de um campo de link, nome de objeto vinculado ou um nome de campo vinculado ao aprová-lo (porque eles vivem no objeto intermediário).
   >
   >Um objeto personalizado usado como _objeto intermediário_ requer um campo de link, nome de objeto vinculado e nome de campo vinculado, mas **não** requer um campo de dedupe.
   >
   >Consulte [Entendendo objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações.

Pronto! Agora, é possível selecionar o objeto personalizado nas restrições dos filtros e acionadores a serem usados nas campanhas.

## Aprovar um objeto personalizado editado {#approve-an-edited-custom-object}

Depois de editar um objeto personalizado aprovado, você deve aprovar o rascunho para retornar o objeto personalizado a um estado Aprovado.

1. Ao editar um objeto personalizado já aprovado, ele recebe um estado Aprovado com Rascunho.

   ![](assets/four.png)

1. Quando estiver pronto para aprovar o rascunho, clique no menu suspenso **Ações do objeto personalizado** e selecione **Aprovar objeto**.

   ![](assets/five-1.png)

1. Uma visualização exibe os itens que foram alterados no rascunho. Clique em **Aprovar**.

   ![](assets/six-1.png)
