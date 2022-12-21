---
unique-page-id: 1900579
description: Desative o rastreamento de um link de email - Documentos do Marketo - Documentação do produto
title: Desativar o rastreamento para um link de email
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Desativar o rastreamento para um link de email {#disable-tracking-for-an-email-link}

Às vezes, você não quer ativar a variável **URL de rastreamento do Marketo** em um link em um email. Isso é útil quando a página de destino não suporta parâmetros de URL e pode resultar em um link quebrado.

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/one-7.png)

1. Clique duas vezes na seção editável que contém o link.

   ![](assets/two-6.png)

1. Clique no link em questão e, em seguida, clique no link **Inserir/Editar link** botão.

   ![](assets/three-6.png)

1. Na janela pop-up Editar link , desmarque a opção **Rastrear link** caixa de seleção.

   ![](assets/four-4.png)

1. Você notará o **Incluir caixa mkt_tok** desaparece. Clique em **Aplicar**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Desmarcar apenas **Inclua mkt_tok** O ainda permitirá que o link seja rastreado, mas após o redirecionamento, o URL de destino não incluirá o parâmetro da string de consulta mkt_tok . Esse parâmetro é usado pelas Páginas de aterrissagem e pelo Munchkin do Marketo para garantir o rastreamento adequado das atividades da pessoa (como quando uma pessoa cancela a assinatura de um email). Evite usar esse recurso, a menos que esteja vendo um comportamento estranho no site devido ao parâmetro estar presente.

1. Clique em **Salvar**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Deseja desativar o rastreamento de cliques para um link em um email **modelo**? Use este formato:
   >`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`\
   >Se precisar de ajuda para implementar isso, consulte seu desenvolvedor da Web.

Legal! Agora você desativou o rastreamento de um link.
