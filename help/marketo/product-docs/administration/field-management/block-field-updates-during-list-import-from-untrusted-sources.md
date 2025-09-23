---
unique-page-id: 2360335
description: Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis - Documentação do Marketo - Documentação do produto
title: Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 9%

---

# Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis {#block-field-updates-during-list-import-from-untrusted-sources}

Você pode confiar mais nos dados de algumas listas do que de outras. Às vezes, você tem dados questionáveis e quer usá-los se o campo estiver em branco, mas não se houver um valor existente. Você pode fazer isso bloqueando as atualizações de campo em campos principais.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Bloqueando Atualizações De Campo De Origens Não Confiáveis {#blocking-field-updates-from-untrusted-sources}

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Clique em **[!UICONTROL Gerenciamento de campos]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Localize o campo desejado, selecione-o e, em **[!UICONTROL Ações do Campo]**, clique em **[!UICONTROL Bloquear Atualizações do Campo]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Marque **[!UICONTROL Origem não confiável de Importação de Lista]** e clique em **[!UICONTROL Aplicar]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Você pode manter os campos protegidos de todas as listas, confiáveis e não confiáveis, verificando também a **[!UICONTROL fonte confiável de Importação de Lista]**.

Repita as etapas acima para quaisquer outros campos que você queira manter a salvo de listas não confiáveis.

## Executando uma Importação de Lista Não Confiável {#running-an-untrusted-list-import}

1. Ao executar a importação da lista, selecione **[!UICONTROL Não confiável]** se quiser que todos os campos configurados na etapa anterior sejam seguros.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Para obter instruções detalhadas sobre como importar listas, consulte [Importar uma Lista de Pessoas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Bom trabalho! Agora você sabe como manter os campos principais protegidos contra listas não confiáveis.
