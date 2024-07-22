---
unique-page-id: 1900579
description: Desativar o rastreamento para um link de email - Documentação do Marketo - Documentação do produto
title: Desativar o rastreamento para um link de email
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 0%

---

# Desativar o rastreamento para um link de email {#disable-tracking-for-an-email-link}

Às vezes, você não quer habilitar a **URL de rastreamento do Marketo** em um link em um email. Isso é útil quando a página de destino não suporta parâmetros de URL e pode resultar em um link quebrado.

1. Selecione seu email e clique em **Editar Rascunho**.

   ![](assets/one-7.png)

1. Clique duas vezes na seção editável que contém o link.

   ![](assets/two-6.png)

1. Clique no link em questão e no botão **Inserir/Editar Link**.

   ![](assets/three-6.png)

1. Na janela pop-up Editar link, desmarque a caixa de seleção **Rastrear link**.

   ![](assets/four-4.png)

1. Você perceberá que a **Incluir mkt_tok box** desaparece. Clique em **Aplicar**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Se você desmarcar apenas **Incluir mkt_tok**, ainda permitirá que o link seja rastreado; porém, após o redirecionamento, a URL de destino não incluirá o parâmetro de cadeia de caracteres de consulta mkt_tok. Esse parâmetro é usado pelas páginas de aterrissagem do Marketo e pelo Munchkin para garantir o rastreamento adequado das atividades da pessoa (como quando uma pessoa cancela a assinatura de um email). Você deve evitar o uso desse recurso, a menos que esteja vendo um comportamento estranho em seu site devido à presença do parâmetro.

1. Clique em **Salvar**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Deseja desabilitar o rastreamento de cliques para um link em um email **modelo**? Usar este formato:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Se precisar de ajuda para implementar isso, consulte o desenvolvedor da Web.

Legal! Agora você desativou o rastreamento de um link.
