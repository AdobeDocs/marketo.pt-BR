---
unique-page-id: 10094188
description: Aprovar um objeto personalizado - Documentos de marketing - Documentação do produto
title: Aprovar um objeto personalizado
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Aprovar um objeto personalizado {#approve-a-custom-object}

Você deve aprovar um objeto personalizado antes de poder usá-lo. O processo é ligeiramente diferente para novos objetos personalizados e para objetos que você editou.

## Aprovar um novo objeto personalizado {#approve-a-new-custom-object}

Você criou um novo objeto personalizado. Aqui está como aprová-lo.

1. Em Admin, clique em **Marcar objetos** personalizados e selecione um objeto que esteja em um estado de Rascunho.

   ![](assets/one.png)

1. Clique no menu suspenso Ações **de objeto** personalizado e selecione **Aprovar objeto**.

   ![](assets/two.png)

1. O estado é alterado para Aprovado.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Um objeto personalizado usado em uma estrutura ** um para muitos deve ter pelo menos um campo de dedupe, um campo de link, um nome de objeto vinculado e um nome de campo vinculado a ser aprovado.
   >
   >
   >Um objeto personalizado usado em uma estrutura *muitas para muitas* não **** precisa de um campo de link, nome de objeto vinculado ou nome de campo vinculado ao aprová-lo (porque eles vivem no objeto intermediário).
   >
   >
   >Um objeto personalizado usado como objeto ** intermediário requer um campo de link, um nome de objeto vinculado e um nome de campo vinculado, mas **não** requer um campo de dedupe.
   >
   >
   >Consulte [Compreensão de objetos](understanding-marketo-custom-objects.md) personalizados de marketing para obter mais informações.

É isso! Agora, você pode selecionar seu objeto personalizado nas restrições de seus filtros e acionadores para usar em suas campanhas.

## Aprovar um objeto personalizado editado {#approve-an-edited-custom-object}

Depois de editar um objeto personalizado aprovado, você deve aprovar o rascunho para retornar o objeto personalizado a um estado Aprovado.

1. Quando você edita um objeto personalizado já aprovado, ele recebe um estado Aprovado com rascunho.

   ![](assets/four.png)

1. Quando estiver pronto para aprovar o rascunho, clique no menu suspenso Ações **de objeto** personalizado e selecione **Aprovar objeto**.

   ![](assets/five-1.png)

1. Uma pré-visualização exibe os itens que foram alterados no rascunho. Clique em **Aprovar**.

   ![](assets/six-1.png)

