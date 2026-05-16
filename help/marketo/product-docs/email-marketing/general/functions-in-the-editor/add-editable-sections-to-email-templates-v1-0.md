---
unique-page-id: 1900585
description: Saiba como adicionar seções editáveis a modelos de email na v1.0. Permitir que os usuários editem áreas específicas, mantendo o restante bloqueado.
title: Adicionar seções editáveis a modelos de email v1.0
exl-id: f397aa8e-0d0b-4007-91e1-9b9158bd6432
feature: Email Editor
TQID: https://experienceleague.adobe.com/j2rwpy7Bq-HH3-mva5FkDb3kKH8cvlH2hMUp0ic7sno
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 111
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
