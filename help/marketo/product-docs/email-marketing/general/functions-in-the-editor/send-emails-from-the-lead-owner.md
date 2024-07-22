---
unique-page-id: 1147340
description: Enviar emails do proprietário principal - Documentação do Marketo - Documentação do produto
title: Enviar Emails do Proprietário Principal
exl-id: b7ceb976-f52f-4134-8b7e-1c18d09af5de
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 1%

---

# Enviar Emails do Proprietário Principal {#send-emails-from-the-lead-owner}

E se você quiser enviar um email para um cliente potencial em nome do Proprietário do cliente potencial?  Veja como.

1. Encontre seu email, selecione-o e clique em **Editar Rascunho**.

   ![](assets/one.png)

1. Clique no campo **De** (exclua qualquer nome existente) e clique no botão **Inserir token**.

   ![](assets/two.png)

1. Comece a digitar &quot;`{{lead.Lead Owner`&quot; e selecione o token **`{{lead.Lead Owner First Name}}`**.

   ![](assets/image2014-9-11-13-3a7-3a43.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **Inserir**.

   ![](assets/image2014-9-11-13-3a7-3a58.png)

1. Clique depois do primeiro token, adicione um espaço e clique no botão **Inserir token**.

   ![](assets/five.png)

1. Comece a digitar &quot;`{{lead.Lead Owner`&quot; e selecione o token **`{{lead.Lead Owner Last Name}}`**.

   ![](assets/image2014-9-11-13-3a8-3a24.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **Inserir**.

   ![](assets/image2014-9-11-13-3a8-3a39.png)

   >[!TIP]
   >
   >Verifique se você adicionou um espaço entre os tokens de nome e sobrenome.

1. Clique em no campo Do email (exclua qualquer endereço de email existente) e clique no botão Inserir token.

   ![](assets/eight.png)

1. Comece a digitar &quot;`{{lead.Lead Owner`&quot; e selecione o token **`{{lead.Lead Owner Email Address}}`**.

   ![](assets/image2014-9-11-13-3a9-3a33.png)

1. Insira um valor padrão caso o cliente potencial ainda não tenha um proprietário de cliente potencial e clique em **Inserir**.

   ![](assets/ten.png)

1. Verifique se os campos **Responder-para** e **Assunto** estão preenchidos, e pronto!

   ![](assets/eleven.png)
