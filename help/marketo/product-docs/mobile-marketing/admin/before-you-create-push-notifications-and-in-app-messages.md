---
unique-page-id: 11376159
description: Antes de criar notificações por push e mensagens no aplicativo - Documentos do Marketing - Documentação do produto
title: Antes de criar notificações por push e mensagens no aplicativo
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# Antes de criar notificações por push e mensagens no aplicativo {#before-you-create-push-notifications-and-in-app-messages}

Criar notificações por push e mensagens no aplicativo não é difícil, mas é necessário ter tudo pronto antes de poder start. O Administrador de marketing e o desenvolvedor de aplicativos móveis devem seguir as etapas abaixo para preparar as integrações necessárias.

1. Primeiro, o Administrador de marketing [adiciona um aplicativo móvel](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. Em seguida, o Administrador de marketing [envia um trecho de código para o desenvolvedor](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. O desenvolvedor baixa o SDK e inclui snippet e outros métodos para [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Por padrão, as mensagens no aplicativo são acionadas quando seu aplicativo é aberto. Se você quiser disparar mensagens para outros eventos, como quando uma página específica é visualizada ou um botão específico é pressionado, o desenvolvedor precisa adicionar eventos personalizados ao código (consulte [Eventos personalizados para mensagens no aplicativo](#CustomEvents) abaixo).

1. O desenvolvedor [gera a chave da API do servidor e o número do projeto para Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [a certificação e senha para iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e a envia para o Administrador de marketing.

1. O Administrador de marketing configura o acesso à notificação por push [com a chave API do servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [com o certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>É fácil para um Administrador de marketing verificar se sua configuração de push foi verificada. Basta ir [aqui](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensagens no aplicativo {#custom-events-for-in-app-messages}

Para mensagens no aplicativo, o acionador de exibição é definido como **App Open** por padrão. Se você quiser usar quaisquer eventos personalizados para acionar a exibição de mensagens no aplicativo (por exemplo, **Cliques em Adicionar ao carrinho**, **Página de configurações do Visualização**), crie uma lista dos eventos desejados e forneça-a ao desenvolvedor de aplicativos móveis. O desenvolvedor adicionará os eventos personalizados ao código. Depois de aprovados, eles aparecem como acionadores de exibição ao configurar sua audiência. **Cuidado**: O processo de aprovação de codificação de eventos personalizado pode levar algum tempo para ser concluído.

Depois de concluir toda a preparação para mensagens no aplicativo e notificações por push, é hora de começar!

>[!MORELIKETHIS]
>
>* [Criar uma mensagem no aplicativo](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
   >
   >
* [Criar uma notificação por push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

