---
unique-page-id: 11376159
description: Antes de criar notificações por push e mensagens no aplicativo - Documentos do Marketo - Documentação do produto
title: Antes de criar notificações por push e mensagens no aplicativo
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Antes de criar notificações por push e mensagens no aplicativo {#before-you-create-push-notifications-and-in-app-messages}

Criar notificações por push e mensagens no aplicativo não é difícil, mas é necessário ter tudo pronto antes de começar. O administrador do Marketo e o desenvolvedor de aplicativos móveis devem seguir as etapas abaixo para preparar as integrações necessárias.

1. Primeiro, o Administrador do Marketo [adiciona um aplicativo móvel](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. O Administrador do Marketo e [envia um trecho de código para o desenvolvedor](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. O desenvolvedor baixa o SDK e inclui o trecho e outros métodos, para [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Por padrão, as mensagens no aplicativo são acionadas quando o aplicativo é aberto. Se você quiser acionar mensagens para outros eventos, como quando uma página específica for exibida ou um botão específico for enviado, o desenvolvedor precisará adicionar eventos personalizados ao código (consulte [Eventos personalizados para mensagens no aplicativo](#CustomEvents) abaixo).

1. O desenvolvedor [gera a chave da API do servidor e o número do projeto para Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [a certificação e senha do iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e o envia para o administrador do Marketo.

1. O Administrador do Marketo configura o acesso à notificação por push [com a chave de API do servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [com o certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>É fácil para um administrador do Marketo verificar se a configuração de push foi verificada. Vá [here](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensagens no aplicativo {#custom-events-for-in-app-messages}

Para mensagens no aplicativo, o acionador de exibição é definido como **Abertura do aplicativo** por padrão. Se quiser usar qualquer evento personalizado para acionar a exibição de mensagens no aplicativo (por exemplo, **Cliques Adicionar ao Carrinho**, **Página Configurações de Exibições**), crie uma lista de eventos desejados e forneça-a ao desenvolvedor de aplicativos móveis. O desenvolvedor adicionará os eventos personalizados ao código. Depois de aprovados, eles são exibidos como acionadores de exibição ao configurar o público-alvo. **Cuidado**: O processo de aprovação de codificação de evento personalizado pode levar algum tempo para ser concluído.

Depois de concluir toda a preparação para mensagens no aplicativo e notificações por push, é hora de começar!

>[!MORELIKETHIS]
>
>* [Criar uma mensagem no aplicativo](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Criar uma notificação por push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

