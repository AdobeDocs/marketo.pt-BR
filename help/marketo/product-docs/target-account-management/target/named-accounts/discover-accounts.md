---
unique-page-id: 11378812
description: Contas do Discover - Documentação do Marketo - Documentação do produto
title: Descobrir contas
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 1%

---

# Descobrir contas {#discover-accounts}

Use a opção Discover para identificar contas de público-alvo potenciais.

## [!UICONTROL Descobrir Contas do CRM] {#discover-crm-accounts}

Identifique contas de destino em potencial pelo seu CRM.

>[!NOTE]
>
>Depois de conectar seu CRM ao Marketo TAM, **[!UICONTROL Descubra Contas do CRM]** mostrará todas as contas do CRM e informações relevantes para ajudá-lo a escolher as contas nomeadas certas. O Marketo adiciona mais informações sobre o que é recebido do CRM.

**[!UICONTROL Pessoas]** (Em [!UICONTROL Descobrir Contas do CRM] e [!UICONTROL Descobrir Empresas da Marketo]): Inclui Contatos e Clientes Potenciais. Clientes potenciais podem ser descobertos usando a [correspondência entre lead e conta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md) da Marketo.

**[!UICONTROL Pessoas em Potencial]** (Em [!UICONTROL Descobrir Contas do CRM] e [!UICONTROL Descobrir Empresas da Marketo]): mostra quantos clientes em potencial a Marketo encontrou que poderiam pertencer a uma conta do CRM.

**Campo do CRM personalizado** (somente em contas do Discover CRM): isso ajudará você a alinhar sua organização de vendas e marketing para a seleção das contas de destino corretas. Depois que você [mapear o campo personalizado do CRM](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) com o Marketo TAM, mostraremos os dados mapeados para ajudá-lo a identificar suas contas de destino.

1. Em [!UICONTROL Contas Nomeadas], clique no menu suspenso **[!UICONTROL Novas]** e selecione **[!UICONTROL Descobrir Contas do CRM]**.

   ![](assets/disc-crm-one.png)

1. Uma nova janela/guia será aberta. Selecione as contas do CRM que você deseja adicionar às suas [!UICONTROL Contas Nomeadas] e clique em **[!UICONTROL Avançar]**.

   ![](assets/disc-crm-two.png)

1. A tela de visualização confirma a quantidade de seleções. Clique em **[!UICONTROL Criar]**.

   ![](assets/disc-three.png)

   Isso é tudo!

   ![](assets/disc-four.png)

## [!UICONTROL Descobrir Empresas da Marketo] {#discover-marketo-companies}

Identifique as empresas certas para o direcionamento.

>[!NOTE]
>
>Em [!UICONTROL Descobrir Empresas da Marketo], você verá empresas da Marketo que não vieram do seu CRM.

1. Em [!UICONTROL Contas Nomeadas], clique no menu suspenso **[!UICONTROL Novas]** e selecione **[!UICONTROL Descobrir Empresas da Marketo]**.

   ![](assets/one-1.png)

1. Uma nova janela/guia será aberta. Selecione as empresas que deseja adicionar às suas [!UICONTROL Contas Nomeadas] e clique em **[!UICONTROL Avançar]**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >Em [!UICONTROL Descobrir Empresas da Marketo] e Descobrir CRM, a Marketo automaticamente:
   >
   >* Localiza pessoas do banco de dados do Marketo que têm essa empresa listada em seus registros. Se você vir vários valores para alguns dos atributos (por exemplo, Setor), é porque o Marketo encontrou valores diferentes listados para essas pessoas individuais. O atributo com mais ocorrências vence
   >
   >Somente no **Discover CRM**, o Marketo automaticamente:
   >
   >* Sincroniza e associa Contatos do CRM à [!UICONTROL Conta Nomeada]
   >
   >Somente em **[!UICONTROL Descobrir Empresas da Marketo]**, a Marketo automaticamente:
   >
   >* Filtra a maioria dos provedores de serviço de Internet e domínios públicos (por exemplo, yahoo.com, gmail.com) como nomes de empresa
   >
   >* Elimina duplicatas de contas do CRM. Se você tiver &quot;Acme&quot; em um registro e &quot;Acme Inc&quot; (ou qualquer um dos seguintes sufixos: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), nós os fundiremos no TAM como apenas &quot;Acme&quot;

1. Clique na seta para baixo na coluna [!UICONTROL Conta nomeada] para exibir o menu suspenso.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >A partir de agora, todas as novas pessoas dessas empresas selecionadas serão automaticamente atribuídas às respectivas contas nomeadas. Verifique essas empresas e certifique-se de que elas estejam atribuídas à [!UICONTROL Conta nomeada] correta.

1. Para selecionar uma Conta existente, clique no menu suspenso **[!UICONTROL Conta nomeada]**, escolha a conta desejada e clique em **[!UICONTROL Avançar]**.

   ![](assets/disc-comp-four.png)

   Você também tem a opção de criar uma nova [!UICONTROL Conta nomeada] digitando o nome desejado diretamente na caixa suspensa. Clique fora da caixa quando terminar...

   ![](assets/disc-comp-five.png)

   ...e você verá sua nova [!UICONTROL Conta nomeada]. Nesse ponto, basta clicar em **[!UICONTROL Avançar]**, como na Etapa 4.

   ![](assets/disc-comp-six.png)

1. Clique em **[!UICONTROL Criar]**.

   ![](assets/disc-comp-seven.png)

   Bom trabalho!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Se você estiver vendo uma incompatibilidade entre as contas do CRM selecionadas e o que está na Grade do Discover CRM, é provável que seja devido a um ou mais dos seguintes motivos:
>
>* Ter diferentes contas do CRM com nomes semelhantes que foram deduplicados
>* A próxima sincronização agendada ainda não ocorreu

>[!MORELIKETHIS]
>
>[Lead para Correspondência de Conta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
