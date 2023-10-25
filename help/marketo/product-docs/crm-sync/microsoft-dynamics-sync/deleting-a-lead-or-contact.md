---
unique-page-id: 45417322
description: Exclusão de um cliente em potencial ou contato - Documentação do Marketo - Documentação do produto
title: Excluindo um Cliente Potencial ou Contato
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Excluindo um Cliente Potencial ou Contato {#deleting-a-lead-or-contact}

Há algumas coisas a saber quando se trata de excluir clientes potenciais/contatos no Microsoft Dynamics.

* O Marketo Engage não exclui pessoas automaticamente apenas porque os clientes em potencial foram excluídos no Dynamics. Em vez disso, o sinalizador do campo &quot;Microsoft foi excluído&quot; está definido como verdadeiro. É possível acionar esse campo para excluir o registro no Marketo, se desejado.

* Ação de fluxo &quot;Excluir pessoa&quot;: exclui apenas uma pessoa no Marketo (não há uma opção disponível para excluí-la no Dynamics).

* Se um cliente potencial for excluído no Marketo (mas não no Dynamics) e atualizado no Dynamics depois disso, ele criará uma nova pessoa no Marketo (mesmo endereço de email, nova ID de pessoa).

* Se um cliente potencial for excluído no Dynamics (mas não no Marketo) e executado subsequentemente pela ação de fluxo &quot;Sincronizar pessoa com o Microsoft&quot;, ele criará um novo cliente potencial no Dynamics.
