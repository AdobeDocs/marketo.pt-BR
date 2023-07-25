---
unique-page-id: 11378812
description: Contas do Discover - Documentação do Marketo - Documentação do produto
title: Descobrir Contas
exl-id: 90da4ae0-0a12-48bd-8bae-a7431d2cf4f4
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 2%

---

# Descobrir Contas {#discover-accounts}

Use a opção Discover para identificar contas de público-alvo potenciais.

## Descobrir contas do CRM {#discover-crm-accounts}

Identifique contas de destino em potencial pelo seu CRM.

>[!NOTE]
>
>Depois de conectar seu CRM ao Marketo TAM, **Descobrir Contas do CRM** O mostrará todas as contas CRM e informações relevantes para ajudá-lo a escolher as contas nomeadas certas. O Marketo adiciona mais informações sobre o que é recebido do CRM.

**Pessoas** (Em Descobrir contas do CRM e Descobrir empresas da Marketo): inclui Contatos e Clientes potenciais. Marketo Clientes potenciais podem ser detectados usando o [correspondência entre lead e conta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**Pessoas em potencial** (Em Descobrir contas do CRM e Descobrir empresas da Marketo): mostra quantos clientes em potencial a Marketo encontrou que poderiam pertencer a uma conta do CRM.

**Campo CRM personalizado** (Somente em Descobrir Contas do CRM): isso ajudará você a alinhar sua organização de vendas e marketing para a seleção das contas de destino corretas. Uma vez que [mapear o campo personalizado do CRM](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) com o Marketo TAM, mostraremos os dados mapeados para ajudá-lo a identificar suas contas do target.

1. Em Contas Nomeadas, clique no link **Novo** e selecione **Descobrir Contas do CRM**.

   ![](assets/disc-crm-one.png)

1. Uma nova janela/guia será aberta. Selecione as contas CRM que deseja adicionar às Contas Nomeadas e clique em **Próxima**.

   ![](assets/disc-crm-two.png)

1. A tela de visualização confirma a quantidade de seleções. Clique em **Criar**.

   ![](assets/disc-three.png)

   Isso é tudo!

   ![](assets/disc-four.png)

## Descobrir empresas do Marketo {#discover-marketo-companies}

Identifique as empresas certas para o direcionamento.

>[!NOTE]
>
>Em Descobrir Empresas da Marketo, você verá empresas da Marketo que não vieram do seu CRM.

1. Em Contas Nomeadas, clique no link **Novo** e selecione **Descubra as empresas da Marketo**.

   ![](assets/one-1.png)

1. Uma nova janela/guia será aberta. Selecione as empresas que deseja adicionar às Contas Nomeadas e clique em **Próxima**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >Em Descobrir empresas da Marketo e Descobrir CRM, o Marketo automaticamente:
   >
   >* Localiza pessoas do banco de dados do Marketo que têm essa empresa listada em seus registros. Se você vir vários valores para alguns dos atributos (por exemplo, Setor), é porque o Marketo encontrou valores diferentes listados para essas pessoas individuais. O atributo com mais ocorrências vence
   >
   >Entrada **Descubra o CRM** somente, o Marketo automaticamente:
   >
   >* Sincroniza e associa Contatos CRM à Conta Nomeada
   >
   >Entrada **Descubra as empresas da Marketo** somente, o Marketo automaticamente:
   >
   >* Filtra a maioria dos provedores de serviço de Internet e domínios públicos (por exemplo, yahoo.com, gmail.com) como nomes de empresa
   >
   >* Elimina duplicatas de contas do CRM. Se você tiver &quot;Acme&quot; em um registro e &quot;Acme Inc&quot; (ou qualquer um dos seguintes sufixos: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), nós os fundiremos no TAM como apenas &quot;Acme&quot;
   >
   >Se você quiser que a Marketo elimine a duplicação de contas pelo CRM ID ou pelo Proprietário da conta, em vez de pelo Nome da empresa, entre em contato com [Suporte ao Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Clique na seta para baixo na coluna Conta Nomeada para revelar o menu suspenso.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >A partir de agora, todas as novas pessoas dessas empresas selecionadas serão automaticamente atribuídas às respectivas contas nomeadas. Verifique essas empresas e certifique-se de que elas estejam atribuídas à Conta nomeada correta.

1. Para selecionar uma Conta existente, clique na guia **Conta nomeada** selecione a conta desejada e clique em **Próxima**.

   ![](assets/disc-comp-four.png)

   Você também tem a opção de criar uma nova Conta nomeada digitando o nome desejado diretamente na caixa suspensa. Clique fora da caixa quando terminar...

   ![](assets/disc-comp-five.png)

   ...e você verá sua nova Conta Nomeada. Nesse ponto, basta clicar em **Próxima** como na Etapa 4.

   ![](assets/disc-comp-six.png)

1. Clique em **Criar**.

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
