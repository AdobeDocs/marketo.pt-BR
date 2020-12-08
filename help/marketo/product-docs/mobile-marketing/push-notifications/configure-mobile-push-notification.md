---
unique-page-id: 7512454
description: Configurar notificação por push móvel - Documentos do Marketing - Documentação do produto
title: Configurar notificação por push móvel
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Configurar notificação por push móvel {#configure-mobile-push-notification}

1. Vá para a área Atividades de marketing.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Selecione o ativo de push e clique em **Editar rascunho**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Vá para **Configuração**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Selecione o aplicativo desejado. As plataformas Android e Apple são ativadas por padrão.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

   Se sua mensagem de push se aplicar a apenas uma plataforma (por exemplo, casos para iPhones), você poderá excluir a outra plataforma deslizando seu seletor para Desativado.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

   Clique em PRÓXIMO.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Insira o texto da mensagem ou selecione o ícone do token para adicionar tokens. Em seguida, selecione **Toque em Ação**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Se uma plataforma estiver ativada, ela será exibida no lado esquerdo da tela do telefone. É exibido em cores quando é selecionado.

   >[!NOTE]
   >
   >**Definição**
   >
   >
   >Há três tipos de** Ações de toque:**
   >
   >
   >**Iniciar aplicativo** - **Este aplicativo** abre o home page do aplicativo quando a notificação é tocada. **O Custom** usa um deep link para abrir outras áreas do aplicativo ou de qualquer outro aplicativo ao qual você tenha o link (consulte URIs [do](#Deeplink) Deep Link abaixo para obter detalhes).
   >
   >
   >**landing page** - leva você para uma landing page de marketing especificada.
   >
   >
   >**URL** externo - leva você para uma landing page que não é de marketing.

   Para inserir um link profundo para uma ação de toque personalizada, clique em Personalizado e insira o URI [do link](#Deeplink) profundo no campo.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

   Para inserir tokens, selecione um token, insira um valor padrão e clique em Inserir.

   >[!NOTE]
   >
   >Os tokens são exibidos no local em que o cursor é colocado na caixa de texto. Você pode usar mais de um token.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >As ações de mensagem e toque serão idênticas em ambas as plataformas.

   Somente para iOS, marque a caixa de seleção para instruir o aplicativo a reproduzir um som quando a mensagem chegar. O Android reproduz o som automaticamente.

   ![](assets/ios-tap-and-notification-hand.png)

   Pré-visualização a outra plataforma e clique em FINISH (Concluir).

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Clique em **APROVAR e FECHAR**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Parabéns! Agora a notificação por push está pronta para ser enviada.

## URIs de deep link {#deep-link-uris}

Quando os assinantes clicam em um botão em uma mensagem de push, ele pode levá-los ao home page do aplicativo ou diretamente para uma página específica no aplicativo. Um deep link é uma referência exclusiva para uma página específica do seu aplicativo e se parece muito com um link de site.

Um URI de deep link é composto de três partes: nome do esquema, caminho e identificador. No exemplo abaixo, &quot;myappname&quot; é o esquema. &quot;products&quot; é o caminho e &quot;camiseta roxa&quot; é o identificador. Quando o cliente toca, eles são levados especificamente para o item de camisa violeta nas páginas de produto do aplicativo.

![](assets/image2016-7-29-12-3a49-3a1.png)

Dito isso, a estrutura de deep link do aplicativo pode ser diferente do exemplo acima. Seu desenvolvedor tem muitas opções para definir URIs de deep link, portanto peça ao desenvolvedor para enviar os URIs (links) das páginas que você está interessado em usar. Isso garantirá que os URIs inseridos nas mensagens de push apontem para os locais corretos. Seu desenvolvedor pode [encontrar mais informações aqui](http://developers.marketo.com/mobile/enabling-deep-links-in-your-app/).

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Enviar uma notificação por push móvel](send-a-mobile-push-notification.md)

>



