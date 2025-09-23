---
unique-page-id: 14352407
description: Visão geral do canal de entrega - Documentação do Marketo - Documentação do produto
title: Visão geral do canal de entrega
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# Visão geral do canal de entrega {#delivery-channel-overview}

O Marketo [!DNL Sales Connect] oferece várias opções de entrega de emails. Este artigo analisará os canais de entrega que você pode usar, como selecioná-los e quando escolher um em vez do outro.

## Recomendado: Gmail ou [!DNL Exchange] via conexão de email {#recommended-gmail-or-exchange-via-email-connection}

O [!DNL Sales Connect] permite uma configuração simplificada e a capacidade de entrega aprimorada por meio do nosso serviço de Conexão de email. A [!UICONTROL Conexão de Email] permite que cada usuário se conecte à sua conta do [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou do [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) para o [!DNL Sales Connect] para ser usada como o canal de entrega preferido para todos os emails do [!DNL Sales Connect].

O uso do Gmail ou do [!DNL Exchange] apresenta algumas vantagens distintas em relação a outras opções de canal de entrega:

* Esse é um canal de delivery comprovado com reputação estabelecida que ajuda a manter a capacidade de delivery alta.
* Os métodos de autenticação, como SPF e DKIM, já estão configurados e gerenciados pela sua equipe de TI, portanto, não há nenhuma configuração adicional.
* O envio de emails em uma determinada rede de email (ou seja, o envio de um email como um usuário [!DNL Exchange] para uma empresa que recebe emails por meio do [!DNL Exchange]) pode ajudar a aumentar ainda mais a capacidade de entrega.

É importante observar que esses canais de entrega têm seus próprios limites de envio, que são aplicados pela Microsoft e pela Google. Para combater isso, usamos um mecanismo de controle para ajudar os usuários a ficar dentro desses limites. Saiba mais sobre a [limitação de email aqui](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Por padrão, o plug-in O365 sempre usará o canal de entrega do Exchange e o plug-in Gmail sempre usará o canal de entrega do Gmail para enviar emails dos plug-ins.

**Rastreamento de rejeição**: o MSC pode detectar rejeições para [!DNL Exchange Online] ou usuários do Gmail detectando a mensagem de rejeição enviada para a caixa de entrada do remetente. Essas notificações de rejeição serão agrupadas em Análises de modelo, Análises de campanha e Notificações de feed ao vivo para os usuários. O rastreamento de rejeição não é suportado para [!DNL Exchange] clientes locais.

## Canal de entrega personalizado via SMTP {#custom-delivery-channel-via-smtp}

O [!DNL Sales Connect] oferece a opção adicional de conectar um servidor SMTP de terceiros para ser usado como o canal de entrega preferido da sua equipe de vendas.

Usar um provedor SMTP de terceiros é uma ótima opção para equipes de vendas em que o volume de email é a prioridade número um. Provedores de SMTP como o [!DNL Sendgrid] e o [!DNL Sparkpost] são otimizados para atender às necessidades de entrega de emails em massa e podem ser dimensionados para atender às necessidades daqueles que procuram implantar grandes volumes de email.

Além disso, provedores SMTP de terceiros oferecem vários recursos para ajudar a atender às necessidades de capacidade de entrega da sua equipe (como relatórios de entrega de email e endereços IP dedicados), tornando isso uma ótima opção para aqueles que buscam controles mais granulares e visibilidade sobre seu canal de entrega de email de vendas.

## Servidores MSC (Herdados) {#msc-servers-legacy}

Os servidores MSC estão disponíveis apenas para alguns clientes herdados do ToutApp. Esses clientes verão os servidores MSC disponíveis nas configurações de email. Todos os clientes não herdados não verão o MSC como uma opção e deverão conectar sua conta do Gmail ou [!DNL Outlook] ao [!DNL Sales Connect] para desbloquear um canal de entrega.

Os servidores MSC não são compatíveis com os métodos de autenticação DKIM e SPF, o que pode reduzir a taxa de capacidade de delivery. Devido a isso, recomendamos que todos os clientes se conectem ao Gmail ou ao [!DNL Outlook] para obter a melhor capacidade de entrega.

## Servidores Marketo {#marketo-servers}

Os servidores de email da Marketo não se integram com o [!DNL Sales Connect]. Os servidores da Marketo são otimizados para entrega em massa para permitir que eles sejam dimensionados de acordo com as necessidades dos profissionais de marketing. No entanto, o Gmail e o [!DNL Exchange] têm uma taxa de sucesso mais alta para 1:1 comunicação de vendas, razão pela qual recomendamos o uso desses servidores para sua comunicação de vendas.

>[!MORELIKETHIS]
>
>* [Conexão de email para usuários do Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexão de email para [!DNL Outlook] Usuários](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configurando um Canal de Entrega Personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitação da Conexão de Email](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
