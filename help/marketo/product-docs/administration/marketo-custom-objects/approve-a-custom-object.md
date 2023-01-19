---
unique-page-id: 10094188
description: Aprovar um objeto personalizado - Documentos do Marketo - Documentação do produto
title: Aprovar um objeto personalizado
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: a51ee0b2b513d50febbffd7e3a72874c5ef4679c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Aprovar um objeto personalizado {#approve-a-custom-object}

Você deve aprovar um objeto personalizado antes de usá-lo. O processo é um pouco diferente para novos objetos personalizados e os que você editou.

## Aprovar um novo objeto personalizado {#approve-a-new-custom-object}

Você criou um novo objeto personalizado. Aqui está como aprová-lo.

1. Vá para o **Administrador** área.

   ![](assets/approve-a-custom-object-1.png)

1. Clique em **Objetos personalizados do Marketo**.

   ![](assets/approve-a-custom-object-2.png)

1. Selecione um objeto que esteja no estado Rascunho.

   ![](assets/approve-a-custom-object-3.png)

1. Clique no botão **Ações do objeto personalizado** e selecione **Aprovar objeto**.

   ![](assets/approve-a-custom-object-4.png)

1. O estado é alterado para Approved.

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Um objeto personalizado usado em um _estrutura um para muitos_ deve ter pelo menos um campo de dedupe, um campo de link, um nome de objeto vinculado e um nome de campo vinculado para ser aprovado.
   >
   >Um objeto personalizado usado em um _estrutura muitos para muitos_ **does not** precisa de um campo de link, nome de objeto vinculado ou um nome de campo vinculado ao aprová-lo (porque eles estão no objeto intermediário).
   >
   >Um objeto personalizado usado como um _objeto intermediário_ requer um campo de link, um nome de objeto vinculado e um nome de campo vinculado, mas **does not** requer um campo de dedupe.
   >
   >Consulte [Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações.

Pronto! Agora, é possível selecionar o objeto personalizado nas restrições dos filtros e acionadores a serem usados nas campanhas.

## Aprovar um objeto personalizado editado {#approve-an-edited-custom-object}

Depois de editar um objeto personalizado aprovado, você deve aprovar o rascunho para retornar o objeto personalizado a um estado Aprovado.

1. Ao editar um objeto personalizado já aprovado, ele recebe um estado Aprovado com Rascunho.

   ![](assets/approve-a-custom-object-6.png)

1. Quando estiver pronto para aprovar o rascunho, clique no botão **Ações do objeto personalizado** e selecione **Aprovar objeto**.

   ![](assets/approve-a-custom-object-7.png)

1. Uma visualização exibe os itens que foram alterados no rascunho. Clique em **Aprovar**.

   ![](assets/approve-a-custom-object-8.png)
