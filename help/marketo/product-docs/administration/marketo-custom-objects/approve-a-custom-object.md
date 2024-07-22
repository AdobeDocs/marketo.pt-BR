---
unique-page-id: 10094188
description: Aprovar um objeto personalizado - Documentação do Marketo - Documentação do produto
title: Aprovar um objeto personalizado
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Aprovar um objeto personalizado {#approve-a-custom-object}

Você deve aprovar um objeto personalizado antes de usá-lo. O processo é um pouco diferente para novos objetos personalizados e para os que você editou.

## Aprovar um novo objeto personalizado {#approve-a-new-custom-object}

Você criou um novo objeto personalizado. Veja como aprová-la.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/approve-a-custom-object-1.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/approve-a-custom-object-2.png)

1. Selecione um objeto que esteja no estado Rascunho.

   ![](assets/approve-a-custom-object-3.png)

1. Clique no menu suspenso **[!UICONTROL Ações de Objetos Personalizados]** e selecione **[!UICONTROL Aprovar Objeto]**.

   ![](assets/approve-a-custom-object-4.png)

1. O estado é alterado para [!UICONTROL Aprovado].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Um objeto personalizado usado em uma _estrutura de um para muitos_ deve ter pelo menos um campo de eliminação de duplicação, um campo de link, um nome de objeto vinculado e um nome de campo vinculado a ser aprovado.
   >
   >Um objeto personalizado usado em uma estrutura _muitos para muitos_ **não** precisa de um campo de link, nome de objeto vinculado ou um nome de campo vinculado ao aprová-lo (porque ele está no objeto intermediário).
   >
   >Um objeto personalizado usado como um _objeto intermediário_ requer um campo de link, um nome de objeto vinculado e um nome de campo vinculado, mas **não** requer um campo de eliminação de duplicação.
   >
   >Consulte [Entendendo os objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações.

Pronto! Agora, você pode selecionar o objeto personalizado nas restrições de seus filtros e acionadores para usar em suas campanhas.

## Aprovar um objeto personalizado editado {#approve-an-edited-custom-object}

Após editar um objeto personalizado aprovado, você deve aprovar o rascunho para retornar o objeto personalizado ao estado Aprovado.

1. Ao editar um objeto personalizado já aprovado, ele recebe um estado [!UICONTROL Aprovado com Rascunho].

   ![](assets/approve-a-custom-object-6.png)

1. Quando estiver pronto para aprovar o rascunho, clique no menu suspenso **[!UICONTROL Ações de Objetos Personalizados]** e selecione **[!UICONTROL Aprovar Objeto]**.

   ![](assets/approve-a-custom-object-7.png)

1. Uma visualização exibe os itens que foram alterados no rascunho. Clique em **[!UICONTROL Aprovar]**.

   ![](assets/approve-a-custom-object-8.png)
