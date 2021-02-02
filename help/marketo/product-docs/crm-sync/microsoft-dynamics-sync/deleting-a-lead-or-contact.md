---
unique-page-id: 45417322
description: Exclusão de um cliente potencial ou contato - Documentos de marketing - Documentação do produto
title: Excluindo um Cliente Potencial ou Contato
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Excluindo um Cliente Potencial ou Contato {#deleting-a-lead-or-contact}

Há algumas coisas para saber quando se trata de excluir clientes potenciais/contatos no Microsoft Dynamics.

* O Marketo não exclui automaticamente as pessoas apenas porque os clientes potenciais foram excluídos no Dynamics. Em vez disso, um sinalizador de campo &quot;Microsoft is Deleted&quot; está definido como true. Você pode acionar esse campo para excluir o registro em Marketo, se desejar.

* Ação de fluxo &quot;Excluir Pessoa&quot;: Isso exclui apenas uma pessoa no Marketo (uma opção para excluí-la também no Dynamics não está disponível).

* Se um cliente potencial for excluído no Marketing (mas não no Dynamics) e atualizado no Dynamics depois disso, ele criará uma nova pessoa no Marketo (mesmo endereço de email, ID de nova pessoa).

* Se um cliente potencial for excluído no Dynamics (mas não no Marketing) e, em seguida, for executado pela ação de fluxo &quot;Sincronizar pessoa com a Microsoft&quot;, ele criará um novo cliente potencial no Dynamics.
