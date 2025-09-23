---
unique-page-id: 7505310
description: Assinar uma lista inteligente - Documentação do Marketo - Documentação do produto
title: Assinar uma lista inteligente
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
feature: Reporting
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 2%

---

# Assinar uma lista inteligente {#subscribe-to-a-smart-list}

A inscrição em listas inteligentes é uma ótima maneira de rastrear pessoas, com relatórios enviados diretamente para sua caixa de entrada.

É possível criar uma assinatura de lista inteligente em dois lugares separados:

* [!UICONTROL Atividades de marketing]
* [!UICONTROL Banco de dados]

As assinaturas usam a lista completa de pessoas no momento em que são executadas.

As assinaturas ficam no local em que se encontra a sua lista inteligente, em [!UICONTROL Atividades de marketing] ou [!UICONTROL Banco de dados].

É possível criar várias assinaturas a partir da mesma lista inteligente.

As assinaturas são específicas do espaço de trabalho. Por exemplo, essa lista de assinaturas está em um espaço de trabalho diferente daqueles mostrados no restante deste artigo:

![](assets/one.png)

>[!NOTE]
>
>Você está limitado a 100 assinaturas e a um máximo de 100.000 pessoas por assinatura, em espaços de trabalho e por instância do Marketo. Se a lista inteligente contiver mais de 100.000 nomes, o Marketo executará a assinatura para os primeiros 100.000.

## Criar uma assinatura de lista inteligente {#create-a-smart-list-subscription}

1. Vá para o **[!UICONTROL Banco de Dados]** ou **[!UICONTROL Atividades de Marketing]**.

   ![](assets/db.png)

1. Selecione a lista inteligente para a qual deseja criar uma assinatura. Clique em **[!UICONTROL Listar Ações]** e selecione **[!UICONTROL Nova Assinatura da Smart List]**.

   ![](assets/three.png)

1. Dê um **[!UICONTROL Nome]** à sua assinatura e selecione ou insira os endereços de email dos **[!UICONTROL Destinatários]**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Clique na lista **[!UICONTROL Frequência]** e selecione uma frequência.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Defina a data de **[!UICONTROL Término da Entrega]**. Você pode selecionar **[!UICONTROL Nunca]** ou uma data de calendário.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Clique em **[!UICONTROL Formatar]** e escolha na lista.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. A nova assinatura da lista inteligente é exibida na parte superior da lista na guia Subscriptions. Clique em **[!UICONTROL Enviar]** se desejar enviar agora e não aguardar a entrega agendada de email.

   ![](assets/eight.png)

1. Recomendamos que você desmarque a caixa de seleção **[!UICONTROL Ativo]** para desativar uma assinatura de lista inteligente se ninguém tiver assinado.

   ![](assets/nine.png)

   Isso foi fácil, não foi?

## Mensagem de email {#email-message}

Os recipients receberão um email com uma opção para baixar o relatório, bem como um link diretamente para a lista na instância do Marketo. O link de download expira em quatro dias.

>[!NOTE]
>
>Se a configuração [Administrador de Assinatura Segura](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) estiver definida como **[!UICONTROL Sim]**, somente as pessoas com acesso à instância do Marketo poderão baixar o relatório.

![](assets/image2015-4-17-15-3a46-3a47.png)

Se um relatório tiver 0 pessoas, os recipients ainda receberão um email. No entanto, o email simplesmente declara que não há pessoas para relatar.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Quando você modifica um filtro de lista inteligente no qual uma assinatura foi baseada, ele também atualiza o relatório.

O email também fornece informações adicionais sobre os filtros usados para criar a lista.

## Excluir uma assinatura {#delete-a-subscription}

Para excluir uma assinatura, selecione-a na guia de assinaturas e clique em **[!UICONTROL Excluir Assinatura]**.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Editar uma Assinatura de Smart List](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Proteger a Configuração de Administrador da Assinatura](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)
