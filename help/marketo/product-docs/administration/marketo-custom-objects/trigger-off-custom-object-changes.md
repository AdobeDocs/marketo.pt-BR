---
unique-page-id: 11378713
description: Acionador de alterações no objeto personalizado - Documentos do Marketo - Documentação do produto
title: Acionar Alterações no Objeto Personalizado
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
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
>Entre em contato [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para ativar os Acionadores de alteração de objeto personalizado.

Na lista inteligente de uma campanha inteligente, é possível acionar uma ação de fluxo quando um objeto personalizado é adicionado a uma pessoa ou empresa. Você também pode criar uma lista inteligente que use uma *alterar* em um objeto personalizado como acionador. Por exemplo, use-o para enviar um email quando o nome de um curso for atualizado.

>[!NOTE]
>
>Uma entrada do log de atividades não é criada quando um registro de objeto personalizado é alterado.

1. No Marketo, acesse **Atividades de marketing.**

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Crie ou abra uma Campanha inteligente existente e selecione a Lista inteligente.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Procure o acionador necessário e arraste-o para a tela.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Selecione o atributo do acionador.

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Como opção, defina uma restrição.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. E aí está. A alteração é salva automaticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

