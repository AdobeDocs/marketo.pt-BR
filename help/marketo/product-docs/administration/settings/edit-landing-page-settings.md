---
unique-page-id: 2359918
description: Editar configurações de página de aterrissagem - Documentos do Marketo - Documentação do produto
title: Editar configurações de página inicial
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 3%

---

# Editar configurações de página inicial {#edit-landing-page-settings}

É possível editar o nome de domínio e a página de fallback, ativar ou desativar o preenchimento do formulário, evitar o uso indevido da página de aterrissagem e muito mais. Veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para o **Administrador** área.

   ![](assets/edit-landing-page-settings-1.png)

1. Clique em **Páginas de aterrissagem**.

   ![](assets/edit-landing-page-settings-2.png)

1. No **Páginas de aterrissagem** seção , clique em **Editar**.

   ![](assets/edit-landing-page-settings-3.png)

1. Insira seu domínio e informações da página.

   ![](assets/edit-landing-page-settings-4.png)

   | Termo | Definição |
   |---|---|
   | Nome do domínio para landing pages | Este é o seu CNAME. Um CNAME é a primeira parte do URL que você fornece às pessoas para landing pages. Por exemplo, em `https://go.yourCompany.com`, a palavra &quot;go&quot; é o CNAME. Você pode ter vários, mas a maioria das pessoas só usa um. |
   | Página de fallback | Este é o local para onde ir se a landing page não existir ou estiver inativa. Saiba mais sobre [páginas de fallback](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Página inicial | Insira o URL do site corporativo. |

1. Verifique a **Preenchimento do formulário** caixa de seleção para permitir que formulários preencham previamente informações para pessoas conhecidas (com cookies). Desmarque para bloquear.

   ![](assets/edit-landing-page-settings-5.png)

1. Se você quiser impedir que um site mal-intencionado hospede seu conteúdo, verifique a **Não permitir que páginas do Marketo sejam incorporadas a páginas da Web externas** caixa de seleção.

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >Se desejar preencher `<script>` a ser exibida no final do `<head>` no código, verifique a **Inserir script de preenchimento prévio no final do cabeçalho** caixa. Deixe desmarcado se quiser que ele apareça no início.
   >
   >Verificar **Remover links favicon padrão** para impedir que o Marketo insira qualquer link favicon no código.

1. Depois de fazer suas seleções, clique em **Salvar.**

   ![](assets/edit-landing-page-settings-7.png)

   Muito bem! Suas landing pages agora têm as informações certas e devem começar a funcionar imediatamente.
