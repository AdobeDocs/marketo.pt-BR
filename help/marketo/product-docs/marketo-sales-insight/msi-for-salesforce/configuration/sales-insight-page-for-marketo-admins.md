---
unique-page-id: 42762409
description: Página de insights de vendas para administradores do Marketo - Documentação do Marketo - Documentação do produto
title: Página de insights de vendas para administradores do Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 3%

---

# Página de insights de vendas para administradores do Marketo {#sales-insight-page-for-marketo-admins}

Os administradores do Marketo têm determinados privilégios no Sales Insight. Saiba o que eles estão abaixo.

## Configuração da API Soap {#soap-api-configuration}

Essas credenciais são usadas para conectar sua conta do Salesforce à sua instância do Marketo, para usar o MSI no Salesforce.

![](assets/one-1.png)

## Configuração da API Rest {#rest-api-configuration}

Essas credenciais são usadas para conectar sua conta do Salesforce à sua instância do Marketo, a fim de usar o Painel de insights do MSI no Salesforce.

![](assets/two-1.png)

## Configurações de pontuação de pessoa {#person-score-settings}

* **Estrelas**: as estrelas representam a pontuação total do lead em comparação a outros leads.
* **Chamas**: As chamas representam a urgência - o quanto a pontuação de um lead mudou recentemente.

Por padrão, o Marketo Sales Insight usa o campo Pontuação de lead para calcular estrelas e chamas. Mas se você quiser escolher um campo diferente, veja como:

1. No **Admin** da Marketo, clique em **Sales Insight**.

   ![](assets/four.png)

1. Em Configurações de pontuação de lead, clique em **Editar**.

   ![](assets/five.png)

1. Selecione o campo que deseja usar para estrelas.

   ![](assets/six.png)

1. Selecione o campo que deseja usar para as chamas.

   ![](assets/seven.png)

1. Clique em **Salvar**. O Sales Insight levará algum tempo para ser recalculado. Você pode verificar seu CRM mais tarde para ver as estrelas e as chamas.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se você ainda não tiver seus campos de pontuação personalizados, veja como [criar](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Estrelas e chamas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Configurações {#settings}

![](assets/nine.png)

**Configurações de cancelamento de inscrição:**

Você pode escolher entre as seguintes configurações de cancelamento de inscrição para emails sem modelo, padrão e operacionais

* Respeitar Configuração De Cancelamento De Inscrição
* Respeitar as configurações de cancelamento de inscrição quando houver mais de 1 destinatário
* Respeitar as configurações de cancelamento de inscrição quando houver mais de 5 destinatários
* Ignorar configurações de cancelamento de inscrição

**Ativar possibilidade de bloquear modelos:**

Quando ativados, os usuários MSI não poderão editar modelos ao enviar emails do Salesforce

**Ativar feed RSS:**

Quando ativado, os usuários do MSI podem visualizar seu feed de lead em um feed RSS (além do feed de lead no Salesforce). O RSS feed só poderá funcionar se o recurso &quot;Expiração do token&quot; estiver desativado.

**Expiração do token:**

A expiração do token é controlada no Gerenciador de recursos. Para ativá-la/desativá-la, entre em contato com [Suporte ao Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Quando ativado, todos os tokens do Marketo expiram em 10 minutos. Quando desativados, os tokens do Marketo não expiram.

Os tokens gerados antes da ativação da Expiração do token não terão um tempo de expiração para validação, portanto, não expirarão mesmo se o recurso estiver ativado no momento.

Os tokens gerados após a ativação da Expiração do token terão um tempo de expiração de 10 minutos, portanto, eles ainda expirarão em 10 minutos, mesmo depois que o recurso for desativado.

O comportamento do token será baseado em quando ele foi gerado (quando o recurso de Expiração do token foi ativado/desativado, em vez do status atual do recurso).
