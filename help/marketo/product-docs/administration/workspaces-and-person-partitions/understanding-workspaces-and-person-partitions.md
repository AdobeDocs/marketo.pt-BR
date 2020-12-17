---
unique-page-id: 2360309
description: Noções básicas sobre espaços de trabalho e partições pessoais - Documentos do Marketing - Documentação do produto
title: Como entender espaços de trabalho e partições de pessoas
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---


# Noções Gerais de Espaços de Trabalho e Partições de Pessoa {#understanding-workspaces-and-person-partitions}

## Espaços de trabalho {#workspaces}

>[!CAUTION]
>
>Os espaços de trabalho podem ser complexos de configuração.  Entre em contato com o [Suporte do Marketing](http://support.marketo.com/) para descobrir se eles são adequados para você.

Os espaços de trabalho são áreas separadas no Marketing que contêm ativos de marketing, como programas, landings page, e-mails e muito mais. Eles podem ser usados por várias pessoas. Cada usuário tem acesso a um ou mais espaços de trabalho.

>[!NOTE]
>
>**Exemplo**
>
>Alguns motivos para usar um espaço de trabalho:
>
>* Geografia: Os departamentos de marketing da Europa, Ásia e América do Norte recebem cada um um espaço de trabalho
>* Unidade de negócio: Cada um recebe um espaço de trabalho rápido, Quickbooks e TurboTax

>
>
Em cada caso, a separação ocorre porque os ativos de marketing são completamente diferentes. Se compartilharem ativos de marketing, os espaços de trabalho podem não ser a ferramenta certa para você.

>[!NOTE]
>
>**Mergulho profundo**
>
>Saiba como criar [um novo espaço de trabalho](create-a-new-workspace.md).

## Compartilhamento entre espaços de trabalho {#sharing-across-workspaces}

Veja como compartilhar ativos entre áreas de trabalho. Funciona da mesma forma para qualquer coisa que você queira compartilhar. este exemplo mostra segmentações.

>[!NOTE]
>
>A pasta pai que contém seus ativos é a única pasta que pode ser compartilhada, não as pastas filhas.

1. Crie uma nova pasta.

   ![](assets/one.png)

1. Nomeie a pasta que você vai compartilhar.

   ![](assets/two.png)

1. Mova os ativos que deseja compartilhar para a pasta.

   ![](assets/three.png)

1. Clique com o botão direito do mouse na pasta e selecione **Compartilhar pasta**.

   ![](assets/four.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta e clique em **Salvar**. A caixa de diálogo Compartilhar pasta exibirá apenas espaços de trabalho com permissão para visualização.

   ![](assets/image2015-5-27-11-3a6-3a40.png)

   >[!NOTE]
   >
   >A pasta de origem agora terá uma seta verde, indicando que foi compartilhada. No espaço de trabalho compartilhado, a pasta terá um cadeado, indicando somente leitura.

Você pode compartilhar esses itens em áreas de trabalho.

* Modelos de e-mail
* Modelos de landing page
* Modelos
* Campanhas inteligentes
* [Listas inteligentes](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentações](share-segmentations-across-workspaces-and-partitions.md)
* Trechos

## Clonagem entre espaços de trabalho {#cloning-across-workspaces}

Para ativos que não são modelos, é melhor cloná-los como ativos locais dentro de um programa.  Com o nível de acesso adequado, você pode arrastar e soltar esses ativos em outro espaço de trabalho:

* Programas
* Emails
* landings page
* Forms

>[!NOTE]
>
>Ao clonar ativos que têm modelos, esses modelos devem ser compartilhados com a área de trabalho de destino.

## Mover ativos para outros espaços de trabalho {#moving-assets-to-other-workspaces}

Para mover ativos para um novo espaço de trabalho, coloque-os em uma pasta e arraste a pasta para o outro espaço de trabalho.

>[!NOTE]
>
>Não é possível mover um programa que contenha membros de um espaço de trabalho para outro.

## Partições de Pessoas {#person-partitions}

As partições de pessoa atuam como bancos de dados separados. Cada partição tem seu próprio povo que não desduplica nem se mistura com outras partições. Se achar que você tem um caso de uso comercial que pode exigir a existência de registros de duplicados com o mesmo endereço de email, entre em contato com o [Suporte do Marketing](http://support.marketo.com).

Você pode atribuir partições de pessoa a [espaços de trabalho](create-a-new-workspace.md) nas seguintes configurações:

* um espaço de trabalho para uma partição de pessoa (1:1)
* um espaço de trabalho para muitas partições de pessoa (1:x)
* muitos espaços de trabalho para uma partição de pessoa (x:1)

>[!NOTE]
>
>**Exemplo**
>
>Motivos para usar uma partição de pessoa:
>
>* Seus espaços de trabalho não têm apenas ativos diferentes, mas também não compartilham pessoas
>* Você quer duplicados por outros motivos comerciais

>



>[!CAUTION]
>
>As partições pessoais não interagem entre si, portanto, tenha cuidado ao configurá-las.

>[!NOTE]
>
>**Mergulho profundo**
>
> Saiba como [criar uma partição de pessoa](create-a-person-partition.md).

