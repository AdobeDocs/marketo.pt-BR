---
unique-page-id: 2952636
description: Localizar pessoas duplicadas com lógica personalizada - Documentação do Marketo - Documentação do produto
title: Localizar pessoas duplicadas com lógica personalizada
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 6%

---

# Localizar pessoas duplicadas com lógica personalizada {#find-duplicate-people-with-custom-logic}

O Marketo tem uma lista inteligente do sistema que encontra pessoas duplicadas ao corresponder seus endereços de email. Se quiser usar outro campo para localizar duplicatas, veja como.

>[!PREREQUISITES]
>
>[Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Vá para a **Atividades de marketing** área.

![](assets/ma-2.png)

1. Selecione sua lista inteligente, clique no botão **Lista inteligente** guia.

   ![](assets/two-4.png)

1. Localize e arraste o **Duplicar campos** filtro na tela de desenho.

   ![](assets/three-4.png)

1. Escolha uma das quatro opções disponíveis:

   * Endereço de email
   * Nome completo
   * Sobrenome
   * Atualizado em

   >[!NOTE]
   >
   >Todos os campos, com exceção do Endereço de email, fazem distinção entre maiúsculas e minúsculas. Portanto, usar &quot;john doe&quot; no campo Nome completo _não_ retorna resultados para João da Silva.

   ![](assets/four-2.png)

   Feito! Execute a lista inteligente para encontrar pessoas com o mesmo valor no campo selecionado anteriormente.
