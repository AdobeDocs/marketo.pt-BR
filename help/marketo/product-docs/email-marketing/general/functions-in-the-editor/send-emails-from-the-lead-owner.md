---
unique-page-id: 1147340
description: Enviar emails do proprietário líder - Documentos da Marketo - Documentação do produto
title: Enviar Emails do Proprietário Potencial
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# Enviar Emails do Proprietário Potencial {#send-emails-from-the-lead-owner}

E se você quiser enviar um email para um cliente potencial em nome do Proprietário principal?  Veja como.

1. Encontre seu email, selecione-o e clique em **Editar rascunho**.

   ![](assets/one.png)

1. Clique no botão **De** (exclua qualquer nome existente) e clique no botão **Inserir Token** botão.

   ![](assets/two.png)

1. Comece digitando &quot;`{{lead.Lead Owner`&quot; e selecione o **`{{lead.Lead Owner First Name}}`** token.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **Inserir**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Clique depois do primeiro token, adicione um espaço e clique no botão **Inserir Token** botão.

   ![](assets/five.png)

1. Comece digitando &quot;`{{lead.Lead Owner`&quot; e selecione o **`{{lead.Lead Owner Last Name}}`** token.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **Inserir**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Certifique-se de ter adicionado um espaço entre os tokens de nome e sobrenome.

1. Clique no campo De email (exclua qualquer endereço de email existente) e clique no botão Inserir token .

   ![](assets/eight.png)

1. Comece digitando &quot;`{{lead.Lead Owner`&quot; e selecione o **`{{lead.Lead Owner Email Address}}`** token.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **Inserir**.

   ![](assets/ten.png)

1. Certifique-se de que o **Responder para** e **Assunto** Os campos são preenchidos e você está pronto!

   ![](assets/eleven.png)
