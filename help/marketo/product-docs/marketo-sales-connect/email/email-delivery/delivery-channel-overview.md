---
unique-page-id: 14352407
description: Visão geral do Canal do delivery - Documentos do Marketing - Documentação do produto
title: Visão geral do Canal do delivery
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Visão geral do Canal do delivery {#delivery-channel-overview}

Analisaremos os três canais diferentes que você pode aproveitar, como selecioná-los, quando escolher um sobre o outro e as nuances ao seu redor.

>[!NOTE]
>
>Essas informações só são relevantes se você estiver enviando seus emails do aplicativo [da](http://toutapp.com/login)Web. Se você estiver usando o Sales Connect no Gmail ou Outlook, seus e-mails serão entregues por meio desses servidores de e-mail.

## Servidores de e-mail MSC (padrão) {#msc-email-servers-default}

Por padrão, esse método será selecionado para o delivery de seus emails. Os servidores de email MSC são uma excelente opção para usuários que não usam o Gmail ou o Outlook. Além disso, como eles são nossos servidores, temos a capacidade de receber mensagens de erro relacionadas a rejeições ou delivery com falha e de exibi-las até você na seção &quot;Delivery com falha&quot; da guia Conversações.

Outro benefício de usar os servidores MSC é que, ao usar uma Identidade [de](https://help.toutapp.com/hc/en-us/articles/215371427)email, o recipient visualizará o endereço de email da identidade que você criou.

Ao usar servidores MSC, seus recipient podem ver uma tag &quot;via toutapp.com&quot;. Esse é o cliente de e-mail deles informando que o e-mail foi enviado usando o Sales Connect.

Para obter mais detalhes, consulte este artigo [da Ajuda do](https://support.google.com/mail/answer/1311182?hl=en)Gmail.

>[!NOTE]
>
>Nossos servidores MSC não têm um registro [](https://dmarc.org/) DMARC disponibilizado. Eles não podem ser listados em whitelist em seus próprios servidores.

## Servidor Gmail {#gmail-server}

Se seu provedor de e-mail do empresa for Gmail, você poderá aproveitar sua conta existente para enviar seus e-mails do Sales Connect. Essa é uma excelente opção se você quiser evitar as informações &quot;via toutapp.com&quot; e se preferir confiar na reputação do domínio de empresa e na capacidade de entrega. Uma vantagem adicional de usar um servidor Gmail é que qualquer coisa que você enviar do aplicativo da Web será automaticamente adicionada à sua pasta Gmail enviada.

Só é possível nos conectar corretamente com uma única conta do Gmail (um endereço de email) que entregará seus emails do Sales Connect. Isso significa que, se você usar várias identidades de email, somente o endereço da conta à qual estamos conectados aparecerá ao observar os detalhes.

No aplicativo da Web, sua identidade será exibida conforme você a criou (acima). No entanto, enviar por meio de servidores Gmail mostrará o endereço da conta conectada.

>[!NOTE]
>
>Como o Sales Connect não gerencia diretamente seus servidores Gmail, não gravamos eventos de email ocultos no aplicativo da Web.

## Servidor SMTP Personalizado  {#custom-smtp-server}

Pague pelo seu próprio servidor? Usar um ambiente do Microsoft Exchange? Esta é uma opção para você. Confira [estas instruções](http://docs.marketo.com/x/zYTS) sobre como configurar. Como os servidores Gmail, como o Sales Connect não gerencia diretamente seu servidor, não gravamos eventos de email ocultos no aplicativo da Web.

