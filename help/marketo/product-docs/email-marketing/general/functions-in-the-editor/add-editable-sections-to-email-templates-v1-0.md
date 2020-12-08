---
unique-page-id: 1900585
description: Adicionar seções editáveis a modelos de e-mail v1.0 - Documentos do Marketing - Documentação do produto
title: Adicionar seções editáveis a modelos de e-mail v1.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Adicionar seções editáveis a modelos de e-mail v1.0 {#add-editable-sections-to-email-templates-v1.0}

Se você estiver criando um modelo no Editor de modelos de e-mail v1.0, poderá tornar qualquer seção editável colocando um especial `<div>` ao redor.

>[!NOTE]
>
>**Exemplo**
>`<pre> <div class="mktEditable" id="UNIQUE_ID">This part is editable</div></pre>`

Regras:

1. O HTML deve ser sempre válido.
1. A classe de **mktEditable** deve ser incluída.
1. A ID deve ser exclusiva nesse HTML.
1. Nenhum espaço na ID.

>[!CAUTION]
>
>instruções mktEditable não podem ser aninhadas.

Se quiser saber como fazer isso no Editor de modelos de e-mail v2.0, verifique a sintaxe [do modelo de](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)e-mail.
