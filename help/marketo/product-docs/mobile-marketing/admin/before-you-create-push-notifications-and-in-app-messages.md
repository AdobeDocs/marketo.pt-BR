---
unique-page-id: 11376159
description: Antes de criar notificações por push e mensagens no aplicativo - Documentação do Marketo - Documentação do produto
title: Antes de criar notificações por push e mensagens no aplicativo
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Antes de criar notificações por push e mensagens no aplicativo {#before-you-create-push-notifications-and-in-app-messages}

Criar notificações por push e mensagens no aplicativo não é difícil, mas você precisa ter tudo pronto antes de começar. O administrador do Marketo e o desenvolvedor do aplicativo móvel devem seguir as etapas abaixo para preparar as integrações necessárias.

1. Primeiro, o Administrador do Marketo [adiciona um aplicativo móvel](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md).

1. O Administrador do Marketo [envia um trecho de código para o desenvolvedor](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md).

1. O desenvolvedor baixa o SDK e inclui o trecho e outros métodos para [Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) ou [iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios).

1. Por padrão, as mensagens no aplicativo são acionadas quando o aplicativo é aberto. Se você quiser acionar mensagens para outros eventos, como quando uma determinada página é exibida ou um botão específico é pressionado, o desenvolvedor precisa adicionar eventos personalizados ao código (consulte [Eventos personalizados para mensagens no aplicativo](#CustomEvents) abaixo).

1. O desenvolvedor [gera a chave de API do Servidor e o número do projeto para o Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) ou [a certificação e a senha para o iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios) e a envia para o Administrador do Marketo.

1. O Administrador do Marketo configura o acesso à notificação por push [com a Chave de API do Servidor (Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) ou [com o certificado (iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md).

>[!TIP]
>
>É fácil para um administrador do Marketo verificar se a configuração de push foi verificada. Basta ir [aqui](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md).

## Eventos personalizados para mensagens no aplicativo {#custom-events-for-in-app-messages}

Para mensagens no aplicativo, o acionador de exibição está definido como **Aberto no Aplicativo** por padrão. Se você quiser usar qualquer evento personalizado para acionar a exibição de mensagens no aplicativo (por exemplo, **Cliques, Adicionar ao carrinho**, **Página Configurações de exibição**), crie uma lista de eventos desejados e forneça-a ao desenvolvedor de aplicativos para dispositivos móveis. O desenvolvedor adicionará os eventos personalizados no código. Depois de aprovados, eles são exibidos como acionadores de exibição ao configurar seu público-alvo. **Cuidado**: o processo de aprovação da codificação de eventos personalizada pode levar algum tempo para ser concluído.

Depois de concluir toda a preparação para mensagens no aplicativo e notificações por push, é hora de começar!

>[!MORELIKETHIS]
>
>* [Criar uma mensagem no aplicativo](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [Criar uma Notificação por Push](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
