---
unique-page-id: 7512454
description: Configurar notificação por push para dispositivos móveis - Documentação do Marketo - Documentação do produto
title: Configurar notificação por push para dispositivos móveis
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Configurar notificação por push para dispositivos móveis {#configure-mobile-push-notification}

1. Vá para a **Atividades de marketing** área.

![](assets/2fbf1ab6-2247-40c8-980d-be56b9d94890.png)

1. Selecione o ativo de push e clique em **Editar rascunho**.

   ![](assets/image2016-8-23-16-3a49-3a48.png)

1. Ir para **Configuração**.

   ![](assets/image2016-8-23-16-3a51-3a56.png)

1. Selecione o aplicativo desejado. As plataformas Android e Apple são ativadas por padrão.

   ![](assets/image2016-8-23-16-3a53-3a33.png)

1. Se a sua mensagem por push se aplicar a apenas uma plataforma (por exemplo, casos para iPhones), você poderá excluir a outra plataforma deslizando seu seletor para Desativado.

   ![](assets/image2016-8-23-16-3a41-3a48.png)

1. Clique em **Próxima**.

   ![](assets/image2016-8-23-16-3a43-3a28.png)

1. Insira o texto da mensagem ou selecione o ícone de token para adicionar tokens. Em seguida, selecione um **Toque em Ação**.

   ![](assets/image2015-9-14-16-3a7-3a43.png)

   >[!NOTE]
   >
   >Se uma plataforma estiver ativada, ela aparecerá no lado esquerdo da tela do telefone. Ele é exibido em cor quando é selecionado.

   >[!NOTE]
   >
   >Há três tipos de ações de toque:
   >
   >**Iniciar aplicativo** - **Este aplicativo** abre a página inicial do aplicativo quando a notificação é tocada. **Personalizado** O usa um deep link para abrir outras áreas do aplicativo ou qualquer outro aplicativo para o qual você tenha o link (consulte [URIs de deep link](#Deeplink) abaixo para obter detalhes).
   >
   >**Landing Page** - leva você a uma página de aterrissagem do Marketo especificada.
   >
   >**URL externo** - leva você a uma página de aterrissagem que não seja da Marketo.

1. Para inserir um deep link para uma ação de toque personalizada, clique em Personalizado e insira o [URI do deep link](#Deeplink) no campo.

   ![](assets/image2016-7-28-16-3a19-3a13.png)

1. Para inserir tokens, selecione um token, insira um valor padrão e clique em Insert.

   >[!NOTE]
   >
   >Os tokens são exibidos onde você coloca o cursor na caixa de texto. Você pode usar mais de um token.

   ![](assets/image2015-8-10-14-3a48-3a52.png)

   >[!NOTE]
   >
   >As mensagens e as ações de toque serão iguais em ambas as plataformas.

1. Somente para o iOS, marque a caixa de seleção para informar ao aplicativo para reproduzir um som quando a mensagem chegar. O Android reproduz o som automaticamente.

   ![](assets/ios-tap-and-notification-hand.png)

1. Visualize a outra plataforma e clique em **Concluir**.

   ![](assets/image2015-9-14-16-3a12-3a34.png)

1. Clique em **Aprovar e fechar**.

   ![](assets/323dda12-0543-4558-8562-563eed5fa0e0.png)

Parabéns! Agora, a notificação por push está pronta para ser enviada.

## URIs de deep link {#deep-link-uris}

Quando os assinantes clicam em um botão em uma mensagem por push, ele pode levá-los para a página inicial do seu aplicativo ou diretamente para uma página específica no aplicativo. Um deep link é uma referência exclusiva a uma página específica no seu aplicativo e se parece muito com um link de site.

Um URI de deep link é composto de três partes: nome do esquema, caminho e identificador. No exemplo abaixo, &quot;myappname&quot; é o schema. &quot;products&quot; é o caminho e &quot;purple-shirt&quot; é o identificador. Quando o cliente toca, ele é direcionado especificamente para o item de camisa roxa nas páginas de produto do aplicativo.

![](assets/image2016-7-29-12-3a49-3a1.png)

Dito isso, a estrutura de deep link do seu aplicativo pode ser diferente do exemplo acima. Seu desenvolvedor tem muitas opções para definir URIs de deep link. Portanto, peça ao desenvolvedor para enviar os URIs (links) para as páginas que você está interessado em usar. Isso garantirá que os URIs inseridos nas mensagens de push apontem para os locais corretos. Seu desenvolvedor pode [encontre mais informações aqui](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Enviar uma notificação por push em dispositivo móvel](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
