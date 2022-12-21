---
unique-page-id: 7505310
description: Assinar uma Smart List - Marketo Docs - Documentação do produto
title: Assinar uma Smart List
exl-id: 4ea1664b-8178-41ae-a184-a8ebe090ef96
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---

# Assinar uma Smart List {#subscribe-to-a-smart-list}

Assinar listas inteligentes é uma ótima maneira de acompanhar as pessoas, com relatórios enviados diretamente para sua caixa de entrada.

Você pode criar uma assinatura de lista inteligente em dois lugares separados:

* Atividades de marketing
* Banco de dados

As assinaturas usam a lista completa de pessoas no momento em que a assinatura é executada.

As assinaturas são ativas, onde sua lista inteligente está, em Atividades de marketing ou Banco de dados.

É possível criar várias subscrições da mesma lista inteligente.

As assinaturas são específicas do espaço de trabalho. Por exemplo, essa lista de assinaturas está em um espaço de trabalho diferente daqueles mostrados no restante deste artigo:

![](assets/one.png)

>[!NOTE]
>
>Você está limitado a 100 assinaturas e um máximo de 100.000 pessoas por assinatura, em espaços de trabalho, por instância do Marketo. Se a lista inteligente tiver mais de 100.000 nomes, o Marketo executará a assinatura dos primeiros 100.000.

## Criar uma assinatura de lista inteligente {#create-a-smart-list-subscription}

1. Vá para o **Banco de dados** ou **Atividades de marketing**.

   ![](assets/db.png)

1. Selecione a lista inteligente para a qual deseja criar uma assinatura. Clique em **Ações de lista** e selecione **Nova assinatura da lista inteligente**.

   ![](assets/three.png)

1. Dê à sua assinatura um **Nome**, em seguida, selecione ou insira os endereços de email do **Recipients**.

   ![](assets/image2015-9-14-13-3a18-3a38.png)

1. Clique no botão **Frequência** e selecione uma frequência.

   ![](assets/image2015-9-14-13-3a21-3a21.png)

1. Defina as **Encerrar entrega** data. Você pode selecionar **Nunca** ou uma data de calendário.

   ![](assets/image2015-9-14-13-3a23-3a37.png)

1. Clique em **Formato** e escolha na lista.

   ![](assets/image2015-9-14-13-3a25-3a25.png)

1. Clique em **Criar**.

   ![](assets/image2015-9-11-15-3a58-3a4.png)

1. A nova assinatura da lista inteligente aparece na parte superior da lista na guia Subscriptions . Clique em **Enviar** se desejar enviar agora, e não aguarde até o delivery de email agendado.

   ![](assets/eight.png)

1. Recomendamos que você desmarque a caixa de seleção Ativa para desativar uma assinatura de lista inteligente se ninguém estiver inscrito nela.

   ![](assets/nine.png)

   Foi fácil, não foi?

## Mensagem de email {#email-message}

Os recipients receberão um email com uma opção para baixar o relatório, bem como um link diretamente para a lista na instância do Marketo. O link de download expira em quatro dias.

>[!NOTE]
>
>Se a variável [Administrador de assinatura segura](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md) está definida como **Sim**, somente as pessoas com acesso à instância do Marketo poderão baixar o relatório.

![](assets/image2015-4-17-15-3a46-3a47.png)

Se um relatório tiver 0 pessoas, os recipients ainda receberão um email. No entanto, o e-mail simplesmente declara que não há pessoas para relatar.

![](assets/image2015-4-17-16-3a11-3a8.png)

>[!NOTE]
>
>Ao modificar um filtro de lista inteligente no qual você baseou uma assinatura, ele também atualiza o relatório.

O email também fornece informações adicionais sobre os filtros usados para criar a lista.

## Excluir uma assinatura {#delete-a-subscription}

Para excluir uma assinatura, selecione-a na guia subscriptions e clique em Delete Subscription.

![](assets/twelve.png)

>[!MORELIKETHIS]
>
>* [Editar uma assinatura de lista inteligente](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/edit-a-smart-list-subscription.md)
>* [Proteger a configuração do administrador de assinatura](/help/marketo/product-docs/reporting/basic-reporting/report-subscriptions/secure-the-subscription-admin-setting.md)

