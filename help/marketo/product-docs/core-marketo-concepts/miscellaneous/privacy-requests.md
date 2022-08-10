---
description: Solicitações de privacidade - Documentos do Marketo - Documentação do produto
title: Solicitações de privacidade
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: e3f7b0082b77c1be6b4f046838d7ebe725533e78
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Solicitações de privacidade {#privacy-requests}

Este documento fornece uma visão geral do gerenciamento de solicitações individuais de privacidade de dados que você pode enviar para o Marketo Engage por meio da interface do usuário do Privacy Service e da API do Privacy Service.

>[!NOTE]
>
>As solicitações de privacidade enviadas por meio da interface do usuário do Privacy Service ou da API do Marketo Engage aplicam-se somente àquelas que têm as edições Marketo Engage + RT-CDP, B2B e B2P.

Você pode enviar solicitações individuais para acessar e excluir dados do consumidor do Marketo Engage de duas formas:

* Por meio da [Interface do usuário do Privacy Service](https://privacyui.cloud.adobe.io/). Veja a documentação [here](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html){target=&quot;_blank&quot;}.
* Pela API do Privacy Service. Veja a documentação [here](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;} e informações da API [here](https://developer.adobe.com/experience-platform-apis/){target=&quot;_blank&quot;}.

O [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html){target=&quot;_blank&quot;} oferece suporte a dois tipos de solicitações: acesso aos dados e exclusão dos dados.

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

* &quot;Ação&quot;: ou **access** ou **excluir**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **padrão**
   * “Valor”: `<Data Subject’s Email Address>`

&quot;include&quot;:

* **marketo** (que é o Adobe product que se aplica à solicitação)

&quot;regulamento&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** ou **nzpa_nzl**  (que é o regulamento de privacidade que se aplica à solicitação)

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
