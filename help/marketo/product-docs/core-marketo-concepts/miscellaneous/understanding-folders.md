---
unique-page-id: 4720779
description: Saiba mais sobre pastas dentro de programas para organizar Campanhas inteligentes e ativos. Criar, renomear e excluir pastas.
title: Noções básicas sobre pastas
exl-id: 2ea914f6-ca64-4e87-806c-93beba075ab2
TQID: https://experienceleague.adobe.com/wAE129LK3Pk-CB5SSQqqSV50ng085soYsm4JHfh0CuI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: b77e1a1e72b89e7cdef5733dbb2de4405ebf3b07
workflow-type: tm+mt
source-wordcount: 427
ht-degree: 1%

---

# Noções básicas sobre pastas {#understanding-folders}

As pastas em um programa podem ser usadas para organizar suas campanhas e ativos inteligentes. Estas são diferentes de [pastas de campanha](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.md).

## Criar uma pasta {#create-a-folder}

1. Acesse a área **[!UICONTROL Atividades de marketing]**.

   ![](assets/ma.png)

1. Clique com o botão direito em um programa e selecione **[!UICONTROL Nova pasta]**.

   ![](assets/image2015-4-20-18-3a45-3a14.png){width="600" zoomable="yes"}

1. Nomeie a nova pasta e pressione **[!UICONTROL Enter]**.

   ![](assets/image2015-4-20-18-3a46-3a57.png){width="600" zoomable="yes"}

A nova pasta agora está pronta para seus ativos locais.

## Renomear uma pasta {#rename-a-folder}

1. Clique com o botão direito do mouse na pasta e selecione **[!UICONTROL Renomear Pasta]**.

   ![](assets/image2015-4-20-18-3a49-3a10.png){width="600" zoomable="yes"}

1. Digite um novo nome e pressione **[!UICONTROL Enter]**.

   ![](assets/image2015-4-20-18-3a52-3a30.png){width="600" zoomable="yes"}

## Excluir uma pasta {#delete-a-folder}

>[!NOTE]
>
>Verifique se a pasta está vazia antes de excluí-la.

1. Clique com o botão direito do mouse na pasta e selecione **[!UICONTROL Excluir Pasta]**.

   ![](assets/image2015-4-20-18-3a55-3a51.png){width="600" zoomable="yes"}

## Arquivar uma pasta {#archive-a-folder}

No Marketo, você pode converter pastas existentes em pastas de arquivo. As pastas de arquivo existem em [!UICONTROL Atividades de marketing], [!UICONTROL Banco de dados] e [!UICONTROL Design Studio].

![](assets/image2015-4-20-19-3a3-3a46.png){width="600" zoomable="yes"}

Ao arquivar uma pasta:

* A pasta e os ativos não estão mais visíveis nos resultados da pesquisa. Se você pesquisar um Programa ou Evento que esteja dentro de uma pasta arquivada, os resultados retornarão uma exibição recolhida da pasta arquivada
* Os ativos na pasta não aparecem mais na sugestão automática
* Modelos arquivados não estão disponíveis ao criar um email ou uma landing page no Design Studio
* Páginas arquivadas não podem ser usadas em grupos de teste de landing page

Funcionalidade que **não** será alterada durante o arquivamento:

* A pesquisa global ainda encontra resultados em pastas arquivadas
* Você pode usar um filtro para selecionar ativos arquivados para uso em relatórios

### Desativar campanhas no arquivo {#disable-campaigns-archive}

Quando uma pasta ou programa é arquivado ou uma Campanha inteligente ativa é movida para uma pasta que já está arquivada, o Marketo Engage impede a execução das campanhas afetadas:

* **Campanhas acionadas** estão desativadas.
* **Campanhas em lote** têm suas execuções pendentes canceladas.
* **Campanhas executáveis** não têm estado de execução, portanto, nenhuma ação foi tomada.

**Ações com suporte**

As seguintes ações desativam campanhas:

* Arrastando e soltando uma **pasta** contendo campanhas ativas em uma pasta arquivada
* Arrastando e soltando um **programa** (qualquer tipo) contendo campanhas ativas em uma pasta arquivada
* Arrastando e soltando uma **única Campanha Inteligente** em uma pasta arquivada
* Clicar com o botão direito do mouse em **Mover** de uma única Campanha Inteligente para uma pasta arquivada
* Clicando com o botão direito do mouse em **Mover Pasta** em uma pasta que contém campanhas ativas para uma pasta arquivada
* Clicar com o botão direito do mouse em **Mover** em um programa que contém campanhas ativas para uma pasta arquivada
* Clicar com o botão direito do mouse em **Converter em Pasta Arquivada** em uma pasta para arquivá-la no local sem movê-la

>[!NOTE]
>
>Se uma Campanha inteligente dentro da pasta ou do programa que está sendo arquivado for referenciada em outro lugar (por exemplo, por meio de uma etapa de fluxo &quot;Solicitar campanha&quot;), o arquivamento será bloqueado para evitar a interrupção dessa outra campanha.
