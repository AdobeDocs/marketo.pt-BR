---
unique-page-id: 42762825
description: Uso de ações em massa no Salesforce Lightning - Documentos do Marketo - Documentação do produto
title: Uso de ações em massa no Salesforce Lightning
exl-id: 72022507-6568-4cc2-b3b5-c1703a1493ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# Uso de ações em massa no Salesforce Lightning {#using-bulk-actions-in-salesforce-lightning}

Saiba como executar ações em massa, como adicionar leads a uma campanha, enviar um email em massa ou enviar leads do Salesforce para o Sales Connect.

>[!PREREQUISITES]
>
>Atualize para a versão mais recente do pacote Sales Connect e instale os botões de ação em massa na visualização lead/contato. [Clique aqui para obter instruções](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf).

>[!NOTE]
>
>Antes de seguir as etapas abaixo, verifique se você está conectado à conta do Marketo Sales Connect.

## Email em massa {#bulk-email}

1. No Salesforce, clique no botão **Clientes potenciais** e escolha a lista de leads desejados.

   ![](assets/one-6.png)

   >[!NOTE]
   >
   >Se você já estiver na lista que usará, será necessário executá-la novamente escolhendo-a na lista suspensa para garantir que os botões de ação em massa do MSC sejam exibidos. Este é o comportamento do Salesforce que não pode ser alterado.

1. Clique no menu suspenso da seta (na extremidade direita da tela) e selecione **E-mail com MSC**.

   ![](assets/two-6.png)

1. Um e-mail da MSC aparecerá. Ele inclui os seguintes recursos:

   a. O campo &quot;Para&quot; mostra &quot;Todos os recebimentos&quot; - corresponde à lista de leads que você escolheu na Exibição da Lista de Lead\
   b. Essa lista é visível no painel esquerdo chamado &quot;Composição em massa&quot; - você pode adicionar/remover destinatários aqui\
   c. Você pode escolher um modelo ou criar seu próprio email\
   d. Você pode enviar o email imediatamente ou agendar o envio posteriormente

   ![](assets/three-5.png)

## Adicionar à campanha  {#add-to-campaign}

1. No Salesforce, clique no botão **Clientes potenciais** e escolha a lista de leads desejados.

   ![](assets/four-4.png)

1. Clique no menu suspenso da seta (na extremidade direita da tela) e selecione **Adicionar à Campanha MSC**.

   ![](assets/five-4.png)

1. Um pop-up &quot;Adicionar pessoas à sua campanha&quot; será exibido. Clique em **Próximo** e percorra o fluxo de campanha típico para acionar uma campanha MSC.

   ![](assets/six-1.png)

## Enviar por push ao Marketo Sales Connect {#push-to-marketo-sales-connect}

1. No Salesforce, clique no botão **Clientes potenciais** e escolha a lista de leads desejados.

   ![](assets/seven-2.png)

1. Clique no menu suspenso da seta (na extremidade direita da tela) e selecione **Encaminhar para MSC**.

   ![](assets/eight-2.png)

1. Uma nova guia chamada &quot;Salesforce Bridge&quot; será aberta. Clique no botão **Prossiga para o Grupo →** botão.

   ![](assets/nine-2.png)

1. Você será enviado para sua conta do MSC onde verá um grupo criado com carimbo de data/hora. Você receberá uma notificação quando a sincronização for concluída e o grupo incluirá os leads sincronizados do Salesforce.

   ![](assets/ten-1.png)

>[!NOTE]
>
>Você também pode seguir as mesmas etapas para usar ações em massa na Exibição de lista de contatos.

>[!MORELIKETHIS]
>
>* [Enviar emails por email de grupo](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/sending-emails-via-group-email.md)
>* [Composição de emails em massa com Selecionar e enviar](/help/marketo/product-docs/marketo-sales-connect/email/using-the-compose-window/composing-bulk-emails-with-select-and-send.md#sending-emails)

