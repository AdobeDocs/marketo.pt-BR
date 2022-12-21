---
unique-page-id: 5472348
description: Tornar um modelo de página de aterrissagem livre existente compatível com dispositivos móveis - Documentos do Marketo - Documentação do produto
title: Tornar um modelo de página de aterrissagem de forma livre compatível com dispositivos móveis
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Tornar um modelo de página de aterrissagem de forma livre compatível com dispositivos móveis {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Isso pode ser feito em dois lugares, o Editor de modelo e o Editor de página de aterrissagem.

## Atualizar a partir do Editor de Modelos {#upgrade-from-the-template-editor}

1. Vá para o **Design Studio**.

   ![](assets/designstudio-1.png)

1. Selecionar **Modelos**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Selecione um modelo em que **Compatível com dispositivos móveis** é **Não**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Clique em **Editar rascunho**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Clique em **Tornar o Mobile Compatível**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Clique em **Atualizar**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Seu modelo de landing page agora é compatível com dispositivos móveis!

   >[!NOTE]
   >
   >A atualização deve ser inofensiva, mas verifique se as páginas estão discrepantes. A atualização criará rascunhos de qualquer página de aterrissagem usando esse modelo.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## O que torna um modelo móvel compatível? {#what-makes-a-template-mobile-compatible}

Grandes perguntas! Seu modelo deve ter as seguintes tags:

`<pre data-theme="Confluence">Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV></pre>`

Se tudo parecer bom, você verá esta mensagem.

![](assets/image2015-1-22-20-3a41-3a31.png)

Se algo estiver errado, uma mensagem de erro será exibida, clique em reparar para corrigir o problema e repetir o processo de validação.

![](assets/image2015-1-22-20-3a43-3a20.png)

Se você fizer alterações no modelo, clique em Ações do modelo e selecione Validar compatibilidade móvel.

## Atualização de um modelo no editor de páginas de aterrissagem de forma livre {#upgrading-a-template-from-the-free-form-landing-page-editor}

Ao editar uma página de aterrissagem e clicar na guia móvel, você às vezes observará que o modelo não foi atualizado. Medo não! Você pode atualizá-lo aqui mesmo.

1. Clique no botão **Celular** guia .

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Clique na caixa de seleção e em **Ativar**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Ativar a versão móvel de um modelo criará rascunhos de qualquer página de aterrissagem que o utilize.

Ótimo! Agora você pode [personalizar a visualização móvel](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) de todas as suas landing pages que usam esse template.
