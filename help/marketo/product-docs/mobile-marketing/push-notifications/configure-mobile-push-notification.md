---
unique-page-id: 7512454
description: Configurar notificação por push para dispositivos móveis - Documentação do Marketo - Documentação do produto
title: Configurar notificação por push para dispositivos móveis
exl-id: 10368b13-40c9-435a-847c-68aaa5a892ea
feature: Mobile Marketing
source-git-commit: 7007c9f61bac2d5b860e166f285c87f565683933
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Configurar notificação por push para dispositivos móveis {#configure-mobile-push-notification}

1. Vá para a área **Atividades de marketing**.

   ![](assets/configure-mobile-push-notification-1.png)

1. Selecione seu ativo de push e clique em **Editar rascunho**.

   ![](assets/configure-mobile-push-notification-2.png)

1. Em **Configurar**, selecione o aplicativo desejado. As plataformas Android e Apple são ativadas por padrão.

   ![](assets/configure-mobile-push-notification-3.png)

   >[!NOTE]
   >
   >Se sua mensagem de push se aplicar a apenas uma plataforma (por exemplo, iOS), você poderá excluir a outra plataforma deslizando manualmente seu seletor para **Desabilitado**.

1. Clique em **Avançar**.

   ![](assets/configure-mobile-push-notification-4.png)

1. Insira o texto da mensagem ou selecione o ícone do token para adicionar tokens (neste editor, os tokens são formatados como [normalmente são](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) - você pode usar vários tokens). Selecione uma **Ação de toque**.

   ![](assets/configure-mobile-push-notification-5.png)

   >[!NOTE]
   >
   >Se uma plataforma estiver ativada, ela aparecerá no lado esquerdo da tela do telefone. Ele é exibido em cor quando é selecionado.

   >[!NOTE]
   >
   >Há três tipos de ações de toque:
   >
   >**Iniciar Aplicativo** - **Este Aplicativo** abre a home page do seu aplicativo quando a notificação é tocada. **Personalizado** usa um deep link para abrir outras áreas do aplicativo ou qualquer outro aplicativo para o qual você tenha o link (consulte [URIs de deep link](#deep-link-uris) abaixo para obter detalhes).
   >
   >**Página de aterrissagem** - leva você a uma página de aterrissagem do Marketo especificada.
   >
   >**URL externa** - direciona você a uma página de aterrissagem que não seja da Marketo.

1. Para inserir um deep link para uma ação de toque personalizada, selecione **Personalizado** e insira o [URI do deep link](#deep-link-uris) no campo.

   ![](assets/configure-mobile-push-notification-6.png)

   >[!NOTE]
   >
   >As mensagens e as ações de toque serão iguais em ambas as plataformas.

1. Somente para o iOS, marque a caixa de seleção para informar ao aplicativo para reproduzir um som quando a mensagem chegar. O Android reproduz o som automaticamente.

   ![](assets/configure-mobile-push-notification-7.png)

1. Visualize a outra plataforma e clique em **Concluir**.

   ![](assets/configure-mobile-push-notification-8.png)

1. Clique em **Aprovar e Fechar**.

   ![](assets/configure-mobile-push-notification-9.png)

Parabéns! Agora, a notificação por push está pronta para ser enviada.

## URIs de deep link {#deep-link-uris}

Quando os assinantes clicam em um botão em uma mensagem por push, ele pode levá-los para a página inicial do seu aplicativo ou diretamente para uma página específica no aplicativo. Um deep link é uma referência exclusiva a uma página específica no seu aplicativo e se parece muito com um link de site.

Um URI de deep link é composto de três partes: nome do esquema, caminho e identificador. No exemplo abaixo, &quot;myappname&quot; é o schema. &quot;products&quot; é o caminho e &quot;purple-shirt&quot; é o identificador. Quando o cliente toca, ele é direcionado especificamente para o item de camisa roxa nas páginas de produto do aplicativo.

![](assets/configure-mobile-push-notification-10.png)

Dito isso, a estrutura de deep link do seu aplicativo pode ser diferente do exemplo acima. Seu desenvolvedor tem muitas opções para definir URIs de deep link. Portanto, peça ao desenvolvedor para enviar os URIs (links) para as páginas que você está interessado em usar. Isso garantirá que os URIs inseridos nas mensagens de push apontem para os locais corretos. Seu desenvolvedor pode [encontrar mais informações aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/mobile/enabling-deep-links-in-your-app).

>[!MORELIKETHIS]
>
>[Enviar uma Notificação por Push Móvel](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)
