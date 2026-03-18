---
unique-page-id: 1900585
description: Saiba como adicionar seções editáveis a modelos de email na v1.0. Permitir que os usuários editem áreas específicas, mantendo o restante bloqueado.
title: Adicionar seções editáveis a modelos de email v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 14%

---

# Adicionar seções editáveis a modelos de email v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se você estiver criando um modelo no Editor de modelo de email v1.0, poderá tornar qualquer seção editável colocando um `<div>` especial ao redor dela.

>[!NOTE]
>
>**Exemplo**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regras:

1. O HTML sempre deve ser válido.
1. A classe de **mktEditable** deve ser incluída.
1. A ID deve ser exclusiva nessa HTML.
1. Nenhum espaço na ID.

>[!CAUTION]
>
>instruções mktEditable não podem ser aninhadas.

Se quiser saber como fazer isso no Editor de modelo de email v2.0, confira a [sintaxe do modelo de email](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
