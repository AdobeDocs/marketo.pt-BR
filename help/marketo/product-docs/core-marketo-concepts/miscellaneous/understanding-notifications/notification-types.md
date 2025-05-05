---
unique-page-id: 2953243
description: Tipos de notificação - Documentação do Marketo - Documentação do produto
title: Tipos de notificação
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 5%

---

# Tipos de notificação {#notification-types}

Há vários tipos de notificação.

## Falha na campanha  {#campaign-failure}

As falhas de campanha notificam você sobre erros em suas campanhas inteligentes.

## Sincronização com CRM {#crm-sync}

As notificações de sincronização do CRM alertam sobre problemas críticos encontrados com a sincronização do CRM, como permissões incorretas ou o fato de a sincronização estar inativa.

**[!DNL Microsoft Dynamics]**

As notificações do Dynamics são enviadas uma vez a cada 24 horas e contêm leads que não foram sincronizados nesse período. Os motivos típicos de falha são leads duplicados (como acima) ou erros de incompatibilidade de comprimento de campo.

![](assets/image2016-1-20-11-3a19-3a58.png)

**[!DNL Salesforce]**

Se você usa o Salesforce, as notificações de erro de sincronização são parecidas com as abaixo. Os erros típicos incluem credenciais expiradas e limites de API excedidos.

![](assets/salesforcesyncerror.png)

## Engajamento {#engagement}

Quando as pessoas ficam exaustas em um riacho, enviamos uma notificação. A notificação inclui o número de pessoas que se exauriram e algumas outras informações.

![](assets/image2014-10-14-10-3a57-3a9.png)

## Facebook {#facebook}

Se você tentar enviar pessoas para a Facebook sem aceitar os Termos de serviço, ou se tentar enviar pessoas para a Facebook após remover o aplicativo Marketo.

## Limpeza de campanha com gatilho ociosa {#idle-trigger-campaign-cleanup}

Desative Campanhas inteligentes acionadas que não recebem mais nenhuma atividade. Saiba mais sobre [limpeza automática da campanha de acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

## LinkedIn {#linkedin}

Quando o Marketo não consegue criar um novo público-alvo, fazer logon ou enviar emails para o LinkedIn após três tentativas.

![](assets/linkedin.png)

## Serviços da Web {#web-services}

Você será notificado quando atingir sua cota diária. A cota é redefinida a cada noite à meia-noite, horário central.

>[!NOTE]
>
>Alguns dos códigos de erro que você pode receber estão descritos em nossa [Documentação do desenvolvedor](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/error-codes).
