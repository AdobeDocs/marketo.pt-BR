---
unique-page-id: 1900581
description: Encaminhar para um link de amigo em emails - Documentos do Marketo - Documentação do produto
title: Encaminhar para um link de amigo em emails
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Encaminhar para um link de amigo em emails {#forward-to-a-friend-link-in-emails}

Adicionar o link &quot;Encaminhar para o Amigo&quot; aos seus emails permite rastrear pessoas que receberam um email encaminhado por meio desse link e adicioná-las automaticamente como uma nova pessoa se ainda não estiverem no banco de dados.

Por exemplo, digamos que Keith use o link &quot;Encaminhar para o Amigo&quot; para encaminhar o email a uma pessoa desconhecida, Mark. O Mark é adicionado automaticamente como uma nova pessoa, recebe seu próprio cookie e qualquer um de seus emails e atividades da Web é vinculado a ele. No entanto, se Keith usar o botão de encaminhamento em seu cliente de email, Mark recebe um cookie incorreto como Keith e sua atividade é registrada como Keith.

## Adicionar o link a um modelo de email {#add-the-link-to-an-email-template}

1. Vá para o **Design Studio**.

   ![](assets/one-8.png)

1. Localize e selecione o template de email ao qual deseja adicionar o link. Clique em **Editar rascunho**.

   ![](assets/two-7.png)

1. Cole o seguinte código de HTML onde deseja que o link &quot;Encaminhar para o Amigo&quot; apareça (se precisar de ajuda com essa parte, consulte seu desenvolvedor da Web):

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >É possível adicionar estilo ao link para torná-lo mais bonito. Por exemplo:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Não recomendamos usar o estilo **posição:relativa** no seu template de email. Ele pode criar problemas com a posição e a exibição da caixa &quot;Encaminhar para o Amigo&quot;.

1. Clique em **Visualizar rascunho** para garantir que o modelo tenha a aparência desejada.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Lembre-se de aprovar o rascunho do template para aplicar as alterações.

   Agora, todos os emails que usam esse modelo terão o link &quot;Encaminhar para o Amigo&quot;. Quando o destinatário do email clica nele, ele é direcionado para uma versão da Web do email com a caixa &quot;Encaminhar para um amigo&quot;:

   ![](assets/f2afbox.png)

## Adicionar o link a um email individual {#add-the-link-to-an-individual-email}

Você também pode adicionar o link &quot;Encaminhar para um Amigo&quot; diretamente em um email.

1. Abra o email no qual deseja incluir o link e clique duas vezes na área editável.

   ![](assets/five-4.png)

1. Coloque o cursor onde deseja que o link apareça e clique no botão **Inserir Token** botão.

   ![](assets/six-2.png)

1. Selecione o **`{{system.forwardToFriendLink}}`** token.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Esse token é o URL da versão da Web do email com uma caixa &quot;Encaminhar para o Amigo&quot;.

1. Escreva o que deseja que seja o texto de exibição do link (por exemplo, &quot;Encaminhar para um Amigo&quot;).

   ![](assets/seven-1.png)

1. Corte o **`{{system.forwardToFriendLink}}`** Token usando Ctrl+X (Windows) ou Cmd+X (Mac). Realce &quot;Encaminhar para um amigo&quot; e clique no botão **Inserir/Editar link** botão.

   ![](assets/eight-1.png)

1. Cole o **`{{system.forwardToFriendLink}}`** token no **URL** caixa usando Ctrl/Cmd+V, em seguida, clique em **Inserir**.

   ![](assets/nine.png)

1. Salve a edição e visualize o novo link!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Por padrão, as novas pessoas que são adicionadas por meio do recebimento de um email de &quot;Encaminhar para um amigo&quot; cancelam a assinatura dos emails de marketing.

## Exibir atividade de encaminhamento {#view-forwarding-activity}

Você pode ver quem encaminhou e recebeu os emails no registro de atividades da pessoa.

1. Vá para o **`Database`**.

   ![](assets/db.png)

1. Clique duas vezes na pessoa para a qual deseja exibir a atividade.

   ![](assets/fourteen.png)

1. Vá para o **Log de atividades** guia . Clique duas vezes **Enviar para o Amigo Recebido** ou **Enviado para o Email Amigo** para ver detalhes.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >Para o email de encaminhamento recebido para o amigo, a ID de pessoa é a pessoa que encaminhou o email.
   >
   >Para Enviar e-mail para amigo, a ID de pessoa é a pessoa que recebeu o e-mail.

   ![](assets/sixteen.png)

1. Para exibir uma pessoa por ID, copie e cole o **ID da pessoa** ao final do URL (o início desse URL dependerá da instância do Marketo):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >Faremos o **ID da pessoa** clicável e vinculado diretamente à pessoa em um patch futuro.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Se o amigo que recebe o encaminhamento for uma pessoa desconhecida, uma nova pessoa é criada com a opção &quot;Encaminhar para Amigo&quot; marcada como a **Origem**.
   >Se o email for um ativo local de um programa, o programa será marcado como **Programa de aquisição**.

## Acionar ou filtrar usando a atividade de encaminhamento {#trigger-or-filter-using-forwarding-activity}

Há seis acionadores/filtros que você pode usar para acionar ações de fluxo ou filtrar pessoas por atividade de &#39;Encaminhar para amigo&#39; enviada e recebida.

Na lista inteligente de uma campanha inteligente, se você pesquisar por &quot;encaminhar&quot;, você encontrará os acionadores e filtros disponíveis.

![](assets/nineteen.png)

## Testar Encaminhamento para Amigo {#test-forward-to-friend}

Para testar &quot;Encaminhar para o Amigo&quot;, envie um email para você com o link de encaminhamento. Certifique-se de enviá-lo por meio do **Enviar Email** degrau do fluxo, *not* through **Enviar email de teste**.
