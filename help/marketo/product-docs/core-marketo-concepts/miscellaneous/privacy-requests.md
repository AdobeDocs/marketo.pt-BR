---
description: Solicitações de privacidade - Documentação do Marketo - Documentação do produto
title: Solicitações de privacidade
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 0abb315be0f9cb5f42fa41d72b446de8c2f62c1e
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Solicitações de privacidade {#privacy-requests}

Este documento fornece uma visão geral do gerenciamento de solicitações individuais de privacidade de dados que você pode enviar para o Marketo Engage por meio da interface do usuário do Privacy Service e da API Privacy Service.

>[!NOTE]
>
>As solicitações de privacidade enviadas por meio da interface do usuário ou da API do Privacy Service para Marketo Engage se aplicam apenas ao seguinte:
>
>* Usuários do Marketo Engage que integraram ao sistema Adobe Identity Management
>
>**-ou-**
>
>* Usuários de Marketo Engage que utilizam outro produto de Experience Cloud que já está no sistema Adobe Identity Management (por exemplo, RT-CDP, edições B2B e B2P, Audience Manager).

Você pode enviar solicitações individuais para acessar e excluir dados do consumidor do Marketo Engage de duas maneiras:

* Por meio da [interface do Privacy Service](https://privacyui.cloud.adobe.io/). Consulte a documentação [aqui](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=pt-BR){target="_blank"}.
* Por meio da API de Privacy Service. Consulte a documentação [aqui](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} e as informações sobre a API [aqui](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

O [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=pt-BR){target="_blank"} dá suporte a dois tipos de solicitações: acesso e exclusão de dados.

Saiba como criar solicitações de Acesso e Exclusão.

## Configuração necessária para enviar solicitações para Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Para fazer solicitações de Acesso e Exclusão de dados para o Marketo Engage, você deve:

1. Identifique o seguinte:

   a. ID da Organização IMS<br/>
b. Endereço de e-mail da pessoa sobre a qual deseja agir

   Uma ID de organização IMS é uma sequência de 24 caracteres alfanuméricos anexada com @AdobeOrg. Se a sua equipe de marketing ou o administrador interno do sistema Adobe não souber a ID de organização IMS, entre em contato com o Atendimento ao cliente da Adobe em `gdprsupport@adobe.com`. Você precisa da ID de organização IMS para enviar solicitações à API de privacidade.

1. No Privacy Service, você pode enviar solicitações de Acesso e Exclusão ao Marketo Engage e verificar o status das solicitações existentes.

## Valores de campo obrigatórios em solicitações JSON do Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: `<Your IMS Org ID Value>`

&quot;users&quot;:

* &quot;ação&quot;: **acessar** ou **excluir**
* &quot;userIDs&quot;
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * &quot;value&quot;: `<Data Subject's Email Address>`

&quot;include&quot;:

* **marketo** (que é o produto do Adobe que se aplica à solicitação)

&quot;Regulamentação&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** ou **nzpa_nzl** (que é o regulamento de privacidade que se aplica à solicitação)

## Exemplo um: solicitação de exclusão do GDPR {#gdpr-delete-request}

Solicitação JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

Resposta JSON

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## Exemplo dois: solicitação de acesso ao CCPA {#ccpa-access-request}

Solicitação JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

Resposta JSON

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

>[!MORELIKETHIS]
>
>[Gerenciamento de privacidade](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
