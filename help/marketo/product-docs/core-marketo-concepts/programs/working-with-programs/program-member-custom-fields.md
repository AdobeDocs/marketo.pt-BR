---
unique-page-id: 37355569
description: Campos personalizados de membros do programa - Documentos do Marketing - Documentação do produto
title: Campos personalizados de membro do programa
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Campos personalizados de membros do programa {#program-member-custom-fields}

Campos personalizados de membros do programa permitem coletar dados específicos do programa para cada membro. Eles podem ser usados em: Formulários de marketing, filtros e acionadores de Lista inteligente e ações de fluxo de Campanha inteligente. Os dados podem ser visualizados na guia Membros do programa.

## Criar um campo personalizado de membro do Programa {#create-a-program-member-custom-field}

1. Em Marketo, clique em **Admin**.

   ![](assets/one.png)

1. Clique em **Gerenciamento de campo**.

   ![](assets/two.png)

1. Clique em **Novo campo personalizado**.

   ![](assets/three.png)

1. Clique na lista suspensa Objeto e selecione o objeto desejado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Os campos personalizados de Pessoa e Membro do Programa não podem compartilhar o mesmo nome.

1. Preencha os campos restantes e clique em **Criar**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Os tipos suportados para campos personalizados de membros do Programa são: booleano, data, datetime, float, integer, string, URL. [Saiba mais sobre tipos](http://docs.marketo.com/x/Wwgt) de campos.

## Descrições do objeto {#object-descriptions}

| Objeto | Descrição |
|---|---|
| Empresa | O nome da empresa associada à pessoa. |
| Oportunidade | Uma oportunidade pode ser associada a uma pessoa ou conta como uma possível venda futura. Normalmente, eles entram no Marketing por meio de um CRM ou por API. |
| Pessoa | Um indivíduo em seu banco de dados de marketing com o qual você está se relacionando por meio de campanhas de marketing. |
| Membro programa | Pessoa que também é membro de um programa |

## Acionadores e Filtros {#triggers-and-filters}

Você pode aproveitar esses dados específicos do programa em listas inteligentes por meio de [acionadores](http://docs.marketo.com/x/PoAR)e/ou [filtros](http://docs.marketo.com/x/2YAI).

![](assets/six.png)

## Coisas para saber {#things-to-know}

* Os campos personalizados de membros do programa estão disponíveis somente em ativos locais. Eles não são suportados no Design Studio porque não há como vinculá-los a um programa específico.
* Não é possível clonar/mover um formulário (ou uma landing page com um formulário) que contenha campos personalizados de membros do Programa para o Design Studio.
* Campos personalizados do membro do programa não podem ser usados como tokens.
* O objeto Membro do Programa pode ter até 20 campos personalizados. Esses campos estão disponíveis para qualquer programa.
* Quando você remove um membro de um programa, se ele tiver dados em seu campo personalizado Membro do Programa, os dados serão depurados desse campo.
* Para visualização dos dados, clique na guia Membros no programa e crie uma visualização personalizada que inclua os campos mencionados.
* Importar e exportar por meio de [lista](http://docs.marketo.com/x/egAk)e [API](http://developers.marketo.com/)são suportados.
* Quando duas pessoas forem unidas, os dados de campo personalizado do membro Programa vencedor serão usados. Mas se o vencedor não tiver nenhum, o valor do perdedor será usado.

>[!MORELIKETHIS]
>
>[Criar um campo personalizado no Marketo](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

