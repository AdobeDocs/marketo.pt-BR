---
unique-page-id: 2953243
description: Tipos de notificação - Documentos do Marketing - Documentação do produto
title: Tipos de notificação
translation-type: tm+mt
source-git-commit: e5050328cbddaf072dd60ddd8d7363a704e720b5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Tipos de notificação {#notification-types}

Há vários tipos de notificação.

## Falha de campanha {#campaign-failure}

As falhas de campanha notificam você de erros em suas campanhas inteligentes.

## Sincronização do CRM {#crm-sync}

As notificações de sincronização do CRM alertam para problemas críticos encontrados com a sincronização do CRM, como permissões incorretas ou a sincronização que está sendo desativada.

**Microsoft Dynamics**

As notificações dinâmicas são enviadas uma vez a cada 24 horas e contêm clientes potenciais que falharam na sincronização nesse período. Os motivos típicos para falha são erros de incompatibilidade de duplicado (como acima) ou de comprimento de campo.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Se você usar o Salesforce, as notificações de erro de sincronização se assemelharão às que estão abaixo. Os erros típicos incluem credenciais expiradas e limites de API excedidos.

![](assets/salesforcesyncerror.png)

Envolvimento

Quando os clientes potenciais se exaurem em um fluxo, nós enviamos uma notificação.  A notificação inclui o número de clientes potenciais que se esgotaram e outras informações.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Se você tentar enviar clientes potenciais para o Facebook sem aceitar os Termos de serviço, ou se tentar enviar clientes potenciais para o Facebook após remover o aplicativo Marketo.

Limpeza da Campanha do acionador ocioso

Desative Campanhas inteligentes acionadas que não têm mais atividade. Saiba mais sobre [limpeza automática de campanha de disparo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

Quando o Marketo não puder criar uma nova audiência, fazer logon ou enviar emails para o LinkedIn após três tentativas.

![](assets/linkedin.png)

Serviços Web

Você será notificado quando atingir sua cota diária. A cota é redefinida todas as noites à meia-noite, Hora Central.

>[!NOTE]
>
>Alguns dos códigos de erro que você pode receber estão descritos em nossa [Documentação do desenvolvedor](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
