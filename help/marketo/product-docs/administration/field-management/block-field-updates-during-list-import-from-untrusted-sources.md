---
unique-page-id: 2360335
description: Bloqueie a substituição de campos principais durante importações de listas de fontes não confiáveis para proteger dados existentes.
title: Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
TQID: https://experienceleague.adobe.com/cT1pOoWjR-UdHLqNJwhwgR9R12ciIa95q1xHPTf7rBY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 205
ht-degree: 10%

---

# Bloquear atualizações de campo durante a importação de lista de fontes não confiáveis {#block-field-updates-during-list-import-from-untrusted-sources}

Você pode confiar mais nos dados de algumas listas do que de outras. Às vezes, você tem dados questionáveis e quer aceitar os dados se o campo estiver em branco, mas não se houver um valor existente. Você pode fazer isso bloqueando as atualizações de campo em campos principais.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

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

Os campos principais agora estão protegidos contra importações de listas não confiáveis.
