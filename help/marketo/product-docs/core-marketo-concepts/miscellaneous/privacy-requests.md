---
description: Solicitações de privacidade - Documentos do Marketo - Documentação do produto
title: Solicitações de privacidade
source-git-commit: 17e68ea00647dbfd98fde94827eb300804944511
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Solicitações de privacidade {#privacy-requests}

Este documento fornece uma visão geral do gerenciamento de solicitações individuais de privacidade de dados que você pode enviar para o Marketo Engage por meio da interface do usuário do Privacy Service e do **API Privacy Service**.

Você pode enviar solicitações individuais para acessar e excluir dados do consumidor do Marketo Engage de duas formas:

* Por meio da [Interface do usuário do Privacy Service](https://privacyui.cloud.adobe.io/). Veja a documentação [here](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_ui_tutorial.md).
* Por meio da **API Privacy Service**. Veja a documentação [here](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_api_tutorial.md) e a referência da API [here](https://www.adobe.io/apis/experiencecloud/gdpr/api-reference.html#!acpdr/swagger-specs/privacy-service.yaml).

O [Privacy Service](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html) O suporta dois tipos de solicitações: acesso aos dados e exclusão dos dados.

Observação: As solicitações de privacidade enviadas por meio da interface do usuário do Privacy Service ou da API do Marketo Engage aplicam-se somente aos clientes que têm as edições Marketo Engage + RT-CDP, B2B e B2P.

Vamos ver como criar solicitações de acesso e exclusão.

## Configuração necessária para enviar solicitações para o Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Para fazer solicitações de acesso e exclusão de dados para o Marketo Engage, você deve:

1. Identifique o seguinte:

   a. ID organizacional IMS<br/>
b. Endereço de email da pessoa em quem você deseja agir

   Uma ID de organização IMS é uma sequência de 24 caracteres alfanuméricos anexada com @AdobeOrg. Se a sua equipe de marketing ou o administrador interno do sistema do Adobe não souber a ID de organização IMS, entre em contato com o Atendimento ao cliente da Adobe em gdprsupport@adobe.com. Você precisa da ID de organização IMS para enviar solicitações à API de privacidade.

1. No Privacy Service, você pode enviar solicitações de Acesso e Exclusão para o Marketo Engage e verificar o status das solicitações existentes.

## Valores de campo obrigatórios em solicitações Marketo Engage JSON {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* “Valor”: `<Your IMS Org ID Value>`

“usuários”:

* &quot;key&quot;: `<Your Request Tracking Key>`   (opcional)
* &quot;Ação&quot;: ou **access** ou **excluir**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **padrão**
   * “Valor”: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** (que é o Adobe product que se aplica à solicitação)

&quot;regulamento&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd** ou **nzpa**  (que é o regulamento sobre privacidade que se aplica à solicitação)

## Exemplo Um: Solicitação de exclusão do RGPD {#gdpr-delete-request}

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
      "key": "AAGDPRO1", 
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
          "key": "AAGDPRO1",
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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

## Exemplo dois: Solicitação de acesso à CCPA {#ccpa-access-request}

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
      "key": "AAGDPRO1",
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
      "jobId": " 3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
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
