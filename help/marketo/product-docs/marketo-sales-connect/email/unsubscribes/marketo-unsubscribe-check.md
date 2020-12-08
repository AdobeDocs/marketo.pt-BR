---
unique-page-id: 18317340
description: Marketo Unsubscribe Check - Marketing to Docs - Documentação do produto
title: Marketo Unsubscrition Check
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Marketo Unsubscrition Check {#marketo-unsubscribe-check}

A verificação de cancelamento de inscrição do Marketo usa a conexão da sua equipe com o Marketo para impedir que emails sejam enviados para pessoas que não se inscrevem no sistema de gerenciamento de clientes potenciais do Marketo. Quando um usuário de vendas envia um email com o Sales Connect, uma chamada de API é feita para o Marketo para verificar se a ID do email está cancelada. Se estiver, impediremos o envio do email.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Ligar {#turning-it-on}

1. No aplicativo da Web, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one-2.png)

1. Em Configurações administrativas, clique em **Cancelar inscrição**.

   ![](assets/two-3.png)

1. Clique em **Integrações**.

   ![](assets/three-3.png)

1. Na seção Marketo Unsubscribe Check (Cancelar inscrição de marca), clique no controle deslizante para ativar a verificação.

   ![](assets/four-2.png)

## Coisas para saber {#things-to-know}

A verificação Cancelar assinatura do Marketo...

* Não conta com seus limites de API
* Exige que seja estabelecida uma conexão com o Marketing
* É uma configuração global
* Bloqueia e-mails enviados do aplicativo da Web, clientes de e-mail e Salesforce

