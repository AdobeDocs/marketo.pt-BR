---
unique-page-id: 2360309
description: Noções básicas sobre espaços de trabalho e partições de pessoa - Documentos do Marketo - Documentação do produto
title: Como entender espaços de trabalho e partições de pessoa
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 3%

---

# Como entender espaços de trabalho e partições de pessoa {#understanding-workspaces-and-person-partitions}

## Áreas de trabalho {#workspaces}

>[!CAUTION]
>
>Os espaços de trabalho podem ser complexos para configuração. Contato [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para descobrir se são adequadas para você.

Os espaços de trabalho são áreas separadas no Marketo que contêm ativos de marketing, como programas, páginas de aterrissagem, emails e muito mais. Eles podem ser usados por várias pessoas. Cada usuário tem acesso a um ou mais espaços de trabalho.

>[!NOTE]
>
>**Exemplo**
>
>Alguns motivos para usar um espaço de trabalho:
>
>* Geografia: Os departamentos de marketing da Europa, Ásia e América do Norte recebem cada um um um espaço de trabalho
>* Unidade de negócios: Cada um recebe um espaço de trabalho rápido, Quickbooks e TurboTax
>
>Em cada caso, a separação ocorre porque os ativos de marketing são completamente diferentes. Se eles compartilharem ativos de marketing, os espaços de trabalho podem não ser a ferramenta correta para você.

>[!NOTE]
>
>Saiba como criar [criar um novo espaço de trabalho](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Compartilhamento em espaços de trabalho {#sharing-across-workspaces}

Veja como compartilhar ativos em espaços de trabalho. Funciona da mesma forma para qualquer item que você deseja compartilhar; este exemplo mostra segmentações.

>[!NOTE]
>
>A pasta principal que contém seus ativos é a única pasta que pode ser compartilhada, não as pastas filhas.

1. Crie uma nova pasta.

   ![](assets/one.png)

1. Nomeie a pasta que você vai compartilhar.

   ![](assets/two.png)

1. Mova os ativos que deseja compartilhar na pasta.

   ![](assets/three.png)

1. Clique com o botão direito do mouse na pasta e selecione **Compartilhar pasta**.

   ![](assets/four.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta e clique em **Salvar**. A caixa de diálogo Compartilhar pasta exibirá somente os espaços de trabalho que você tem permissão para visualizar.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >A pasta de origem agora terá uma seta verde, indicando que foi compartilhada. No espaço de trabalho compartilhado, a pasta terá um cadeado, indicando somente leitura.

Você pode compartilhar esses itens em espaços de trabalho.

* Modelos de e-mail
* Modelos de páginas
* Modelos
* Campanhas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentações](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Blocos de conteúdo

## Clonagem em espaços de trabalho {#cloning-across-workspaces}

Para ativos que não são modelos, é melhor cloná-los como ativos locais dentro de um programa.  Com o nível de acesso adequado, você pode arrastar e soltar esses ativos em outro espaço de trabalho:

* Programas
* E-mails
* Páginas
* Formulários

>[!NOTE]
>
>Ao clonar ativos que têm modelos, esses modelos devem ser compartilhados com o espaço de trabalho de destino.

## Mover ativos para outros espaços de trabalho {#moving-assets-to-other-workspaces}

Para mover ativos para um novo espaço de trabalho, coloque-os em uma pasta e arraste a pasta para o outro espaço de trabalho.

>[!NOTE]
>
>Não é possível mover um programa que contenha membros de um espaço de trabalho para outro.

## Partições de pessoas {#person-partitions}

As partições de pessoa atuam como bancos de dados separados. Cada partição tem seu próprio pessoal que não desduplica nem se mistura com outras partições. Se você achar que tem um caso de uso comercial que pode exigir registros duplicados com o mesmo endereço de email, entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

É possível atribuir partições de pessoas a  [espaços de trabalho](create-a-new-workspace.md) nas seguintes configurações:

* um espaço de trabalho para uma partição de pessoa (1:1)
* um espaço de trabalho para várias partições de pessoa (1:x)
* muitos espaços de trabalho para uma partição de pessoa (x:1)

>[!NOTE]
>
>Motivos para usar uma partição de pessoa:
>
>* Seus espaços de trabalho não têm apenas ativos diferentes, mas também não compartilham pessoas
>* Você deseja duplicatas para outros motivos comerciais


>[!CAUTION]
>
>As partições de pessoa não interagem entre si, portanto, tenha cuidado ao configurá-las.

>[!NOTE]
>
>Saiba como [criar uma partição de pessoa](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
