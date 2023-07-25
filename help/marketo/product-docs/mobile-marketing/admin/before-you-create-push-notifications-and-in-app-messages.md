---
unique-page-id: 11376159
description: Antes de criar notificações por push e mensagens no aplicativo - Documentação do Marketo - Documentação do produto
title: Antes de criar notificações por push e mensagens no aplicativo
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Antes de criar notificações por push e mensagens no aplicativo {#before-you-create-push-notifications-and-in-app-messages}

Criar notificações por push e mensagens no aplicativo não é difícil, mas você precisa ter tudo pronto antes de começar. O administrador do Marketo e o desenvolvedor do aplicativo móvel devem seguir as etapas abaixo para preparar as integrações necessárias.

1. Primeiro, o administrador do Marketo [adiciona um aplicativo móvel](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. O administrador do Marketo e [envia um trecho de código ao desenvolvedor](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. O desenvolvedor baixa o SDK e inclui o snippet e outros métodos para [Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) ou [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/).

1. Por padrão, as mensagens no aplicativo são acionadas quando o aplicativo é aberto. Se você quiser acionar mensagens para outros eventos, como quando uma determinada página é exibida ou um botão específico é pressionado, o desenvolvedor precisa adicionar eventos personalizados ao código (consulte [Eventos personalizados para mensagens no aplicativo](#CustomEvents) abaixo).

1. O desenvolvedor [gera a chave da API do servidor e o número do projeto para Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/) ou [a certificação e a senha do iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) e o envia para o administrador do Marketo.

1. O administrador do Marketo configura o acesso à notificação por push [com a chave API do servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [com o certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>É fácil para um administrador do Marketo verificar se a configuração de push foi verificada. Basta ir [aqui](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensagens no aplicativo {#custom-events-for-in-app-messages}

Para mensagens no aplicativo, o acionador de exibição é definido como **Abertura do aplicativo** por padrão. Se quiser usar qualquer evento personalizado para acionar a exibição de mensagens no aplicativo (por exemplo, **Cliques Adicionar ao carrinho**, **Página Definições de Views**), crie uma lista de eventos desejados e forneça-a ao desenvolvedor de aplicativos para dispositivos móveis. O desenvolvedor adicionará os eventos personalizados no código. Depois de aprovados, eles são exibidos como acionadores de exibição ao configurar seu público-alvo. **Cuidado**: o processo de aprovação da codificação de eventos personalizados pode levar algum tempo para ser concluído.

Depois de concluir toda a preparação para mensagens no aplicativo e notificações por push, é hora de começar!

>[!MORELIKETHIS]
>
>* [Criar uma mensagem no aplicativo](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Criar uma notificação por push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
