---
unique-page-id: 2952636
description: Encontre pessoas duplicadas com lógica personalizada - Documentos do Marketo - Documentação do produto
title: Localizar Pessoas Duplicadas com Lógica Personalizada
translation-type: tm+mt
source-git-commit: cfefff241b34571b9778cbd827f45d1b468d121e
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Encontrar Pessoas Duplicadas com Lógica Personalizada {#find-duplicate-people-with-custom-logic}

O Marketo tem uma lista inteligente do sistema que encontra pessoas duplicadas ao corresponder seus endereços de email. Se quiser usar outro campo para encontrar duplicatas, veja como.

>[!PREREQUISITES]
>
>[Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Vá para a área **Marketing Activities**.

![](assets/ma-2.png)

1. Selecione sua lista inteligente, clique na guia **Smart List**.

   ![](assets/two-4.png)

1. Localize e arraste o filtro **Duplicar campos** para a tela.

   ![](assets/three-4.png)

1. Escolha uma das quatro opções disponíveis:

   * Endereço de email
   * Nome completo
   * Sobrenome
   * Atualizado em

   >[!NOTE]
   >
   >Todos os campos, com exceção do Endereço de email, fazem distinção entre maiúsculas e minúsculas. Portanto, usar &quot;john doe&quot; no campo Nome completo _not_ retornaria resultados para John Doe.

   ![](assets/four-2.png)

   Concluído! Execute a lista inteligente para localizar pessoas com o mesmo valor no campo selecionado anteriormente.
