---
unique-page-id: 45417322
description: Exclusão de um lead ou contato - Documentos da Marketo - Documentação do produto
title: Excluindo um Lead ou Contato
exl-id: d561b424-6a2b-4abe-b9bd-81eb23f1a25b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Excluindo um Lead ou Contato {#deleting-a-lead-or-contact}

Há algumas coisas a saber quando se trata de excluir leads/contatos no Microsoft Dynamics.

* O Marketo não exclui automaticamente pessoas apenas porque os leads foram excluídos no Dynamics. Em vez disso, um sinalizador de campo &quot;Microsoft é Excluído&quot; é definido como true. Você pode acionar esse campo para excluir o registro no Marketo, se desejar.

* Ação do fluxo &quot;Excluir pessoa&quot;: Isso exclui apenas uma pessoa no Marketo (uma opção para também excluí-la no Dynamics não está disponível).

* Se um lead for excluído no Marketo (mas não no Dynamics) e for atualizado no Dynamics depois disso, ele criará uma nova pessoa no Marketo (mesmo endereço de email, ID de nova pessoa).

* Se um lead for excluído no Dynamics (mas não no Marketo) e, em seguida, for executado pela ação de fluxo &quot;Sincronizar pessoa para Microsoft&quot;, ele criará um novo lead no Dynamics.
