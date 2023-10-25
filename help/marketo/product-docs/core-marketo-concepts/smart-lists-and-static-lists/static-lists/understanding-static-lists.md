---
unique-page-id: 2949891
description: Noções básicas sobre listas estáticas - Documentação do Marketo - Documentação do produto
title: Compreensão de listas estáticas
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 2%

---

# Compreensão de listas estáticas {#understanding-static-lists}

As listas estáticas são um dos recursos mais simples e úteis do Marketo. Eles são simplesmente uma lista de nomes do seu banco de dados. Você encontrará muitas razões para usá-los.

>[!NOTE]
>
>Uma única pessoa no banco de dados pode estar em muitas listas estáticas diferentes.

A diferença entre uma Lista estática e uma Lista inteligente é essencial para compreender.

| Tipo | Lógica |
|---|---|
| Lista inteligente | Baseado em **regras definidas** |
| Lista estática | Baseado em **adicionar/remover cada pessoa** |

>[!CAUTION]
>
>Um dos erros mais comuns é pensar que você pode remover uma pessoa de uma lista simplesmente &quot;excluindo a pessoa&quot;. **Isso está errado**. Excluir a pessoa fará com que ela seja excluída de **todo o banco de dados** Não apenas a lista.

## Maneiras de adicionar/remover pessoas de uma lista {#ways-to-add-remove-people-from-a-list}

1. Etapa do fluxo do Campaign inteligente ([Adicionar à lista](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Remove from List](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Etapa de fluxo de ação única](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Arrastar pessoas para uma lista na árvore
1. [Importação de lista](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Alguns usos de uma lista estática {#some-uses-of-a-static-list}

* Uma lista que foi pré-selecionada para receber uma mensagem de marketing.
* Uma lista de &quot;concorrentes&quot; usada para enviar mensagens de contrainteligência travessas.
* Uma lista temporária de pessoas em um estado específico, que são removidas pelas Campanhas inteligentes quando saem desse estado.

Aproveite o poder da LISTA!

>[!MORELIKETHIS]
>
>[Criar uma lista estática](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
