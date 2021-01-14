---
unique-page-id: 2360335
description: Bloquear atualizações de campo durante importação de Lista de fontes não confiáveis - Documentos do Marketing - Documentação do produto
title: Bloquear atualizações de campo durante importação de Lista de fontes não confiáveis
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Bloquear atualizações de campo durante importação de Lista de fontes não confiáveis {#block-field-updates-during-list-import-from-untrusted-sources}

Você pode confiar nos dados em algumas listas mais do que em outras. Às vezes, você tem dados questionáveis e deseja utilizá-los se o campo estiver em branco, mas não se houver um valor existente. É possível fazer isso bloqueando atualizações de campo em campos chave.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Bloquear atualizações de campo de fontes não confiáveis {#blocking-field-updates-from-untrusted-sources}

1. Vá para **Admin** e clique em **Gerenciamento de campo**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Localize o campo desejado, selecione-o e, em **Ações de campo**, clique em **Bloquear atualizações de campo**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Marque **Importação de Lista de fonte não confiável** e clique em **Aplicar**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Você pode manter os campos seguros de todas as listas, confiáveis e não confiáveis, verificando também **Origem confiável de Importação de Lista**.

Repita as etapas acima para quaisquer outros campos que você deseja manter seguros contra listas não confiáveis.

## Execução de uma Importação de Lista Não Confiável {#running-an-untrusted-list-import}

1. Ao executar a importação de lista, selecione **Não confiável** se quiser que todos os campos configurados na etapa anterior sejam seguros.

   ![](assets/importpersondetails.jpg)

Para obter instruções detalhadas sobre como importar listas, consulte [Importar uma Lista de Pessoas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Bom trabalho! Agora você sabe como manter os campos chave seguros contra listas não confiáveis.
