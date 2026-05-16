---
unique-page-id: 2949891
description: Saiba mais sobre listas estáticas no Marketo para conjuntos fixos de pessoas. Use listas estáticas quando a associação for gerenciada manualmente.
title: Noções básicas sobre listas estáticas
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
TQID: https://experienceleague.adobe.com/rRi3-6ZggKswYYLTZjUr5EBDNoMRirDc1KJgHbbDqP4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 5%

---

# Noções básicas sobre listas estáticas {#understanding-static-lists}

As listas estáticas são um dos recursos mais simples e úteis do Marketo. Eles são uma lista de nomes do seu banco de dados. Você encontrará muitas razões para usá-los.

>[!NOTE]
>
>Uma única pessoa no banco de dados pode estar em muitas listas estáticas diferentes.

A diferença entre uma Lista estática e uma Lista inteligente é essencial para compreender.

| Tipo | Lógica |
|---|---|
| Lista inteligente | Com base em **regras definidas** |
| Lista estática | Com base em **adicionar/remover cada pessoa** |

>[!CAUTION]
>
>Um dos erros mais comuns é pensar que você pode remover uma pessoa de uma lista &quot;excluindo a pessoa&quot;. **Isso está errado**. Excluir a pessoa irá excluí-la de **todo o banco de dados**, não apenas da lista.

## Maneiras de adicionar ou remover pessoas de uma lista {#ways-to-add-remove-people-from-a-list}

1. Etapa de fluxo do Campaign inteligente ([Adicionar à Lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Remover da Lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Etapa de fluxo de ação única](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Arrastar pessoas para uma lista na árvore
1. [Importação de lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Alguns usos de uma lista estática {#some-uses-of-a-static-list}

* Uma lista que foi pré-selecionada para receber uma mensagem de marketing.
* Uma lista de &quot;concorrentes&quot; usada para enviar mensagens de contrainteligência travessas.
* Uma lista temporária de pessoas em um estado específico, que são removidas pelas Campanhas inteligentes quando saem desse estado.

>[!MORELIKETHIS]
>
>[Criar uma Lista Estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
