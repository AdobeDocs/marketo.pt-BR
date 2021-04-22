---
unique-page-id: 2359918
description: Editar configurações de página de aterrissagem - Documentos do Marketo - Documentação do produto
title: Editar configurações de página inicial
exl-id: 019b4651-3a66-46f9-8722-66af30194380
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 3%

---

# Editar as configurações da página inicial {#edit-landing-page-settings}

É possível editar o nome de domínio e a página de fallback, ativar ou desativar o preenchimento do formulário, evitar o uso indevido da página de aterrissagem e muito mais. Veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Em **Admin**, clique em **Páginas de aterrissagem**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Na seção **Landing Pages**, clique em **Editar**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Insira seu domínio e informações da página.

   | Termo | Definição |
   |---|---|
   | Nome do domínio para landing pages | Este é o seu CNAME. Um CNAME é a primeira parte do URL que você fornece às pessoas para landing pages. Por exemplo, em `https://go.yourCompany.com`, a palavra &quot;go&quot; é o CNAME. Você pode ter vários, mas a maioria das pessoas só usa um. |
   | Página de fallback | Este é o local para onde ir se a landing page não existir ou estiver inativa. Saiba mais sobre [páginas de fallback](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Página inicial | Insira o URL do site corporativo. |

   ![](assets/three.png)

1. Marque a caixa de seleção **Preenchimento de formulário** para permitir que os formulários preencham previamente as informações para pessoas conhecidas (cookies). Desmarque para bloquear.

   ![](assets/four.png)

1. Se você quiser impedir que um site mal-intencionado hospede seu conteúdo, marque a caixa de seleção **Do not allow Marketo pages to be embedded in external web pages**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Se desejar que a tag `<script>` de preenchimento prévio apareça no final da tag `<head>` no código, marque a caixa **Inserir script de preenchimento prévio no final do cabeçalho**. Deixe desmarcado se quiser que ele apareça no início.
   >
   >Marque **Remove default favicon links** para impedir que o Marketo insira qualquer link favicon no código.

1. Depois de fazer suas seleções, clique em **Salvar.**

   ![](assets/six.png)

   Muito bem! Suas landing pages agora têm as informações certas e devem começar a funcionar imediatamente.
