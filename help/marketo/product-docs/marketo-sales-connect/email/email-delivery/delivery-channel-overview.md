---
unique-page-id: 14352407
description: Visão geral do canal de delivery - Documentação do Marketo - Documentação do produto
title: Visão geral do canal de delivery
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Visão geral do canal de delivery {#delivery-channel-overview}

O Marketo Sales Connect oferece várias opções para enviar emails. Este artigo analisará os canais de entrega que você pode aproveitar, como selecioná-los e quando escolher um em outro.

## Recomendado: Gmail ou Exchange via conexão de email {#recommended-gmail-or-exchange-via-email-connection}

O Sales Connect permite uma configuração simplificada e o fornecimento aprimorado por meio do nosso serviço de Conexão de email. A Conexão de email permite que cada usuário se conecte a seus [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) conta para Sales Connect para ser usada como canal de delivery preferido para todos os emails do Sales Connect.

A utilização do Gmail ou do Exchange apresenta algumas vantagens distintas em relação a outras opções de canal de delivery:

* Esse é um canal de delivery comprovado com uma reputação estabelecida que ajuda a manter o deliverability alto.
* Métodos de autenticação como SPF e DKIM já são configurados e gerenciados pela equipe de TI, portanto, não há configuração adicional.
* O envio de emails em uma determinada rede de email (ou seja, o envio de um email como usuário do Exchange para uma empresa que recebe emails por meio do Exchange) pode ajudar a aumentar ainda mais a capacidade de entrega.

É importante observar que esses canais de entrega têm seus próprios limites de envio, que são aplicados pelo Microsoft e Google. Para combater isso, utilizamos um mecanismo de controle para ajudar os usuários a se manter dentro desses limites. Saiba mais sobre [limitação de email aqui](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Por padrão, o plug-in O365 sempre usará seu canal de entrega do exchange e o plug-in do Gmail sempre utilizará seu canal de entrega do Gmail para fornecer emails dos plug-ins.

**Rastreamento de rejeição**: O MSC pode detectar rejeições para usuários do Exchange Online ou do Gmail detectando a mensagem de devolução que é enviada para a caixa de entrada do remetente. Essas notificações de devolução serão submetidas a rollup em Análises de modelo, Análises de campanha e Notificações de Feed em tempo real para usuários. O rastreamento de rejeição não é suportado para clientes do Exchange no local.

## Canal de entrega personalizado via SMTP {#custom-delivery-channel-via-smtp}

O Sales Connect oferece a opção adicional de conectar um servidor SMTP de terceiros para ser usado como canal de delivery preferencial da sua equipe de vendas.

Usar um provedor SMTP de terceiros é uma ótima opção para equipes de vendas em que o volume de email é a prioridade número um. Os provedores SMTP, como Sendgrid e Sparkpost, são otimizados para atender às necessidades de delivery de email em massa e podem ser dimensionados para atender às necessidades dos que buscam implantar grandes volumes de email.

Além disso, provedores SMTP de terceiros oferecem uma variedade de recursos para ajudar a atender às necessidades de deliverability de sua equipe (como relatórios de delivery de email e endereços IP dedicados), tornando essa uma ótima opção para aqueles que procuram controles e visibilidade mais granulares em torno de seu canal de delivery de email de vendas.

## Servidores MSC (herdados) {#msc-servers-legacy}

Os servidores da MSC só estão disponíveis para alguns clientes do ToutApp herdado. Esses clientes verão os servidores MSC disponíveis em suas configurações de email. Todos os clientes não herdados não verão o MSC como uma opção e deverão conectar sua conta do Gmail ou Outlook ao Sales Connect para desbloquear um canal de delivery.

Os servidores MSC não são compatíveis com métodos de autenticação DKIM e SPF, o que pode reduzir a taxa de entrega. Devido a isso, recomendamos que todos os clientes se conectem ao Gmail ou ao Outlook para obter a melhor capacidade de delivery.

## Servidores Marketo {#marketo-servers}

Os servidores de email da Marketo não se integram ao Sales Connect. Os servidores da Marketo são otimizados para entrega em massa para permitir que eles sejam dimensionados com as necessidades dos profissionais de marketing. No entanto, o Gmail e o Exchange têm uma taxa de sucesso mais alta para a comunicação de vendas 1:1, razão pela qual recomendamos usar esses servidores para sua comunicação de vendas.

>[!MORELIKETHIS]
>
>* [Conexão de email para usuários do Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexão de email para usuários do Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configuração de um canal de delivery personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitação da conexão de email](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

