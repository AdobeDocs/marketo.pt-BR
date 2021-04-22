---
unique-page-id: 11378713
description: Acionador de alterações no objeto personalizado - Documentos do Marketo - Documentação do produto
title: Acionar Alterações no Objeto Personalizado
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Acionar Alterações no Objeto Personalizado {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Este recurso está disponível somente:
>
>* Para clientes na infraestrutura Orion
>* Para uso somente com objetos personalizados do Marketo, não objetos personalizados sincronizados por meio da integração nativa do Salesforce ou do Microsoft Dynamics
>* Como acionador, não um filtro

>
>
Entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para ativar os Acionadores de alteração de objeto personalizado.

Na lista inteligente de uma campanha inteligente, é possível acionar uma ação de fluxo quando um objeto personalizado é adicionado a uma pessoa ou empresa. Você também pode criar uma lista inteligente que usa uma *change* em um objeto personalizado como acionador. Por exemplo, use-o para enviar um email quando o nome de um curso for atualizado.

>[!NOTE]
>
>Uma entrada do log de atividades não é criada quando um registro de objeto personalizado é alterado.

1. No Marketo, vá para **Marketing Activities.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Crie ou abra uma Campanha inteligente existente e selecione a Lista inteligente.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Procure o acionador necessário e arraste-o para a tela.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Selecione o atributo do acionador.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Como opção, defina uma restrição.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. E aí está. A alteração é salva automaticamente.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

