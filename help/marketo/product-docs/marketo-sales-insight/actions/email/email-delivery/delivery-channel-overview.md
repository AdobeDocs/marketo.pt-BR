---
description: Visão geral do canal de entrega - Documentação do Marketo - Documentação do produto
title: Visão geral do canal de entrega
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Visão geral do canal de entrega {#delivery-channel-overview}

O Marketo Sales oferece várias opções para enviar emails. Este artigo analisará os canais de entrega que você pode usar, como selecioná-los e quando escolher um em vez do outro.

## Recomendado: Gmail ou Exchange via conexão de email {#recommended-gmail-or-exchange-via-email-connection}

O Marketo Sales permite uma configuração simplificada e a capacidade aprimorada de delivery por meio do serviço de conexão de email. A conexão de email permite que cada usuário se conecte à sua conta do [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) ou do [[!DNL Exchange]](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) para o Marketo Sales para ser utilizada como o canal de entrega preferido para todos os emails de Vendas do Marketo.

O uso do Gmail ou do [!DNL Exchange] apresenta algumas vantagens distintas em relação a outras opções de canal de entrega:

* Esse é um canal de delivery comprovado com reputação estabelecida que ajuda a manter a capacidade de delivery alta.
* Os métodos de autenticação, como SPF e DKIM, já estão configurados e gerenciados pela sua equipe de TI, portanto, não há nenhuma configuração adicional.
* O envio de emails em uma determinada rede de email (ou seja, o envio de um email como um usuário [!DNL Exchange] para uma empresa que recebe emails por meio do [!DNL Exchange]) pode ajudar a aumentar ainda mais a capacidade de entrega.

É importante observar que esses canais de entrega têm seus próprios limites de envio, que são aplicados pela Microsoft e pela Google. Para combater isso, usamos um mecanismo de controle para ajudar os usuários a ficar dentro desses limites. Saiba mais sobre a [limitação de email aqui](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Por padrão, o plug-in O365 sempre usará o canal de entrega do Exchange e o plug-in Gmail sempre usará o canal de entrega do Gmail para enviar emails dos plug-ins.

**Rastreamento de Rejeição**: o Marketo Sales pode detectar rejeições de usuários do Exchange Online ou do Gmail detectando a mensagem de rejeição enviada para a caixa de entrada do remetente. Essas notificações de rejeição serão agrupadas em Análises de modelo, Análises de campanha e Notificações de feed ao vivo para os usuários. O rastreamento de rejeição não é compatível com clientes locais do Exchange.

## Canal de entrega personalizado via SMTP {#custom-delivery-channel-via-smtp}

O Marketo Sales oferece a opção adicional de conectar um servidor SMTP de terceiros para ser usado como canal de entrega preferido da sua equipe de vendas.

Usar um provedor SMTP de terceiros é uma ótima opção para equipes de vendas em que o volume de email é a prioridade número um. Os provedores SMTP, como Sendgrid e Sparkpost, são otimizados para atender às necessidades de delivery de email em massa e podem ser dimensionados para atender às necessidades daqueles que procuram implantar grandes volumes de email.

Além disso, provedores SMTP de terceiros oferecem vários recursos para ajudar a atender às necessidades de capacidade de entrega da sua equipe (como relatórios de entrega de email e endereços IP dedicados), tornando isso uma ótima opção para aqueles que buscam controles mais granulares e visibilidade sobre seu canal de entrega de email de vendas.

## Servidores de vendas da Marketo (herdados) {#marketo-sales-servers-legacy}

Os servidores de vendas da Marketo só estão disponíveis para alguns clientes herdados do ToutApp. Esses clientes verão os servidores de vendas da Marketo disponíveis nas configurações de email. Todos os clientes não herdados não verão o Marketo Sales como uma opção e deverão conectar sua conta do Gmail ou [!DNL Outlook] ao Marketo Sales para desbloquear um canal de entrega.

Os servidores do Marketo Sales não suportam os métodos de autenticação DKIM e SPF, o que pode reduzir a taxa de capacidade de delivery. Devido a isso, recomendamos que todos os clientes se conectem ao Gmail ou ao [!DNL Outlook] para obter a melhor capacidade de entrega.

## Servidores MSC (Herdados) {#msc-servers-legacy}

Os servidores MSC estão disponíveis apenas para alguns clientes herdados do ToutApp. Esses clientes verão os servidores MSC disponíveis nas configurações de email. Todos os clientes não herdados não verão o MSC como uma opção e deverão conectar sua conta do Gmail ou Outlook ao Sales Connect para desbloquear um canal de entrega.

Os servidores MSC não são compatíveis com os métodos de autenticação DKIM e SPF, o que pode reduzir a taxa de capacidade de delivery. Devido a isso, recomendamos que todos os clientes se conectem ao Gmail ou ao [!DNL Outlook] para obter a melhor capacidade de entrega.

## Servidores Marketo {#marketo-servers}

Os servidores de e-mail da Marketo não se integram ao Marketo Sales. Os servidores da Marketo são otimizados para entrega em massa para permitir que eles sejam dimensionados de acordo com as necessidades dos profissionais de marketing. No entanto, o Gmail e o [!DNL Exchange] têm uma taxa de sucesso mais alta para 1:1 comunicação de vendas, razão pela qual recomendamos o uso desses servidores para sua comunicação de vendas.

>[!MORELIKETHIS]
>
>* [Conexão de email para usuários do Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexão de email para [!DNL Outlook] Usuários](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configurando um Canal de Entrega Personalizado](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitação da Conexão de Email](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
