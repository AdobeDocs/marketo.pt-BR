---
unique-page-id: 2359918
description: Editar configurações de Landing page - Documentos de marketing - Documentação do produto
title: Editar configurações de Landing page
translation-type: tm+mt
source-git-commit: 95ca406109e04f56c9846f83cb2c4202bf606518
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Editar configurações de Landing page {#edit-landing-page-settings}

Você pode editar o nome do domínio e a página de fallback, ativar ou desativar o preenchimento prévio do formulário, impedir o uso indevido da sua landing page e muito mais. Veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Em **Admin**, clique em **Landing page**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. Na seção **Landing page**, clique em **Editar**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Insira suas informações de domínio e página.

   | Termo | Definição |
   |---|---|
   | Nome de domínio para landing page | Este é o seu CNAME. Um CNAME é a primeira parte do URL que você fornece às pessoas para landings page. Por exemplo, em `http://go.yourCompany.com`, a palavra &quot;go&quot; é CNAME. Você pode ter vários, mas a maioria das pessoas apenas usa um. |
   | Página de fallback | É para onde ir se a landing page não existe ou está baixa. Saiba mais sobre [páginas de fallback](set-a-fallback-page.md). |
   | Página inicial | Insira o URL do site corporativo. |

   ![](assets/three.png)

1. Marque a caixa de seleção **Preenchimento do formulário** para permitir que os formulários preencham previamente as informações de pessoas conhecidas (cookies). Desmarque para bloquear.

   ![](assets/four.png)

1. Se você quiser impedir que um site mal-intencionado hospede seu conteúdo, marque a caixa de seleção **Não permitir que as páginas do Marketing sejam incorporadas em páginas externas da Web**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Se desejar que a tag prefill `<script>` apareça no final da tag `<head>` no código, marque a caixa **Injetar script de pré-preenchimento no final do Head**. Deixe desmarcado se quiser que apareça no início.
   >
   >Marque **Remova os links de favicon padrão** para impedir que o Marketo insira qualquer link de favicon no código.

1. Depois de fazer suas seleções, clique em **Salvar.**

   ![](assets/six.png)

   Ótimo trabalho! Suas landings page agora têm as informações certas e devem ser start trabalhando imediatamente.

