---
unique-page-id: 2360309
description: Noções básicas sobre espaços de trabalho e partições de pessoas - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre espaços de trabalho e partições de pessoas
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 5%

---

# Noções básicas sobre espaços de trabalho e partições de pessoas {#understanding-workspaces-and-person-partitions}

## Áreas de trabalho {#workspaces}

>[!CAUTION]
>
>Os espaços de trabalho podem ser configurados de forma complexa. Contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para saber se ele é adequado para você.

Os espaços de trabalho são áreas separadas no Marketo que contêm ativos de marketing, como programas, páginas de aterrissagem, emails e muito mais. Elas podem ser usadas por várias pessoas. Cada usuário tem acesso a um ou mais espaços de trabalho.

>[!NOTE]
>
>**Exemplo**
>
>Alguns motivos para usar um espaço de trabalho:
>
>* Geografia: Os departamentos de marketing da Europa, Ásia e América do Norte recebem um espaço de trabalho
>* Unidade de Negócios: [!DNL Quicken], [!DNL Quickbooks] e [!DNL TurboTax] cada uma tem um espaço de trabalho
>
>Em cada caso, a separação ocorre porque os ativos de marketing são completamente diferentes. Se eles compartilharem ativos de marketing, os espaços de trabalho podem não ser a ferramenta certa para você.

>[!NOTE]
>
>Saiba como criar [criar um novo espaço de trabalho](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Compartilhamento entre espaços de trabalho {#sharing-across-workspaces}

Veja como compartilhar ativos entre espaços de trabalho. Funciona da mesma forma para qualquer item que você deseja compartilhar. Este exemplo mostra segmentações.

>[!NOTE]
>
>A pasta principal que contém seus ativos é a única pasta que pode ser compartilhada, não as pastas secundárias.

1. Clique em **[!UICONTROL Banco de Dados]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Clique com o botão direito na pasta Segmentação e clique em **[!UICONTROL Nova pasta]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Nomeie sua pasta e clique em **[!UICONTROL Criar]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Mova o(s) ativo(s) que deseja compartilhar para a pasta.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Clique com o botão direito do mouse na pasta e selecione **[!UICONTROL Compartilhar Pasta]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Selecione o(s) espaço(s) de trabalho com os quais deseja compartilhar a pasta e clique em **[!UICONTROL Salvar]**. A caixa de diálogo Compartilhar pasta exibirá somente os espaços de trabalho que você tem permissão para visualizar.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >A pasta de origem agora terá uma pequena seta verde, indicando que foi compartilhada. No espaço de trabalho compartilhado, a pasta terá um cadeado, indicando somente leitura.

Você pode compartilhar esses itens entre espaços de trabalho.

* Modelos de email
* Modelos de páginas de destino
* Modelos
* Campanhas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentações](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Snippets

## Clonagem entre espaços de trabalho {#cloning-across-workspaces}

Para ativos que não são modelos, é melhor cloná-los como ativos locais dentro de um programa. Com o nível de acesso apropriado, você pode arrastar e soltar esses ativos em outro espaço de trabalho:

* Programas
* Emails
* Páginas de destino
* Formulários

>[!IMPORTANT]
>
>Embora todos os itens listados acima possam ser clonados entre Espaços de Trabalho, emails, formulários e Páginas de Aterrissagem, _devem estar dentro de um programa_ no momento da clonagem.

>[!NOTE]
>
>Ao clonar ativos que têm modelos, esses modelos devem ser compartilhados com o espaço de trabalho de destino.

## Mover o Assets para outros espaços de trabalho {#moving-assets-to-other-workspaces}

Para mover ativos para um novo espaço de trabalho, coloque-os em uma pasta e arraste a pasta para outro espaço de trabalho.

>[!NOTE]
>
>Você não pode mover um programa que contenha membros de um espaço de trabalho para outro.

## Partições de pessoas {#person-partitions}

As partições de pessoas atuam como bancos de dados separados. Cada partição tem seu próprio pessoal que não remove a duplicação nem combina com outras partições. Se você achar que tem um caso de uso comercial que pode exigir registros duplicados com o mesmo endereço de email, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Você pode atribuir partições de pessoas a [espaços de trabalho](create-a-new-workspace.md) nas seguintes configurações:

* um espaço de trabalho para uma partição de pessoa (1:1)
* um espaço de trabalho para muitas partições de pessoas (1:x)
* muitos espaços de trabalho para uma partição de pessoa (x:1)

>[!NOTE]
>
>Motivos para usar uma partição de pessoa:
>
>* Seus espaços de trabalho não só têm ativos diferentes, como também não compartilham pessoas
>* Você deseja duplicações por outros motivos comerciais

>[!CAUTION]
>
>As partições de pessoa não interagem entre si, portanto, tenha cuidado ao configurá-las.

>[!NOTE]
>
>Saiba como [criar uma partição de pessoa](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
