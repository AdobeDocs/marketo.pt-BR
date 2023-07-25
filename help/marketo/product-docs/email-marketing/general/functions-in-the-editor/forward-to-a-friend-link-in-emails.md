---
unique-page-id: 1900581
description: Encaminhar para um link de amigo em emails - Documentação do Marketo - Documentação do produto
title: Encaminhar para um Amigo por e-mail
exl-id: 7addac65-4207-419f-845c-d6b2d08d299c
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Encaminhar para um Amigo por e-mail {#forward-to-a-friend-link-in-emails}

Adicionar o link ‘Encaminhar para o amigo’ aos seus emails permite rastrear pessoas que receberam um email encaminhado por meio desse link e automaticamente as adiciona como uma nova pessoa se ainda não estiverem no banco de dados.

Por exemplo, digamos que Keith use o link &#39;Encaminhar para o amigo&#39; para encaminhar o email a uma pessoa desconhecida, Mark. Mark é automaticamente adicionado como uma nova pessoa, recebe seu próprio cookie atribuído e qualquer atividade de email e da Web é vinculada a ele. No entanto, se Keith usa o botão de avanço em seu cliente de e-mail, Mark é incorretamente cozido como Keith, e sua atividade é registrada como Keith.

## Adicionar o link a um modelo de email {#add-the-link-to-an-email-template}

1. Vá para a **Design Studio**.

   ![](assets/one-8.png)

1. Localize e selecione o template de email ao qual deseja adicionar o link. Clique em **Editar rascunho**.

   ![](assets/two-7.png)

1. Cole o seguinte código de HTML onde deseja que o link &#39;Encaminhar para Amigo&#39; apareça (se precisar de ajuda com esta parte, entre em contato com seu desenvolvedor da Web):

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >É possível adicionar estilo ao link para deixá-lo mais bonito. Por exemplo:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Não recomendamos usar o estilo **posição:relativa** no modelo de email. Isso pode criar problemas com a posição e exibição da caixa &#39;Encaminhar para um amigo&#39;.

1. Clique em **Visualizar rascunho** para garantir que o modelo tenha a aparência desejada.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >Lembre-se de aprovar o rascunho do modelo para aplicar as alterações.

   Agora, todos os emails que usam esse modelo terão o link &#39;Encaminhar para um amigo&#39;. Quando o recipient do email clicar nele, ele será direcionado para uma versão da Web do email com a caixa &quot;Encaminhar para um amigo&quot;:

   ![](assets/f2afbox.png)

## Adicionar o link a um email individual {#add-the-link-to-an-individual-email}

Você também pode adicionar o link &quot;Encaminhar para o amigo&quot; diretamente em um email.

1. Abra o email que deseja incluir no link e clique duas vezes na área editável.

   ![](assets/five-4.png)

1. Coloque o cursor onde deseja que o link apareça e clique no link **Inserir token** botão.

   ![](assets/six-2.png)

1. Selecione o **`{{system.forwardToFriendLink}}`** token.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Este token é o URL da versão da Web do email com uma caixa &quot;Encaminhar para o amigo&quot;.

1. Escreva o texto a ser exibido no link (por exemplo, &quot;Encaminhar para um amigo&quot;).

   ![](assets/seven-1.png)

1. Recorte a **`{{system.forwardToFriendLink}}`** token usando Ctrl+X (Windows) ou Cmd+X (Mac). Selecione &quot;Encaminhar para um amigo&quot; e clique no link **Inserir/Editar link** botão.

   ![](assets/eight-1.png)

1. Cole o **`{{system.forwardToFriendLink}}`** token no **URL** usando Ctrl/Cmd+V e, em seguida, clique em **Inserir**.

   ![](assets/nine.png)

1. Salve a edição e visualize seu novo link!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >As novas pessoas que são adicionadas ao receber um email &quot;Encaminhar para um amigo&quot; têm a assinatura cancelada de emails de marketing.

## Exibir atividade de encaminhamento {#view-forwarding-activity}

Você pode ver quem encaminhou e recebeu os emails no Registro de atividades da pessoa.

1. Vá para a **`Database`**.

   ![](assets/db.png)

1. Clique duas vezes na pessoa cuja atividade você deseja exibir.

   ![](assets/fourteen.png)

1. Vá para a **Log de atividades** guia. Clique duas vezes **Email de encaminhamento para um amigo recebido** ou **Enviado para um e-mail amigo** para ver detalhes.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >Em E-mail de encaminhamento para amigo recebido, a ID de pessoa é a pessoa que encaminhou o e-mail.
   >
   >Para Email enviado para encaminhamento como amigo, a ID de pessoa é a pessoa que recebeu o email.

   ![](assets/sixteen.png)

1. Para exibir uma pessoa por ID, copie e cole a variável **ID de pessoa** até o final do URL (o início desse URL dependerá da instância do Marketo):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >Faremos o **ID de pessoa** clicável e vincular diretamente à pessoa em um patch futuro.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Se o amigo que recebe o encaminhamento for uma pessoa desconhecida, uma nova pessoa será criada com &quot;Encaminhar para o amigo&quot; marcado como o da pessoa **Origem**.
   >Se o email for um ativo local de um programa, o programa será marcado como do usuário **Programa de aquisição**.

## Acionar ou filtrar usando atividade de encaminhamento {#trigger-or-filter-using-forwarding-activity}

Há seis acionadores/filtros que você pode usar para acionar ações de fluxo ou filtrar pessoas por atividade &quot;Encaminhar para um amigo&quot; enviada e recebida.

Em uma lista inteligente de campanha inteligente, se pesquisar por &quot;encaminhar&quot;, você encontrará os acionadores e filtros disponíveis.

![](assets/nineteen.png)

## Testar Encaminhar para Amigo {#test-forward-to-friend}

Para testar &quot;Encaminhar para o amigo&quot;, envie um email com o link de encaminhamento. Certifique-se de enviá-lo por meio da **Enviar e-mail** etapa do fluxo, *não* até **Enviar email de teste**.
