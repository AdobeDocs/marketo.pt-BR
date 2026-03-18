---
description: Saiba mais sobre a verificação de cancelamento de assinatura do Marketo para que os vendedores não possam enviar um email para as pessoas que cancelaram a assinatura no Marketo.
title: Verificação de cancelamentos de inscrição no Marketo
exl-id: 3c242d04-cf6c-466b-9bcd-e77c6d97d308
feature: Sales Insight Actions
source-git-commit: 03f984d4049c119267c7b2c2baa4e68c7db34ad0
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 6%

---

# [!UICONTROL Verificação de Cancelamento de Inscrição do Marketo] {#marketo-unsubscribe-check}

A [!UICONTROL Verificação de cancelamento de inscrição do Marketo] usa a conexão de sua equipe com o Marketo para evitar que os emails sejam enviados para pessoas que cancelaram a inscrição no sistema de gerenciamento de clientes potenciais da Marketo. Quando um usuário de vendas enviar um email com [!DNL Marketo Sales], será feita uma chamada à API para a Marketo verificar se a assinatura da ID do email foi cancelada. Se for, bloquearemos o envio do email.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

## Ativando {#turning-it-on}

1. Clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/marketo-unsubscribe-check-1.png)

1. Em [!UICONTROL Configurações de Administração], clique em **[!UICONTROL Cancelar Assinaturas]**.

   ![](assets/marketo-unsubscribe-check-2.png)

1. Clique na guia **[!UICONTROL Integrações]**. Na seção [!UICONTROL Verificação de cancelamento de inscrição do Marketo], clique no controle deslizante para ativar a verificação.

   ![](assets/marketo-unsubscribe-check-3.png)

## O que você deve saber {#things-to-know}

A verificação de cancelamento de inscrição do Marketo...

* Não é contabilizado em relação aos limites da API
* Requer o estabelecimento de uma conexão com o Marketo
* É uma configuração global
* Bloqueia emails enviados do aplicativo Web, clientes de email e [!DNL Salesforce]
