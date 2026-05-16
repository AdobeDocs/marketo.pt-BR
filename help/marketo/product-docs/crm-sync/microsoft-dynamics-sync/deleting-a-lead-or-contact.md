---
unique-page-id: 45417322
description: Entenda como a exclusão de clientes potenciais e contatos funciona entre o Microsoft Dynamics e o Marketo. Use o sinalizador O Microsoft foi excluído e a ação Excluir fluxo de pessoa conforme necessário.
title: Excluir um lead ou contato
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/4BwBuLQFJ2pRehuS8EqW-UrEcg5sVeqcstu3azh0NvQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 167
ht-degree: 5%

---

# Excluir um lead ou contato {#deleting-a-lead-or-contact}

Há algumas coisas a saber quando se trata de excluir clientes potenciais/contatos em [!DNL Microsoft Dynamics].

* A Marketo não exclui pessoas automaticamente apenas porque os clientes potenciais foram excluídos em [!DNL Dynamics]. Em vez disso, o sinalizador do campo &quot;Microsoft foi excluído&quot; está definido como verdadeiro. É possível acionar esse campo para excluir o registro no Marketo, se desejado.

* Ação de fluxo &quot;Excluir pessoa&quot;: exclui apenas uma pessoa no Marketo (não há uma opção disponível para excluí-la no Dynamics).

* Se um cliente potencial for excluído no Marketo (mas não no [!DNL Dynamics]) e atualizado no [!DNL Dynamics] depois disso, ele criará uma nova pessoa no Marketo (mesmo endereço de email, nova ID de pessoa).

* Se um cliente potencial for excluído no [!DNL Dynamics] (mas não no Marketo) e executado subsequentemente pela ação de fluxo &quot;Sincronizar Pessoa com o Microsoft&quot;, ele criará um novo cliente potencial no [!DNL Dynamics].
