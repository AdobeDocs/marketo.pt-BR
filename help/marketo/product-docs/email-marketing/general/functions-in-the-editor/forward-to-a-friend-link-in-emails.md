---
unique-page-id: 1900581
description: Encaminhar para um link de amigo em emails - Documentos de marketing - Documentação do produto
title: Encaminhar para um link de amigo em emails
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---


# Encaminhar para um link de amigo em emails {#forward-to-a-friend-link-in-emails}

Adicionar o link &quot;Encaminhar para o Amigo&quot; aos seus emails permite rastrear pessoas que receberam um email encaminhado por meio desse link e adicioná-las automaticamente como uma nova pessoa se ainda não estiverem no banco de dados.

Por exemplo, digamos que Keith use o link &quot;Encaminhar para o amigo&quot; para encaminhar o email para uma pessoa desconhecida, Mark. Mark é automaticamente adicionado como uma nova pessoa, recebe seu próprio cookie e qualquer um de seus emails e atividades da Web é vinculado a ele. Entretanto, se Keith usar o botão de avanço em seu cliente de email, Mark recebe um cookie incorreto como Keith, e sua atividade é registrada como Keith.

## Adicionar o link a um modelo de email {#add-the-link-to-an-email-template}

1. Vá para o **Design Studio**.

   ![](assets/one-8.png)

1. Localize e selecione o modelo de e-mail ao qual deseja adicionar o link. Clique em **Editar rascunho**.

   ![](assets/two-7.png)

1. Cole o seguinte código HTML onde deseja que o link &quot;Encaminhar para o amigo&quot; seja exibido (se precisar de ajuda com esta parte, consulte seu desenvolvedor da Web):

   `<pre data-theme="Confluence"><a href="{{system.forwardToFriendLink}}">Forward to Friend</a></pre>`

   ![](assets/three-7.png)

   >[!TIP]
   >
   >
   >Você pode adicionar estilização ao link para torná-lo mais bonito. Por exemplo:
   >
   >`<a href="{{system.forwardToFriendLink}}" style="font-family:arial, sans-serif; padding:10px; position:absolute; right:0px;">Forward to Friend</a>`

   >[!CAUTION]
   >
   >Não recomendamos usar o estilo **position:relative** no seu modelo de email. Pode criar problemas com a posição e a exibição da caixa &quot;Encaminhar para o amigo&quot;.

1. Clique em **Rascunho de Pré-visualização** para verificar se o modelo tem a aparência desejada.

   ![](assets/four-5.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >Lembre-se de aprovar o rascunho do modelo para aplicar as alterações.

   Agora todos os emails que usam esse modelo terão o link &#39;Encaminhar para o amigo&#39;. Quando o recipient de email clicar nele, eles serão direcionados para uma versão da Web do email com a caixa &quot;Encaminhar para um amigo&quot;:
   ![](assets/f2afbox.png)

## Adicionar o link a um email individual {#add-the-link-to-an-individual-email}

Você também pode adicionar o link &quot;Encaminhar para o amigo&quot; diretamente em um email.

1. Abra o e-mail no qual deseja incluir o link e clique com o duplo na área editável.

   ![](assets/five-4.png)

1. Coloque o cursor onde deseja que o link apareça e clique no botão **Inserir token**.

   ![](assets/six-2.png)

1. Selecione o token **`{{system.forwardToFriendLink}}`**.

   ![](assets/seven-1.png)

   >[!NOTE]
   >
   >Este token é o URL da versão da Web do email com uma caixa &quot;Encaminhar para o amigo&quot;.

1. Escreva o que deseja que seja o texto de exibição do link (por exemplo, &quot;Encaminhar para um amigo&quot;).

   ![](assets/seven-1.png)

1. Recorte o token **`{{system.forwardToFriendLink}}`** usando Ctrl+X (Windows) ou Cmd+X (Mac). Realce &quot;Encaminhar para um amigo&quot; e clique no botão **Inserir/Editar link**.

   ![](assets/eight-1.png)

1. Cole o token **`{{system.forwardToFriendLink}}`** na caixa **URL** usando Ctrl/Cmd+V e clique em** Inserir**.

   ![](assets/nine.png)

1. Salve a edição e a pré-visualização do novo link!

   ![](assets/ten-1.png)

   >[!NOTE]
   >
   >Por padrão, as novas pessoas que são adicionadas por meio do recebimento de um e-mail &quot;Encaminhar para um amigo&quot; são canceladas de inscrição em e-mails de marketing.

## Atividade de encaminhamento de visualização {#view-forwarding-activity}

Você pode ver quem encaminhou e recebeu os emails no Registro de Atividades da pessoa.

1. Vá para **`Database`**.

   ![](assets/db.png)

1. Clique com o duplo na pessoa para a qual você deseja visualização a atividade.

   ![](assets/fourteen.png)

1. Vá para a guia **Log de Atividades**. Clique no duplo **Enviado para o Amigo e-mail** ou **Enviado para o Amigo e-mail** para ver os detalhes.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >
   >Para email de encaminhamento recebido para amigo, a ID de pessoa é a pessoa que encaminhou o email.
   >
   >
   >Para Enviado para email de amigo, a ID de pessoa é a pessoa que recebeu o email.

   ![](assets/sixteen.png)

1. Para visualização de uma pessoa por ID, copie e cole a ID de pessoa**** até o final do URL (o início desse URL dependerá da sua instância de marketing):

   `<pre data-theme="Confluence">...marketo.com/Database/loadPersonDetail?personId=</pre>`

   >[!NOTE]
   >
   >Nós tornaremos a **ID da pessoa** clicável e vincularemos diretamente à pessoa em um patch futuro.

   ![](assets/seventeen.png)

   >[!NOTE]
   >
   >Se o amigo que recebe o encaminhamento for uma pessoa desconhecida, uma nova pessoa será criada com a opção &quot;Encaminhar para o Amigo&quot; marcada como a **Fonte** da pessoa.\
   >Se o e-mail for um ativo local de um programa, o programa será marcado como o **Programa de aquisição** da pessoa.

## Acionar ou filtrar usando a Atividade de encaminhamento {#trigger-or-filter-using-forwarding-activity}

Existem seis acionadores/filtros que você pode usar para acionar ações de fluxo ou filtrar pessoas enviando e recebendo a atividade &quot;Encaminhar para o Amigo&quot;.

Em uma lista inteligente de campanha inteligente, se você pesquisar por &quot;avançar&quot;, você encontrará os acionadores e filtros disponíveis.

![](assets/nineteen.png)

## Testar encaminhamento para o amigo {#test-forward-to-friend}

Para testar &quot;Encaminhar para Amigo&quot;, envie um email para você mesmo com o link de encaminhamento. Certifique-se de enviá-lo pela etapa de fluxo **Enviar email**, *não* por **Enviar email de teste**.
