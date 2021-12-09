---
description: Marketo Unsubscribe Check - Marketo Docs - Documentação do produto
title: Verificação de cancelamentos de inscrições no Marketo
hide: true
hidefromtoc: true
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 4%

---

# Verificação de cancelamentos de inscrições no Marketo {#marketo-unsubscribe-check}

A verificação de cancelamento de assinatura do Marketo usa a conexão da sua equipe com o Marketo para impedir que os emails sejam enviados para pessoas que não estão assinadas no sistema de gerenciamento de clientes potenciais da Marketo. Quando um usuário de vendas envia um email com o Marketo Sales, uma chamada de API é feita ao Marketo para verificar se a ID do email foi cancelada. Se estiver, bloquearemos o envio do email.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Ativando {#turning-it-on}

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Em Configurações de administração, clique em **Cancelamentos de assinatura**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Clique no botão **Integrações** guia . Na seção Marketo Unsubscribe Check , clique no controle deslizante para ativar a verificação.

   ![](assets/marketo-unsubscribe-check-3.png)

## O que saber {#things-to-know}

A verificação de cancelamento de assinatura do Marketo...

* Não conta em relação aos limites da API
* Requer que uma conexão Marketo seja estabelecida
* É uma configuração global
* Bloqueia emails enviados da aplicação Web, clientes de email e Salesforce
