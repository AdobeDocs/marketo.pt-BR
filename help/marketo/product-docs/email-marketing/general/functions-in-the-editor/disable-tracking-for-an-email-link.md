---
unique-page-id: 1900579
description: Desabilitar rastreamento para um link de email - Documentos do Marketing - Documentação do produto
title: Desativar o rastreamento para um link de email
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---


# Desativar o rastreamento para um link de email {#disable-tracking-for-an-email-link}

Às vezes, você não quer ativar o URL **de rastreamento de** marketing em um link em um email. Isso é útil quando a página de destino não suporta parâmetros de URL e pode resultar em um link quebrado.

>[!NOTE]
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](/help/marketo/getting-started/updates-to-marketo-terminology.md).

1. Selecione seu email e clique em **Editar** **rascunho**.

   ![](assets/one-7.png)

1. Clique com o duplo na seção editável que contém o link.

   ![](assets/two-6.png)

1. Clique no link em questão e, em seguida, clique no botão **Inserir/Editar link** .

   ![](assets/three-6.png)

1. No pop-up Editar link, desmarque a caixa de seleção **Rastrear link** .

   ![](assets/four-4.png)

1. Você notará que a caixa **Incluir mkt_tok** desaparece. Clique em **Aplicar**.

   ![](assets/five-3.png)

   >[!TIP]
   >
   >Desmarcar apenas **Incluir mkt_tok** permitirá que o link seja rastreado, mas após o redirecionamento, o URL de destino não incluirá o parâmetro de string de query mkt_tok. Este parâmetro é usado pelo Marketo Landing page e Munchkin para garantir o rastreamento correto das atividades pessoais (como quando uma pessoa se cancela a assinatura de um email). Evite usar esse recurso, a menos que você veja um comportamento estranho em seu site devido ao parâmetro estar presente.

1. Clique em **Salvar**.

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!TIP]
   >
   >Deseja desativar o rastreamento de cliques para um link em um **modelo**de email? Use este formato:
   >`<a class="mktNoTrack" href="http://www.mywebsite.com">This link does not have tracking</a>`\
   >Se precisar de ajuda para implementar isso, consulte seu desenvolvedor da Web.

Legal! Agora você desabilitou o rastreamento de um link.
