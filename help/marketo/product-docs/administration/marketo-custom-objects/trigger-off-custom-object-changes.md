---
unique-page-id: 11378713
description: Acionar Alterações De Objetos Personalizados - Documentação Do Marketo - Documentação Do Produto
title: Acionar Alterações de Objeto Personalizado
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: acaf2b421ed65f74bedf18b121ce54e30c19c721
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Acionar Alterações de Objeto Personalizado {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Este recurso está disponível somente:
>
>* Para uso somente com objetos personalizados do Marketo, não com objetos personalizados sincronizados por meio da integração [!DNL Salesforce] ou [!DNL Microsoft Dynamics] nativa
>* Como acionador, não como filtro
>
>Contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para habilitar os Acionadores de Alteração de Objeto Personalizado.

Em uma lista inteligente de campanha inteligente, é possível acionar uma ação de fluxo quando um objeto personalizado é adicionado a uma pessoa ou empresa. Você também pode criar uma lista inteligente que usa uma _alteração_ em um objeto personalizado como um disparador. Por exemplo, use-o para enviar um email quando um nome de curso for atualizado.

>[!NOTE]
>
>Uma entrada do log de atividades não é criada quando um registro de objeto personalizado é alterado.

1. No Marketo Engage, vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Crie ou abra uma Campanha inteligente existente e selecione a Lista inteligente.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Procure o acionador necessário e arraste-o até a tela.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Selecione o [!UICONTROL atributo do acionador].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Opcionalmente, defina uma restrição.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. E aí está você. A alteração é salva automaticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
