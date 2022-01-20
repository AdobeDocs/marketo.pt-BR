---
unique-page-id: 42762409
description: Página de informações de vendas para administradores da Marketo - Documentos da Marketo - Documentação do produto
title: Página de informações de vendas para administradores do Marketo
exl-id: d98bc9d8-1a72-405f-b1d7-b71ad88c8493
source-git-commit: 5812f447fbe22bee13060afae8408de7ca7384e5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 3%

---

# Página de informações de vendas para administradores do Marketo {#sales-insight-page-for-marketo-admins}

Os administradores da Marketo têm determinados privilégios no Sales Insight. Saiba o que estão abaixo.

## Configuração da API Soap {#soap-api-configuration}

Essas credenciais são usadas para conectar sua conta do Salesforce à instância do Marketo, para usar o MSI no Salesforce.

![](assets/one-1.png)

## Configuração da API Restante {#rest-api-configuration}

Essas credenciais são usadas para conectar sua conta do Salesforce à instância do Marketo, para usar o Painel do MSI Insights no Salesforce.

![](assets/two-1.png)

## Configurações de pontuação da pessoa {#person-score-settings}

* **Estrelas**: As estrelas representam a pontuação de lead total em comparação a outros leads.
* **Chama**: As chamas representam urgência - quanto a pontuação de um cliente potencial mudou recentemente.

Por padrão, o Marketo Sales Insight usa o campo Pontuação de lead para calcular estrelas e chamas. Mas se você quiser escolher um campo diferente, veja como:

1. No **Administrador** área do Marketo, clique em **Insight de vendas**.

   ![](assets/four.png)

1. Em Configurações de pontuação de lead , clique em **Editar**.

   ![](assets/five.png)

1. Selecione o campo que deseja usar para estrelas.

   ![](assets/six.png)

1. Selecione o campo que deseja usar para as chamas.

   ![](assets/seven.png)

1. Clique em **Salvar**. O insight de vendas levará algum tempo para ser recalculado. Você pode verificar seu CRM posteriormente para ver as estrelas e as chamas.

   ![](assets/eight.png)

   >[!TIP]
   >
   >Se você ainda não tiver seus campos de pontuação personalizados, veja a seguir como [criá-los](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

   >[!MORELIKETHIS]
   >
   >[Estrelas e chamas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md)

## Configurações {#settings}

![](assets/nine.png)

**Configurações de cancelamento de inscrição:**

Você pode escolher entre as seguintes configurações de cancelamento de inscrição para Sem modelo, Emails padrão e emails operacionais

* Respeitar configuração de cancelamento de assinatura
* Respeitar configurações de cancelamento de inscrição quando mais de 1 destinatário
* Respeitar configurações de cancelamento de inscrição quando mais de 5 recipients
* Ignorar configurações de cancelamento de inscrição

**Ativar possibilidade de bloquear modelos:**

Quando ativado, os usuários do MSI não poderão editar modelos ao enviar emails do Salesforce

**Ativar feed RSS:**

Quando ativados, os usuários do MSI podem visualizar seu Feed de lead em um feed RSS (além do Feed de lead no Salesforce). O feed RSS só poderá funcionar se o recurso &quot;Expiração do token&quot; estiver desativado.

**Expiração do token:**

A Expiração de token é controlada no Gerenciador de recursos. Para ativá-lo/desativá-lo, entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Quando ativados, todos os tokens do Marketo expiram em 10 minutos. Quando desativados, os tokens do Marketo não expirarão.

Os tokens gerados antes de habilitar a Expiração do token não terão um tempo de expiração para validar, portanto, não expirarão mesmo se o recurso estiver habilitado no momento.

Os tokens gerados após a ativação da Expiração do token terão um tempo de expiração de 10 minutos, portanto, ainda expirarão em 10 minutos mesmo depois que o recurso for desativado.

O comportamento do token será baseado no momento em que foi gerado (quando o recurso Expiração do token foi ativado/desativado, em vez do status do recurso atual).
