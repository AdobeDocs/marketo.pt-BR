---
unique-page-id: 42762409
description: Página de insight de vendas para administradores de marketing - Documentos de marketing - Documentação do produto
title: Página de insight de vendas para administradores de marketing
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---


# Página de insight de vendas para administradores de marketing {#sales-insight-page-for-marketo-admins}

Os administradores de marketing têm certos privilégios no Sales Insight. Saiba o que eles estão abaixo.

## Configuração da API Soap {#soap-api-configuration}

Essas credenciais são usadas para conectar sua conta do Salesforce à sua instância do Marketo, a fim de usar o MSI no Salesforce.

![](assets/one-1.png)

## Restaurar configuração da API {#rest-api-configuration}

Essas credenciais são usadas para conectar sua conta do Salesforce à sua instância do Marketo, a fim de usar o Painel MSI Insights no Salesforce.

![](assets/two-1.png)

Você pode optar por remover as credenciais da Rest API no SFDC e usar somente as APIs Soap. Isso desativará o Painel Insights

![](assets/three-1.png)

## Configurações da pontuação da pessoa {#person-score-settings}

| **Estrelas:** | As estrelas representam a pontuação total de chumbo em comparação a outros clientes potenciais. |
|---|---|
| **Chamas:** | As chamas representam a urgência - quanto a pontuação de um cliente potencial mudou recentemente. |

Por padrão, o Marketing Cloud Sales Insight usa o campo Pontuação principal para calcular estrelas e chamas. Mas se você quiser escolher um campo diferente, veja como:

1. Na área **Admin** do Marketing, clique em **Sales Insight**.

   ![](assets/four.png)

1. Em Configurações de Pontuação de Cliente Potencial, clique em **Editar**.

   ![](assets/five.png)

1. Selecione o campo que deseja usar para estrelas.

   ![](assets/six.png)

1. Selecione o campo que deseja usar para as chamas.

   ![](assets/seven.png)

1. Clique em **Salvar**. O insight de vendas levará algum tempo para recalcular. Você pode verificar seu CRM mais tarde para ver as estrelas e as chamas.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se você ainda não tiver seus campos de pontuação personalizados, veja como [criá-los](http://docs.marketo.com/x/3wMk).

   >[!NOTE]
   >
   >**Artigos relacionados**
   >
   >
   >[Estrelas e chamas](http://docs.marketo.com/x/qgU6Ag)

## Configurações {#settings}

![](assets/nine.png)

**Configurações de cancelamento de assinatura: **

Você pode escolher entre as seguintes configurações de cancelamento de inscrição para Sem modelo, e-mails padrão e e e-mails operacionais

* Respeitar configuração de cancelamento de assinatura
* Respeitar configurações de cancelamento de inscrição quando mais de 1 recipient
* Respeitar configurações de cancelamento de inscrição quando mais de 5 recipient
* Ignorar configurações de cancelamento de inscrição

**Habilitar a capacidade de bloquear modelos: **

Quando ativados, os usuários MSI não poderão editar modelos ao enviar emails do Salesforce

**Ativar feed RSS:**

Quando ativados, os usuários MSI podem visualização seus Feed de cliente potencial em um feed RSS (além do Feed de cliente potencial no Salesforce)**.**
