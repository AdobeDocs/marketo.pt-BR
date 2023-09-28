---
description: Uso do envio de email de vendas em massa no Salesforce - Documentação do Marketo - Documentação do produto
title: Utilização do email de vendas de envio em massa no Salesforce
exl-id: eac77a64-7eaa-48eb-820c-c8e188a234dd
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Utilização do email de vendas de envio em massa no Salesforce {#using-bulk-send-sales-email-in-salesforce}

Saiba como enviar emails em massa no Salesforce para ajudar a dimensionar a comunicação de saída usando Ações de vendas.

>[!NOTE]
>
>O Salesforce impõe um limite de 200 registros que podem ser selecionados de uma só vez.

>[!PREREQUISITES]
>
>Verifique se você instalou o [pacote mais recente do Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md){target="_blank"} to your Salesforce instance and have configured the [Action buttons](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/add-action-buttons-to-salesforce-list-view.md){target="_blank"} em suas visualizações de contatos e listas de clientes potenciais no Salesforce.

## Envio de emails em massa no Salesforce Lightning {#sending-bulk-email-in-salesforce-lightning}

1. No Salesforce, navegue até a página inicial de Clientes potenciais/Contatos clicando no **Clientes potenciais/Contatos** guia.

   ![](assets/using-bulk-send-sales-email-in-salesforce-1.png)

1. Na lista suspensa Exibir, selecione a exibição desejada de Clientes potenciais/Contatos que deseja enviar por email.

   >[!TIP]
   >
   >Você pode criar uma nova visualização clicando no ícone da engrenagem à direita e selecionando **Novo**. Depois de dar um novo nome à visualização e salvá-la, você pode clicar no ícone de filtro à direita para ajudar a filtrar para o conjunto desejado de Clientes potenciais/Contatos que deseja enviar por email.

1. Escolha o cliente em potencial ou a lista de contatos desejada e clique no **Enviar email de vendas** botão.

   ![](assets/using-bulk-send-sales-email-in-salesforce-2.png)

1. Você será direcionado para a janela de composição Ações, com as pessoas selecionadas adicionadas.

1. Selecione o modelo que deseja inserir no editor de janela de composição de Ações ou escreva um email personalizado.

   >[!TIP]
   >
   >Uso [Categorias Fixas](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} para fornecer acesso mais fácil aos seus modelos de email favoritos.

   **ETAPA OPCIONAL**: visualize qualquer personalização de Campos dinâmicos clicando no ícone **Visualizar campos dinâmicos** botão.

   >[!TIP]
   >
   >Se quiser personalizar um modelo para todos os destinatários, clicar na opção Todos os destinatários na barra lateral Composição em massa permite fazer edições em todos os emails de destinatários ao mesmo tempo. Se quiser fazer uma alteração em um email específico, clique no nome do recipient ou no email na barra lateral Composição em massa. Observe que, se você fizer alterações em um email individual e, em seguida, fizer alterações ao selecionar Todos os destinatários, as alterações feitas em Todos os destinatários substituirão as alterações feitas no email individual.

1. Selecionar **Enviar** para enviar o email imediatamente ou **Definir programação** para definir a data e a hora para o envio do email.

   ![](assets/using-bulk-send-sales-email-in-salesforce-3.png)

## Envio de emails em massa no Salesforce Classic {#sending-bulk-email-in-salesforce-classic}

1. No Salesforce, clique na guia **Clientes potenciais/Contatos** guia.

1. Na lista suspensa Exibir, selecione a exibição desejada de Clientes potenciais/Contatos que deseja enviar por email e clique em **Ir**.

   ![](assets/using-bulk-send-sales-email-in-salesforce-4.png)

   >[!TIP]
   >
   >Você pode criar uma nova visualização clicando em Criar nova visualização e configurando os filtros disponíveis para restringir a lista de quem você está adicionando a uma Campanha de vendas.

1. Escolha a lista de clientes potenciais ou contatos desejada e clique no botão **Enviar email de vendas** botão.

   ![](assets/using-bulk-send-sales-email-in-salesforce-5.png)

1. Você será direcionado para a janela de composição Ações com os destinatários selecionados na janela de composição.

1. Selecione o modelo que deseja inserir no editor de janela de composição de Ações ou escreva um email personalizado.

   ![](assets/using-bulk-send-sales-email-in-salesforce-6.png)

   >[!TIP]
   >
   >Uso [Categorias Fixas](/help/marketo/product-docs/marketo-sales-insight/actions/email/using-the-compose-window/using-a-template-in-the-compose-window.md#pinning-template-categories-in-the-compose-window){target="_blank"} para fornecer acesso mais fácil aos seus modelos de email favoritos.

   **ETAPA OPCIONAL**: visualize qualquer personalização de Campos dinâmicos clicando no ícone **Visualizar campos dinâmicos** botão.

   >[!TIP]
   >
   >Se quiser personalizar um modelo para todos os destinatários, clicar na opção Todos os destinatários na barra lateral Composição em massa permite fazer edições em todos os emails de destinatários ao mesmo tempo. Se quiser fazer uma alteração em um email específico, clique no nome do recipient ou no email na barra lateral Composição em massa. Observe que, se você fizer alterações em um email individual e, em seguida, fizer alterações ao selecionar Todos os destinatários, as alterações feitas em Todos os destinatários substituirão as alterações feitas no email individual.

1. Selecionar **Enviar** para enviar o email imediatamente ou **Definir programação** para definir a data e a hora para o envio do email.
