---
unique-page-id: 1900585
description: Adicionar seções editáveis aos modelos de email v1.0 - Documentos do Marketo - Documentação do produto
title: Adicionar seções editáveis aos modelos de email v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 2%

---

# Adicionar seções editáveis aos modelos de email v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se você estiver criando um modelo no Editor de modelo de email v1.0, poderá tornar qualquer seção editável colocando um `<div>` à sua volta.

>[!NOTE]
>
>**Exemplo**
>
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regras:

1. O HTML deve ser sempre válido.
1. A classe de **mktEditable** deve ser incluído.
1. A ID deve ser exclusiva nesse HTML.
1. Não há espaços na ID.

>[!CAUTION]
>
>As instruções mktEditable não podem ser aninhadas.

Se quiser saber como fazer isso no Editor de modelo de email v2.0, confira [sintaxe do modelo de email](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md).
