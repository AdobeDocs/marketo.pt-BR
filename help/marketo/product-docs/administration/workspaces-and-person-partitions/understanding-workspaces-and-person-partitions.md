---
unique-page-id: 2360309
description: Saiba como os espaços de trabalho organizam ativos de marketing e como as partições de pessoas atuam como bancos de dados separados.
title: Noções básicas dos espaços de trabalho e partições de pessoas
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
TQID: 'https://experienceleague.adobe.com/Ex-WBSNYTFvevcwryuO4CzUsg79nOmjkVx4WMUx9nqA'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: b4e49ca2-9149-5443-90e6-11978bb87c2f
    internal-label: Partitions
  - id: fffc2f21-ba05-5d98-924c-16da987a5b69
    internal-label: Workspaces
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 76%
---
# Noções básicas dos espaços de trabalho e partições de pessoas {#understanding-workspaces-and-person-partitions}

## Áreas de trabalho {#workspaces}

>[!CAUTION]
>
>Os espaços de trabalho podem ser complexos de configurar. Contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para descobrir se eles são adequados para você.

Os espaços de trabalho são áreas separadas no Marketo que contêm ativos de marketing, como programas, páginas de destino, emails e muito mais. Eles podem ser usados por várias pessoas. Cada usuário tem acesso a um ou mais espaços de trabalho.

>[!NOTE]
>
>**Exemplo**
>
>Alguns motivos para querer usar um espaço de trabalho:
>
>* Geografia: os departamentos de marketing da Europa, Ásia e América do Norte recebem um espaço de trabalho cada
>* Unidade de negócios: [!DNL Quicken], [!DNL Quickbooks] e [!DNL TurboTax] recebem um espaço de trabalho cada
>
>Em cada caso, a separação ocorre porque os ativos de marketing são completamente diferentes. Caso eles compartilhem ativos de marketing, os espaços de trabalho podem não ser a ferramenta certa para você.

>[!NOTE]
>
>Saiba como [criar um novo espaço de trabalho](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Compartilhamento entre espaços de trabalho {#sharing-across-workspaces}

As etapas a seguir explicam como compartilhar ativos entre espaços de trabalho. Funciona da mesma forma para qualquer item que você queira compartilhar. Este exemplo mostra segmentações.

>[!NOTE]
>
>A pasta principal que contém os seus ativos é a única pasta que pode ser compartilhada, não as pastas secundárias.

1. Clique em **[!UICONTROL Banco de dados]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Clique com o botão direito do mouse na pasta “Segmentação” e selecione **[!UICONTROL Nova pasta]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Nomeie a pasta e clique em **[!UICONTROL Criar]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Mova os ativos que deseja compartilhar para a pasta.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Clique com o botão direito do mouse na pasta e selecione **[!UICONTROL Compartilhar pasta]**.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Selecione os espaços de trabalho com os quais deseja compartilhar a pasta e clique em **[!UICONTROL Salvar]**. A caixa de diálogo “Compartilhar pasta” exibirá somente os espaços de trabalho que você tem permissão para visualizar.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >A pasta de origem agora terá uma pequena seta verde, indicando que foi compartilhada. No espaço de trabalho compartilhado, a pasta mostrará um cadeado, indicando que é somente de leitura.

Você pode compartilhar esses itens entre espaços de trabalho.

* Modelos de email
* Modelos de páginas de destino
* Modelos
* Campanhas inteligentes
* [Listas inteligentes](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentações](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Trechos

## Clonagem entre espaços de trabalho {#cloning-across-workspaces}

Para ativos que não são modelos, é recomendável cloná-los como ativos locais dentro de um programa. Com o nível de acesso apropriado, você pode arrastar e soltar esses ativos em outro espaço de trabalho:

* Programas
* Emails
* Páginas de destino
* Formulários

>[!IMPORTANT]
>
>Embora todos os itens listados acima possam ser clonados entre espaços de trabalho, emails, formulários e páginas de destino _precisam estar dentro de um programa_ no momento da clonagem.

>[!NOTE]
>
>Ao clonar ativos que possuem modelos, esses modelos precisam ser compartilhados com o espaço de trabalho de destino.

## Mover ativos para outros espaços de trabalho {#moving-assets-to-other-workspaces}

Para mover ativos para um novo espaço de trabalho, coloque-os em uma pasta e arraste-a para outro espaço de trabalho.

>[!NOTE]
>
>Um programa que contém membros não pode ser movido de um espaço de trabalho para outro.

## Partições de pessoas {#person-partitions}

As partições de pessoas atuam como bancos de dados separados. Cada partição tem suas próprias pessoas, que não são desduplicadas nem combinadas com outras partições. Se o caso de uso comercial exigir registros duplicados com o mesmo endereço de email, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

Você pode atribuir partições de pessoas a [espaços de trabalho](create-a-new-workspace.md) nas seguintes configurações:

* um espaço de trabalho para uma partição de pessoa (1:1)
* um espaço de trabalho para muitas partições de pessoas (1:x)
* muitos espaços de trabalho para uma partição de pessoa (x:1)

>[!NOTE]
>
>Motivos para usar uma partição de pessoa:
>
>* Seus espaços de trabalho não só têm ativos diferentes, como também não compartilham pessoas
>* Você quer fazer duplicações por outros motivos comerciais

>[!CAUTION]
>
>As partições de pessoas não interagem entre si, portanto, tenha cuidado ao configurá-las.

>[!NOTE]
>
>Saiba como [criar uma partição de pessoa](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
