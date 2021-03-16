---
unique-page-id: 11378812
description: Contas do Discover - Documentos do Marketo - Documentação do produto
title: Contas do Discover
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---


# Contas do Discover {#discover-accounts}

Use a opção Discover para identificar possíveis contas-alvo.

## Conheça as contas do CRM {#discover-crm-accounts}

Identifique possíveis contas do target a partir do seu CRM.

>[!NOTE]
>
>Após conectar seu CRM ao Marketo TAM, **Discover CRM Accounts** mostrará todas as contas do CRM e informações relevantes para ajudá-lo a escolher as contas nomeadas certas. O Marketo adiciona informações adicionais sobre o que foi recebido do CRM.

**Pessoas**  (Em Contas de CRM do Discover e Empresas de Marketing do Discover): Inclui Contatos e Clientes Potenciais. Os leads podem ser descobertos usando a [correspondência de lead para conta do Marketo](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md).

**Pessoas em potencial**  (Em Contas CRM do Discover e Empresas de Marketing do Discover): Mostra quantos leads Marketo encontrou que poderiam pertencer a uma conta CRM.

**Campo CRM personalizado**  (somente em contas CRM do Discover ): Isso ajudará você a alinhar sua organização de vendas e marketing para selecionar as contas de destino corretas. Depois que você [mapear o campo CRM personalizado](/help/marketo/product-docs/target-account-management/setup-tam/create-a-custom-field-for-crm-discovery.md) com o Marketo TAM, mostraremos os dados mapeados para ajudar a identificar suas contas de destino.

1. Em Contas Nomeadas, clique no menu suspenso **New** e selecione **Discover CRM Accounts**.

   ![](assets/disc-crm-one.png)

1. Uma nova janela/guia será aberta. Selecione as contas CRM que deseja adicionar às suas Contas Nomeadas e clique em **Next**.

   ![](assets/disc-crm-two.png)

1. A tela de visualização confirma a quantidade de seleções. Clique em **Criar**.

   ![](assets/disc-three.png)

   Isso é tudo!

   ![](assets/disc-four.png)

## Empresas do Marketing Discover {#discover-marketo-companies}

Identifique as empresas certas para direcionamento.

>[!NOTE]
>
>Em Empresas do Discover Marketo, você verá empresas do Marketo que não vieram de seu CRM.

1. Em Contas Nomeadas, clique no menu suspenso **New** e selecione **Discover Marketo Companies**.

   ![](assets/one-1.png)

1. Uma nova janela/guia será aberta. Selecione as empresas que deseja adicionar às suas Contas Nomeadas e clique em **Próximo**.

   ![](assets/disc-comp-two.png)

   >[!NOTE]
   >
   >No Discover Marketing Company e no Discover CRM, o Marketo automaticamente realiza:
   >
   >* Encontra pessoas do banco de dados do Marketo que têm a empresa listada em seus registros. Se você vir vários valores para alguns dos atributos (por exemplo, Setor), é porque o Marketo encontrou valores diferentes listados para essas pessoas individuais. O atributo com mais ocorrências vence
   >
   >Somente em **Discover CRM**, Marketo automaticamente:
   >
   >* Sincroniza e associa os Contatos do CRM à Conta Nomeada
   >
   >Somente em **Discover Marketo Company**, o Marketo automaticamente:
   >
   >* Filtra a maioria dos provedores de serviços de Internet e domínios públicos (por exemplo, yahoo.com, gmail.com) como nomes de empresas
      >
      >
   * Elimina as contas CRM. Se você tiver &quot;Acme&quot; em um registro e &quot;Acme Inc&quot; (ou qualquer um dos seguintes sufixos: Co, Corp, Corporation, Gmbh, Inc, Incorporated, LLC, LLP, LP, Ltd, PA, PC, PLC, PLLC), nós os mesclaremos em TAM como apenas &quot;Acme&quot;
   >
   >Se você quiser que o Marketo decomponha contas por ID de CRM ou Proprietário da conta em vez de por Nome da empresa, entre em contato com [Suporte do Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Clique na seta para baixo na coluna Conta nomeada para exibir o menu suspenso.

   ![](assets/disc-comp-three.png)

   >[!CAUTION]
   >
   >A partir de agora, quaisquer novas pessoas dessas empresas selecionadas serão automaticamente atribuídas às respectivas contas nomeadas. Verifique novamente essas empresas e certifique-se de que elas estejam atribuídas à Conta Nomeada correta.

1. Para selecionar uma Conta existente, clique no menu suspenso **Conta Nomeada**, escolha a conta desejada e clique em **Próximo**.

   ![](assets/disc-comp-four.png)

   Você também tem a opção de criar uma nova Conta nomeada digitando o nome desejado diretamente na caixa suspensa. Clique fora da caixa quando terminar...

   ![](assets/disc-comp-five.png)

   ...e você verá sua nova Conta nomeada. Nesse momento, clique em **Next** como na Etapa 4.

   ![](assets/disc-comp-six.png)

1. Clique em **Criar**.

   ![](assets/disc-comp-seven.png)

   Bom trabalho!

   ![](assets/disc-co-six.png)

>[!NOTE]
>
>Se você estiver vendo uma incompatibilidade entre as contas do CRM que você selecionou e o que está na Grade do Discover CRM, é provável que seja devido a um ou mais dos seguintes itens:
>
>* Ter diferentes contas CRM com nomes semelhantes que foram deduplicados
>* A próxima sincronização programada ainda não ocorreu


>[!MORELIKETHIS]
>
>[Lead para a correspondência da conta](/help/marketo/product-docs/target-account-management/target/named-accounts/lead-to-account-matching.md)
