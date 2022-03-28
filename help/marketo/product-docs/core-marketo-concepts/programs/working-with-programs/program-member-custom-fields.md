---
unique-page-id: 37355569
description: Campos personalizados do membro do programa - Documentos do Marketo - Documentação do produto
title: Campos personalizados do membro do programa
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
source-git-commit: 05f31bc1d48dff0351fb6084893be7f5a96a8754
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 1%

---

# Campos personalizados do membro do programa {#program-member-custom-fields}

Os campos personalizados Membro do programa permitem coletar dados específicos do programa para cada membro. Eles podem ser usados em: Formulários Marketo, filtros e acionadores da Smart List e ações de fluxo do Smart Campaign. Os dados podem ser visualizados na guia Membros do programa.

>[!NOTE]
>
>Os campos personalizados Membro do programa não têm uma integração com os campos Membro do Salesforce Campaign no momento.

## Criar um campo personalizado de membro do programa {#create-a-program-member-custom-field}

1. No Marketo, clique em **Administrador**.

   ![](assets/one.png)

1. Clique em **Gerenciamento de campos**.

   ![](assets/two.png)

1. Clique em **Novo campo personalizado**.

   ![](assets/three.png)

1. Clique na lista suspensa Objeto e selecione o objeto desejado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Os campos personalizados Pessoa e Membro do Programa não podem compartilhar o mesmo nome.

1. Preencha os campos restantes e clique em **Criar**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Os tipos suportados para campos personalizados Membro do Programa são: booleano, data, datetime, float, inteiro, string, URL. [Saiba mais sobre tipos de campo](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md).

## Descrições do objeto {#object-descriptions}

| Objeto | Descrição |
|---|---|
| Empresa | O nome da empresa associada à pessoa. |
| Oportunidade | Uma oportunidade pode ser associada a uma pessoa ou conta como uma possível venda futura. Normalmente, eles entram no Marketo por meio de um CRM ou por meio de uma API. |
| Pessoa | Um indivíduo no banco de dados do Marketo com o qual você está se relacionando por meio de campanhas de marketing. |
| Membro de programa | Pessoa que também é membro de um programa |

## Triggers e filtros {#triggers-and-filters}

Você pode aproveitar esses dados específicos do programa em listas inteligentes por meio de [acionadores](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md) e/ou [filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md).

![](assets/six.png)

## O que saber {#things-to-know}

* Os campos personalizados Membro do programa estão disponíveis somente em ativos locais. Eles não são suportados no Design Studio porque não há como vinculá-lo a um programa específico.
* Não é possível clonar/mover um formulário (ou uma landing page com um formulário) que contenha campos personalizados do Membro do Programa para o Design Studio.
* O objeto Membro do programa pode ter até 20 campos personalizados. Esses campos estão disponíveis para qualquer programa.
* Ao remover um membro de um programa, se ele tiver dados no campo personalizado Membro do programa, os dados serão depurados desse campo.
* Para exibir os dados, clique na guia Membros no programa e crie uma visualização personalizada que inclua os campos mencionados.
* Importar e exportar via [lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md) e [API](https://developers.marketo.com/) são compatíveis.
* Quando você mescla duas pessoas, os dados do campo personalizado Membro do programa vencedor serão usados. Mas se o vencedor não tiver nenhuma, o valor do perdedor será usado.
* O tipo de alteração é **not** permitido nos campos Informações do Membro do Programa.

>[!MORELIKETHIS]
>
>[Criar um campo personalizado no Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
