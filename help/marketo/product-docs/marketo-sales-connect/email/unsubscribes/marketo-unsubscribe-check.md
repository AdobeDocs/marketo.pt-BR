---
unique-page-id: 18317340
description: Marketo Unsubscribe Check - Marketo Docs - Documentação do produto
title: Verificação de cancelamentos de inscrições no Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
source-git-commit: 82c75d52caf3a0320cd3e8534b3b0870cf12d660
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---

# Verificação de cancelamentos de inscrições no Marketo {#marketo-unsubscribe-check}

A verificação de cancelamento de assinatura do Marketo usa a conexão da sua equipe com o Marketo para impedir que os emails sejam enviados para pessoas que não estão assinadas no sistema de gerenciamento de clientes potenciais da Marketo. Quando um usuário de vendas envia um email com o Sales Connect, uma chamada de API é feita ao Marketo para verificar se a ID do email foi cancelada. Se estiver, bloquearemos o envio do email.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Ativando {#turning-it-on}

1. No aplicativo Web, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one-2.png)

1. Em Configurações de administração, clique em **Cancelamentos de assinatura**.

   ![](assets/two-3.png)

1. Clique em **Integrações**.

   ![](assets/three-3.png)

1. Na seção Marketo Unsubscribe Check , clique no controle deslizante para ativar a verificação.

   ![](assets/four-2.png)

## O que saber {#things-to-know}

A verificação de cancelamento de assinatura do Marketo...

* Não conta em relação aos limites da API
* Requer que uma conexão Marketo seja estabelecida
* É uma configuração global
* Bloqueia emails enviados da aplicação Web, clientes de email e Salesforce
* Registrará um email com falha ou impedirá que um usuário envie quando ele tentar enviar para todos os workflows (envio de plug-in de email, envio individual, envio de campanha de vendas, seleção múltipla e envio) exceto para [emails de grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), em que impediremos o envio silencioso de emails
