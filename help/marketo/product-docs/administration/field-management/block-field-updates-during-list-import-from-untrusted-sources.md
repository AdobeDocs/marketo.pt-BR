---
unique-page-id: 2360335
description: Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis - Documentos do Marketo - Documentação do produto
title: Bloquear Atualizações de Campo Durante a Importação de Lista de Fontes Não Confiáveis
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Bloquear atualizações de campo durante importação de lista de fontes não confiáveis {#block-field-updates-during-list-import-from-untrusted-sources}

Você pode confiar nos dados em algumas listas mais do que em outras. Às vezes, você pode ter dados questionáveis e desejar utilizá-los se o campo estiver em branco, mas não se houver um valor existente. Você pode fazer isso bloqueando atualizações de campo em campos principais.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Bloqueio de atualizações de campo a partir de fontes não confiáveis {#blocking-field-updates-from-untrusted-sources}

1. Vá para **Admin** e clique em **Gerenciamento de Campo**.

   ![](assets/image2014-9-19-9-3a38-3a38.png)

1. Localize o campo desejado, selecione-o e, em **Ações do campo**, clique em **Bloquear atualizações de campo**.

   ![](assets/image2014-9-19-9-3a39-3a40.png)

1. Marque **List Import untrusted source** e clique em **Apply**.

   ![](assets/blockupdates.png)

>[!TIP]
>
>Você pode manter os campos seguros de todas as listas, confiáveis e não confiáveis, verificando também **List Import trusted source**.

Repita as etapas acima para qualquer outro campo que desejar manter seguro de listas não confiáveis.

## Executando uma Importação de Lista Não Confiável {#running-an-untrusted-list-import}

1. Ao executar sua importação de lista, selecione **Não confiável** se desejar que todos os campos configurados na etapa anterior sejam seguros.

   ![](assets/importpersondetails.jpg)

Para obter instruções detalhadas sobre como importar listas, consulte [Importar uma Lista de Pessoas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Bom trabalho! Agora você sabe como manter os campos principais seguros de listas não confiáveis.
