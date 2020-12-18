---
unique-page-id: 11376159
description: Antes de criar notificações por push e mensagens no aplicativo - Documentos do Marketing - Documentação do produto
title: Antes de criar notificações por push e mensagens no aplicativo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# Antes de criar notificações por push e mensagens no aplicativo {#before-you-create-push-notifications-and-in-app-messages}

Criar notificações por push e mensagens no aplicativo não é difícil, mas é necessário ter tudo pronto antes de poder start. O Administrador de marketing e o desenvolvedor de aplicativos móveis devem seguir as etapas abaixo para preparar as integrações necessárias.

1. Primeiro, o Administrador de marketing [adiciona um aplicativo móvel](add-a-mobile-app.md)
1. O Administrador do Marketing [envia um trecho de código ao desenvolvedor](send-sdk-code-to-a-developer.md)
1. O desenvolvedor baixa o SDK e inclui snippet e outros métodos para [Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. Por padrão, as mensagens no aplicativo são acionadas quando seu aplicativo é aberto. Se você quiser disparar mensagens para outros eventos, como quando uma página específica é visualizada ou um botão específico é pressionado, o desenvolvedor precisa adicionar eventos personalizados ao código (consulte [Eventos personalizados para mensagens no aplicativo](#CustomEvents) abaixo)
1. O desenvolvedor [gera a chave API do servidor e o número do projeto para Android](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [a certificação e senha para iOS](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e a envia para o Administrador do Marketing
1. O Administrador do Marketo configura o acesso à notificação por push [com a chave API do servidor (Android)](configure-mobile-app-android-push-access.md) ou [com o certificado (iOS)](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>É fácil para um Administrador de marketing verificar se sua configuração de push foi verificada. Basta ir [aqui](verify-push-configuration.md).

## Eventos personalizados para mensagens no aplicativo {#custom-events-for-in-app-messages}

Para mensagens no aplicativo, o acionador de exibição é definido como **App Open** por padrão. Se você quiser usar quaisquer eventos personalizados para acionar a exibição de mensagens no aplicativo (por exemplo, **Cliques em Adicionar ao carrinho**, **Página de configurações do Visualização**), crie uma lista dos eventos desejados e forneça-a ao desenvolvedor de aplicativos móveis. O desenvolvedor adicionará os eventos personalizados ao código. Depois de aprovados, eles aparecem como acionadores de exibição ao configurar sua audiência. **Cuidado**: O processo de aprovação de codificação de eventos personalizado pode levar algum tempo para ser concluído.

Depois de concluir toda a preparação para mensagens no aplicativo e notificações por push, é hora de começar!

>[!MORELIKETHIS]
>
>* [Criar uma mensagem no aplicativo](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [Criar uma notificação por push](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



