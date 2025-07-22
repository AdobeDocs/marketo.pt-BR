---
unique-page-id: 37355569
description: Campos personalizados de membros do programa - Documentação do Marketo - Documentação do produto
title: Campos Personalizados de Membros do Programa
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# Campos Personalizados de Membros do Programa {#program-member-custom-fields}

Os campos personalizados do Membro do Programa permitem coletar dados específicos do programa para cada membro. Eles podem ser usados em: formulários Marketo, filtros e acionadores de Smart List e ações de fluxo do Smart Campaign. Os dados podem ser visualizados na guia Membros do programa.

## Criar um campo personalizado de membro do programa {#create-a-program-member-custom-field}

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Clique em **[!UICONTROL Gerenciamento de campos]**.

   ![](assets/two.png)

1. Clique em **[!UICONTROL Novo Campo Personalizado]**.

   ![](assets/three.png)

1. Clique na lista suspensa **[!UICONTROL Objeto]** e selecione o objeto desejado.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Os campos personalizados [!UICONTROL Pessoa] e [!UICONTROL Membro do Programa] não podem compartilhar o mesmo nome.

1. Preencha os campos restantes e clique em **[!UICONTROL Criar]**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Os tipos com suporte para campos personalizados [!UICONTROL Membro do Programa] são: booleano, data, data e hora, flutuante, inteiro, cadeia de caracteres, URL. [Saiba mais sobre os tipos de campo](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## Descrições de objeto {#object-descriptions}

| Objeto | Descrição |
|---|---|
| Empresa | O nome da empresa associada à pessoa. |
| Oportunidade | Uma oportunidade pode ser associada a uma pessoa ou conta como uma possível venda futura. Normalmente, entram no Marketo por meio de um CRM ou por meio da API. |
| Pessoa | Um indivíduo no banco de dados do Marketo com o qual você está se envolvendo por meio de campanhas de marketing. |
| Membro de programa | Pessoa que também é membro de um programa |

## Acionadores e filtros {#triggers-and-filters}

Você pode aproveitar estes dados específicos do programa em listas inteligentes através de [acionadores](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} e/ou [filtros](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}.

![](assets/six.png)

## O que você deve saber {#things-to-know}

* Os campos personalizados dos membros do programa estão disponíveis somente em ativos locais. Eles não são compatíveis com o Design Studio porque não há como vinculá-los a um programa específico.
* Não é possível clonar/mover um formulário (ou uma página de aterrissagem com um formulário) que contenha campos personalizados de Membro do programa para o Design Studio.
* [Você pode sincronizar](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"} os Campos Personalizados de Membros do Programa com Campos Personalizados de Membros do Campaign.
* O objeto Membro do programa pode ter até 20 campos personalizados. Esses campos estão disponíveis para qualquer programa.
* Ao remover um membro de um programa, se ele tiver dados em seu campo personalizado Membro do programa, os dados serão removidos desse campo.
* Para exibir os dados, clique na guia Membros no programa e crie uma exibição personalizada que inclua esses campos.
* Há suporte para importação e exportação via [lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} e [API](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/home){target="_blank"}. As exportações funcionam somente em listas de Membros do programa, não em listas estáticas.
* Quando você mescla duas pessoas, os dados do campo personalizado do Membro do programa do vencedor são usados. Mas se o vencedor não tiver nenhum, o valor do perdedor será usado.
* O tipo de alteração não é permitido em campos de Informações do membro do programa.
* A restrição &quot;contém&quot; Smart List não é compatível com campos personalizados de Membro do Programa.

>[!MORELIKETHIS]
>
>* [Criar um campo personalizado no Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [Sincronização de Campo Personalizado de Membro do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
