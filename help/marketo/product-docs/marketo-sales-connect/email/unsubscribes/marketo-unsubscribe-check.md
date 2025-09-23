---
unique-page-id: 18317340
description: Verificação de cancelamento de inscrição do Marketo - Documentação do Marketo - Documentação do produto
title: Verificação de cancelamentos de inscrição no Marketo
exl-id: b8bd5b38-a4f5-4ac7-a5ce-a155fce57998
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 4%

---

# Verificação de cancelamentos de inscrição no Marketo {#marketo-unsubscribe-check}

A [!UICONTROL Verificação de cancelamento de inscrição do Marketo] usa a conexão de sua equipe com o Marketo para evitar que os emails sejam enviados para pessoas que cancelaram a inscrição no sistema de gerenciamento de clientes potenciais da Marketo. Quando um usuário de vendas enviar um email com [!DNL Sales Connect], será feita uma chamada à API para a Marketo verificar se a assinatura da ID do email foi cancelada. Se for, bloquearemos o envio do email.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Ativando {#turning-it-on}

1. No aplicativo Web, clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/one-2.png)

1. Em [!UICONTROL Configurações de Administração], clique em **[!UICONTROL Cancelar Assinaturas]**.

   ![](assets/two-3.png)

1. Clique em **[!UICONTROL Integrações]**.

   ![](assets/three-3.png)

1. Na seção [!UICONTROL Verificação de cancelamento de inscrição do Marketo], clique no controle deslizante para ativar a verificação.

   ![](assets/four-2.png)

## O que você deve saber {#things-to-know}

A verificação de cancelamento de inscrição do Marketo...

* Não é contabilizado em relação aos limites da API
* Requer o estabelecimento de uma conexão com o Marketo
* É uma configuração global
* Bloqueia emails enviados do aplicativo Web, de clientes de email e do Salesforce
* Registrará um email com falha ou impedirá que um usuário envie quando tentar enviar para todos os fluxos de trabalho (envio de plug-in de email, envio individual, envio de campanha de vendas, seleção múltipla e envio), exceto para [emails de grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md), nos quais impediremos que os emails sejam enviados silenciosamente
