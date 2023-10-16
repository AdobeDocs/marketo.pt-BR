---
unique-page-id: 37355569
description: Campos personalizados de membros do programa - Documentação do Marketo - Documentação do produto
title: Campos Personalizados de Membros do Programa
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 1%

---

# Campos Personalizados de Membros do Programa {#program-member-custom-fields}

Os campos personalizados do Membro do Programa permitem coletar dados específicos do programa para cada membro. Eles podem ser usados em: formulários Marketo, filtros e acionadores de Smart List e ações de fluxo do Smart Campaign. Os dados podem ser visualizados na guia Membros do programa.

## Criar um campo personalizado de membro do programa {#create-a-program-member-custom-field}

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Clique em **[!UICONTROL Gerenciamento de campo]**.

   ![](assets/two.png)

1. Clique em **[!UICONTROL Novo campo personalizado]**.

   ![](assets/three.png)

1. Clique na lista suspensa Objeto e selecione o objeto desejado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Campos personalizados de Pessoa e Membro do Programa não podem compartilhar o mesmo nome.

1. Preencha os campos restantes e clique em **[!UICONTROL Criar]**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Os tipos suportados para campos personalizados de Membro do programa são: booleano, data, data e hora, flutuação, número inteiro, sequência, URL. [Saiba mais sobre tipos de campo](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## Descrições de objeto {#object-descriptions}

| Objeto | Descrição |
|---|---|
| Empresa | O nome da empresa associada à pessoa. |
| Oportunidade | Uma oportunidade pode ser associada a uma pessoa ou conta como uma possível venda futura. Normalmente, entram no Marketo por meio de um CRM ou por meio da API. |
| Pessoa do  | Um indivíduo no banco de dados do Marketo com o qual você está se envolvendo por meio de campanhas de marketing. |
| Membro de programa | Pessoa que também é membro de um programa |

## Acionadores e filtros {#triggers-and-filters}

Você pode aproveitar esses dados específicos do programa em listas inteligentes via [acionadores](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} and/or [filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}.

![](assets/six.png)

## O que você deve saber {#things-to-know}

* Os campos personalizados dos membros do programa estão disponíveis somente em ativos locais. Eles não são compatíveis com o Design Studio porque não há como vinculá-los a um programa específico.
* Não é possível clonar/mover um formulário (ou uma página de aterrissagem com um formulário) que contenha campos personalizados de Membro do programa para o Design Studio.
* [Você pode sincronizar](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"} os Campos personalizados do membro do programa com Campos personalizados do membro da campanha.
* O objeto Membro do programa pode ter até 20 campos personalizados. Esses campos estão disponíveis para qualquer programa.
* Ao remover um membro de um programa, se ele tiver dados em seu campo personalizado Membro do programa, os dados serão removidos desse campo.
* Para exibir os dados, clique na guia Membros no programa e crie uma exibição personalizada que inclua esses campos.
* Importar e exportar via [lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} and [API](https://developers.marketo.com/){target="_blank"} são compatíveis. As exportações funcionam somente em listas de Membros do programa, não em listas estáticas.
* Quando você mescla duas pessoas, os dados do campo personalizado do Membro do programa do vencedor são usados. Mas se o vencedor não tiver nenhum, o valor do perdedor será usado.
* O tipo de alteração não é permitido em campos de Informações do membro do programa.
* A restrição &quot;contém&quot; Smart List não é compatível com campos personalizados de Membro do Programa.

>[!MORELIKETHIS]
>
>* [Criar um campo personalizado no Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [Sincronização de Campo Personalizado de Membro do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
