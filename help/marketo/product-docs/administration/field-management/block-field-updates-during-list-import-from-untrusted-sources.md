---
unique-page-id: 2360335
description: Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis - Documentos do Marketo - Documentação do produto
title: Bloquear Atualizações de Campo Durante a Importação de Lista de Fontes Não Confiáveis
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Bloquear Atualizações de Campo Durante a Importação de Lista de Fontes Não Confiáveis {#block-field-updates-during-list-import-from-untrusted-sources}

Você pode confiar nos dados em algumas listas mais do que em outras. Às vezes, você pode ter dados questionáveis e desejar utilizá-los se o campo estiver em branco, mas não se houver um valor existente. Você pode fazer isso bloqueando atualizações de campo em campos principais.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Bloqueio de atualizações de campo a partir de fontes não confiáveis {#blocking-field-updates-from-untrusted-sources}

1. Vá para o **Administrador** área.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Clique em **Gerenciamento de campos**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Encontre o campo desejado, selecione-o e, em seguida, em **Ações do campo**, clique em **Bloquear Atualizações de Campo**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Verificar **Importar Lista de Origem Não Confiável** e clique em **Aplicar**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Você pode manter os campos seguros de todas as listas, confiáveis e não confiáveis, verificando também **Origem confiável de Importação de Lista**.

Repita as etapas acima para qualquer outro campo que desejar manter seguro de listas não confiáveis.

## Executando uma Importação de Lista Não Confiável {#running-an-untrusted-list-import}

1. Ao executar a importação da lista, selecione **Não confiável** se quiser que todos os campos configurados na etapa anterior sejam seguros.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Para obter instruções detalhadas sobre importação de listas, consulte [Importar uma lista de pessoas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Bom trabalho! Agora você sabe como manter os campos principais seguros de listas não confiáveis.
