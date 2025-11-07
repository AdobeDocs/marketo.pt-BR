---
solution: Marketo Engage
product: marketo
title: Conteúdo condicional
description: Use o conteúdo condicional nos seus emails para exibir dinamicamente o conteúdo, dependendo do recipient.
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 6b9f6d4b276115e1f3f3dac73eb64e5358a76516
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Conteúdo condicional {#conditional-content}

O conteúdo condicional permite controlar dinamicamente o conteúdo que é visto por cada público-alvo. Use as Segmentações existentes para determinar o que um recipient vê com base em critérios predefinidos.

>[!PREREQUISITES]
>
>Ter pelo menos uma Segmentação [criada](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) e [aprovada](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md).

## Adicionar conteúdo condicional {#add-conditional-content}

1. Abra o email desejado e clique em **Editar conteúdo do email**.

   ![](assets/conditional-content-1.png)

1. Selecione o conteúdo que deseja que seja condicional (neste exemplo, estamos escolhendo a imagem do cabeçalho). Clique no ícone _Habilitar conteúdo condicional_.

   ![](assets/conditional-content-2.png)

1. A caixa de destaque fica laranja. À esquerda, clique no ícone _Selecionar condição_ (![](assets/icon-select-condition.png)) para definir sua variante.

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. Escolha o segmento desejado e clique em **Selecionar**.

   ![](assets/conditional-content-4.png)

1. Clique no ícone _Editar imagem_ para substituir a imagem existente da variante. Escolha a fonte da nova imagem. Neste exemplo, estamos escolhendo a biblioteca _Imagens e Arquivos_ na nossa assinatura do Marketo Engage.

   ![](assets/conditional-content-5.png)

1. Escolha a imagem aplicável e clique em **Selecionar**.

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. A nova imagem é exibida. É recomendável renomear a variante para facilitar a identificação. Basta clicar nas reticências e selecionar **Renomear**.

   >[!NOTE]
   >
   >Clicar nas reticências também permite visualizar a condição definida da variante, bem como duplicá-la. Se você tiver mais de uma variante, uma opção de exclusão ficará disponível. Se você tiver apenas uma variante, a maneira de excluí-la é simplesmente clicar novamente no ícone _Habilitar conteúdo condicional_ (agora ele dirá _Desabilitar conteúdo condicional_ quando você passar o mouse sobre ela).

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. Para adicionar outras variantes (opcional), clique em **Adicionar variante** e siga as mesmas etapas.

   ![](assets/conditional-content-8.png)

1. Quando terminar, cada variante exibirá o conteúdo selecionado.

   ![](assets/conditional-content-9.gif)

1. Os recipients visualizam o conteúdo com base nas regras definidas em cada segmento. No exemplo acima, todos que tiverem &quot;futebol&quot; listado no seu campo do Marketo Engage _Esporte favorito_ verão a imagem do futebol.

>[!MORELIKETHIS]
>
>* [Definir Regras de Segmento](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Criar um campo personalizado no Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
