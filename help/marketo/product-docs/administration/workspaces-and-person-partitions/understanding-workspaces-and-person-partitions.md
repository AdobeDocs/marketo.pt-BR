---
unique-page-id: 2360309
description: Saiba como os espaços de trabalho organizam ativos de marketing e como as partições de pessoas atuam como bancos de dados separados.
title: Noções Básicas sobre Espaços de Trabalho e Partições de Pessoas
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
TQID: https://experienceleague.adobe.com/Ex-WBSNYTFvevcwryuO4CzUsg79nOmjkVx4WMUx9nqA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: d0251300-e25f-466f-9856-7e11ce8fa7aa
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 551
ht-degree: 0%

---

# Noções Básicas sobre Espaços de Trabalho e Partições de Pessoas {#understanding-workspaces-and-person-partitions}

## Espaços de trabalho {#workspaces}

>[!CAUTION]
>
>Os espaços de trabalho podem ser configurados de forma complexa. Contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para descobrir se eles são adequados para você.

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
>Saiba como [criar um novo espaço de trabalho](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Compartilhamento entre espaços de trabalho {#sharing-across-workspaces}

As etapas a seguir explicam como compartilhar ativos entre espaços de trabalho. Funciona da mesma forma para qualquer item que você deseja compartilhar. Este exemplo mostra segmentações.

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
* Modelos de página de destino
* Modelos
* Campanhas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentações](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Trechos

## Clonagem entre espaços de trabalho {#cloning-across-workspaces}

Para ativos que não são modelos, é recomendável cloná-los como ativos locais dentro de um programa. Com o nível de acesso apropriado, você pode arrastar e soltar esses ativos em outro espaço de trabalho:

* Programas
* Emails
* Landing Pages
* Forms

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
>Um programa que contém membros não pode ser movido de um espaço de trabalho para outro.

## Partições de pessoas {#person-partitions}

As partições de pessoas atuam como bancos de dados separados. Cada partição tem seu próprio pessoal que não remove a duplicação nem combina com outras partições. Se o caso de uso comercial exigir registros duplicados com o mesmo endereço de email, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

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
