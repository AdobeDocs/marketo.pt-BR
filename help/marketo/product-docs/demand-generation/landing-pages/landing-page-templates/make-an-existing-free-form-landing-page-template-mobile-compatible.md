---
unique-page-id: 5472348
description: Tornar um modelo de página de aterrissagem de formato livre existente compatível com dispositivos móveis - Documentação do Marketo - Documentação do produto
title: Tornar um modelo de página de aterrissagem de forma livre compatível com dispositivos móveis
exl-id: 942456a5-3f3e-4a71-aecc-4cc6bf6237b3
feature: Landing Pages
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---

# Tornar um modelo de página de aterrissagem de forma livre compatível com dispositivos móveis {#make-an-existing-free-form-landing-page-template-mobile-compatible}

Isso pode ser feito em dois lugares, o Editor de modelo e o Editor de landing page.

## Atualizar a partir do Editor de modelo {#upgrade-from-the-template-editor}

1. Vá para o **Design Studio**.

   ![](assets/designstudio-1.png)

1. Selecione **Modelos**.

   ![](assets/image2015-1-22-20-3a20-3a2.png)

1. Selecione um modelo em que **Compatível com Dispositivos Móveis** seja **Não**.

   ![](assets/image2015-1-22-20-3a22-3a24.png)

1. Clique em **Editar rascunho**.

   ![](assets/image2015-1-22-20-3a25-3a36.png)

1. Clique em **Tornar o Mobile compatível**.

   ![](assets/image2015-1-22-20-3a30-3a33.png)

1. Clique em **Atualizar**.

   ![](assets/image2015-1-22-20-3a32-3a45.png)

   Seu template de landing page agora é compatível com dispositivos móveis!

   >[!NOTE]
   >
   >A atualização deve ser inofensiva, mas verifique se há discrepâncias nas páginas. A atualização criará rascunhos de qualquer landing page que use esse modelo.

   ![](assets/image2015-1-22-20-3a36-3a43.png)

## O que torna um modelo para dispositivos móveis compatível? {#what-makes-a-template-mobile-compatible}

Ótimas perguntas! Seu modelo deve ter as seguintes tags:

`Must have <!DOCTYPE HTML> Must have a <HEAD> element Must have a <TITLE> in the <HEAD> element Must have <META CHARSET="UTF-8"> within the <HEAD> element Must have a <BODY> element that contains one (and only one) <DIV class="mktoContent"></DIV>`

Se tudo estiver bem, você verá esta mensagem.

![](assets/image2015-1-22-20-3a41-3a31.png)

Se algo estiver errado, uma mensagem de erro será exibida. Clique em reparar para corrigir o problema e repetir o processo de validação.

![](assets/image2015-1-22-20-3a43-3a20.png)

Se você fizer alterações no modelo, clique em Ações do modelo e selecione Validar compatibilidade móvel.

## Atualização de um modelo do editor de página de aterrissagem de forma livre {#upgrading-a-template-from-the-free-form-landing-page-editor}

Ao editar uma landing page e clicar na guia móvel, às vezes você notará que o template não foi atualizado. Não tema! Você pode atualizá-lo lá mesmo.

1. Clique na guia **Mobile**.

   ![](assets/image2015-1-22-20-3a48-3a19.png)

1. Clique na caixa de seleção e clique em **Ativar**.

   ![](assets/image2015-1-22-20-3a49-3a34.png)

   >[!NOTE]
   >
   >Ativar a versão móvel de um modelo criará rascunhos de qualquer landing page que o use.

Fantástico! Agora você pode [personalizar a exibição móvel](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/customize-mobile-view-for-your-free-form-landing-page.md) de todas as páginas de aterrissagem que usam este modelo.
