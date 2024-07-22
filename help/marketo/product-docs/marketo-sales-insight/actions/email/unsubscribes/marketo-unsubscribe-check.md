---
description: Verificação de cancelamento de inscrição do Marketo - Documentação do Marketo - Documentação do produto
title: Verificação de cancelamentos de inscrições no Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 4%

---

# Verificação de cancelamentos de inscrições no Marketo {#marketo-unsubscribe-check}

A Verificação de cancelamento de inscrição do Marketo usa a conexão de sua equipe com o Marketo para impedir que os emails sejam enviados para pessoas que cancelaram a inscrição no sistema de gerenciamento de clientes potenciais da Marketo. Quando um usuário de vendas envia um email com o Marketo Sales, é feita uma chamada à API do Marketo para verificar se a assinatura da ID de email foi cancelada. Se for, bloquearemos o envio do email.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Ativando {#turning-it-on}

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Em Configurações do administrador, clique em **Cancelar assinatura**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Clique na guia **Integrações**. Na seção Cancelar inscrição da verificação do Marketo, clique no controle deslizante para ativar a verificação.

   ![](assets/marketo-unsubscribe-check-3.png)

## O que você deve saber {#things-to-know}

A verificação de cancelamento de inscrição do Marketo...

* Não é contabilizado em relação aos limites da API
* Requer o estabelecimento de uma conexão com o Marketo
* É uma configuração global
* Bloqueia emails enviados do aplicativo Web, clientes de email e Salesforce
