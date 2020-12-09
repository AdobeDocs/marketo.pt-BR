---
unique-page-id: 557339
description: Localizar e mesclar pessoas do Duplicado - Documentos do Marketing - Documentação do produto
title: Localizar e mesclar pessoas do Duplicado
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---


# Localizar e mesclar pessoas do Duplicado {#find-and-merge-duplicate-people}

Marketo cancela automaticamente os duplicados quando novas pessoas entram no sistema. No entanto, seu CRM pode ter enviado duplicados inicialmente para o Marketo. Aqui está como mesclá-los.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>O Marketo não eliminará automaticamente a duplicação em uma sincronização do Salesforce ou do Microsoft Dynamics, ou quando você inserir pessoas manualmente.

>[!PREREQUISITES]
>
>Encontrar e mesclar duplicados envolverá o uso de listas [inteligentes](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md)incorporadas/do sistema.

## Localizar Duplicados {#find-duplicates}

1. Vá para a área **Banco de Dados** .

   ![](assets/db.png)

   >[!CAUTION]
   >
   >A mesclagem de pessoas no Marketo pode não funcionar se você usar uma conta pessoal do Salesforce. Por favor, mescle os registros no Salesforce, se possível.

1. Selecione a lista inteligente do sistema **Possíveis** **Duplicados** e clique na guia **Pessoas** .

   ![](assets/two.png)

   >[!NOTE]
   >
   >Você também pode [Localizar pessoas do Duplicado com lógica](find-duplicate-people-with-custom-logic.md)personalizada.

## Unir pessoas manualmente {#merge-people-manually}

>[!CAUTION]
>
>Ao mesclar pessoas, se a pessoa perdedora tiver um objeto personalizado Marketo, ele **não** será associado novamente à pessoa vencedora. Recoloque o objeto personalizado antes de executar a mesclagem.

Selecione os duplicados mantendo Ctrl/Cmd pressionado e clicando em e, em seguida, em Mesclar pessoas.
![](assets/three.png)

>[!TIP]
>
>Você pode ter dois ou mais duplicados para a mesma pessoa - selecione-os todos ao mesmo tempo.

1. Você verá os valores entre os registros que *não* correspondem. Selecione o valor que deseja manter para cada campo. Clique em **Mesclar** quando concluído. Se você não quiser nenhum dos valores, marque **Personalizado** e insira um valor de sua escolha.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Ao mesclar manualmente as pessoas, a primeira pessoa selecionada será &quot;vencedora&quot;. Portanto, na guia Pessoas se você estiver mesclando IDs de registro 198 e 1999, e você clicar em 199 primeiro, 199 será a ID de registro das pessoas mescladas. Isso também se aplica se mais de dois registros forem mesclados.

   >[!TIP]
   >
   >É melhor mesclar do que excluir. Você conservará todo o histórico (visitas à página, cliques em links, abrir e-mail, preenchimentos de formulário etc.).

## Efeito no Salesforce {#effect-in-salesforce}

Se você tiver a integração do Salesforce, há algumas observações sobre o efeito dos Clientes Potenciais de Mesclagem no Salesforce.

    * Ao mesclar somente os Clientes potenciais ou somente os Contatos, eles são mesclados de acordo com as regras normais do Salesforce.
    * Ao unir Clientes potenciais e Contatos, todos os Clientes potenciais são convertidos em Contatos antes da mesclagem de acordo com as regras normais do Salesforce.

Para obter detalhes específicos do comportamento do Salesforce ao mesclar Clientes potenciais ou Contatos, verifique os seguintes documentos do Salesforce:

    * [Mesclando Clientes Potenciais do Duplicado](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
    * [Mesclando Contatos do Duplicado](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Mesclagem em massa {#bulk-merging}

Se você tiver muitos duplicados para mesclar manualmente, entre em contato com o Gerente de sucesso do cliente para discutir suas opções.

Super! Se você estiver conectado a um CRM, os registros serão mesclados lá, de acordo com as regras abaixo.