---
unique-page-id: 2953243
description: Tipos de notificação - Documentos do Marketo - Documentação do produto
title: Tipos de notificação
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 6%

---

# Tipos de notificação {#notification-types}

Há vários tipos de notificação.

## Falha na campanha  {#campaign-failure}

As falhas da campanha notificam você sobre erros em suas campanhas inteligentes.

## Sincronização com CRM {#crm-sync}

As notificações de sincronização do CRM alertam você sobre problemas críticos encontrados com a sincronização do CRM, como permissões incorretas ou a sincronização que está sendo desativada.

**Microsoft Dynamics**

As notificações do Dynamics são enviadas uma vez a cada 24 horas e contêm leads que falharam na sincronização nesse período de tempo. Os motivos típicos para falha são erros duplicados de lead (como acima) ou incompatibilidade de comprimento de campo.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Se você usar o Salesforce, as notificações de erro de sincronização serão semelhantes às abaixo. Erros típicos incluem credenciais expiradas e limites de API excedidos.

![](assets/salesforcesyncerror.png)

Envolvimento

Quando os leads se esgotam em um fluxo, enviamos uma notificação.  A notificação inclui o número de clientes potenciais que se esgotaram e algumas outras informações.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Se você tentar enviar leads para a Facebook sem aceitar os Termos de serviço, ou se tentar enviar leads para a Facebook após remover o aplicativo Marketo.

Limpeza de campanha com gatilho ociosa

Desative as Campanhas inteligentes acionadas que não têm mais atividade. Saiba mais sobre [limpeza automática de campanha de acionamento](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

Quando o Marketo não puder criar um novo público-alvo, fazer logon ou enviar emails para o LinkedIn após três tentativas.

![](assets/linkedin.png)

Serviços da Web

Você será notificado quando atingir sua cota diária. A cota é redefinida todas as noites à meia-noite, horário central.

>[!NOTE]
>
>Alguns dos códigos de erro que você pode receber são descritos em nossa [Documentação do desenvolvedor](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
