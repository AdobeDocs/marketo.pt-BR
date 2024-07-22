---
unique-page-id: 2952636
description: Localizar pessoas duplicadas com lógica personalizada - Documentação do Marketo - Documentação do produto
title: Localizar pessoas duplicadas com lógica personalizada
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 5%

---

# Localizar pessoas duplicadas com lógica personalizada {#find-duplicate-people-with-custom-logic}

O Marketo Engage tem uma Lista inteligente do sistema que encontra pessoas duplicadas ao corresponder seus endereços de email. Se quiser usar outro campo para localizar duplicatas, veja como.

>[!PREREQUISITES]
>
>[Criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Vá para a área **[!UICONTROL Atividades de marketing]**.

![](assets/ma-2.png)

1. Selecione sua Smart List, clique na guia **[!UICONTROL Smart List]**.

   ![](assets/two-4.png)

1. Localize e arraste o filtro **[!UICONTROL Duplicar Campos]** para a tela.

   ![](assets/three-4.png)

1. Escolha uma das quatro opções disponíveis:

   * Endereço de e-mail
   * Nome completo
   * Sobrenome
   * Atualizado em

   >[!NOTE]
   >
   >Todos os campos, com exceção do Endereço de email, fazem distinção entre maiúsculas e minúsculas. Portanto, o uso de &quot;john doe&quot; no campo Nome Completo _não_ retornaria resultados para John Doe.

   ![](assets/four-2.png)

   Concluído! Execute a Smart List para localizar pessoas com o mesmo valor no campo selecionado anteriormente.
