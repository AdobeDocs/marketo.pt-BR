---
unique-page-id: 45417322
description: Exclusão de um cliente em potencial ou contato - Documentação do Marketo - Documentação do produto
title: Excluindo um Cliente Potencial ou Contato
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Excluindo um Cliente Potencial ou Contato {#deleting-a-lead-or-contact}

Há algumas coisas a saber quando se trata de excluir clientes potenciais/contatos em [!DNL Microsoft Dynamics].

* O Marketo não exclui pessoas automaticamente apenas porque os clientes potenciais foram excluídos em [!DNL Dynamics]. Em vez disso, o sinalizador do campo &quot;Microsoft foi excluído&quot; está definido como verdadeiro. É possível acionar esse campo para excluir o registro no Marketo, se desejado.

* Ação de fluxo &quot;Excluir pessoa&quot;: exclui apenas uma pessoa no Marketo (não há uma opção disponível para excluí-la no Dynamics).

* Se um cliente potencial for excluído no Marketo (mas não no [!DNL Dynamics]) e atualizado no [!DNL Dynamics] depois disso, ele criará uma nova pessoa no Marketo (mesmo endereço de email, nova ID de pessoa).

* Se um cliente potencial for excluído no [!DNL Dynamics] (mas não no Marketo) e executado subsequentemente pela ação de fluxo &quot;Sincronizar Pessoa com o Microsoft&quot;, ele criará um novo cliente potencial no [!DNL Dynamics].
