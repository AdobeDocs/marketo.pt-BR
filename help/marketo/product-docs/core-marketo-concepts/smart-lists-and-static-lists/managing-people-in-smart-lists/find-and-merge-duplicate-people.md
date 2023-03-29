---
unique-page-id: 557339
description: Encontrar e mesclar pessoas duplicadas - Documentos do Marketo - Documentação do produto
title: Localizar e mesclar pessoas duplicadas
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Localizar e mesclar pessoas duplicadas {#find-and-merge-duplicate-people}

O Marketo remove a duplicação automaticamente quando novas pessoas entram no sistema. No entanto, seu CRM pode ter enviado inicialmente duplicatas para o Marketo. Aqui está como mesclá-los.

>[!NOTE]
>
>A Marketo não deduplicará automaticamente em relação a uma sincronização do Salesforce ou do Microsoft Dynamics, ou quando você inserir pessoas manualmente.

>[!PREREQUISITES]
>
>Encontrar e mesclar duplicatas envolverá o uso de [listas inteligentes integradas/do sistema](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md).

## Localizar duplicatas {#find-duplicates}

1. Vá para o **Banco de dados** área.

   ![](assets/db.png)

   >[!CAUTION]
   >
   >A mesclagem de pessoas no Marketo pode não funcionar se você usar uma conta de pessoa do Salesforce. Mesclar os registros no Salesforce, se possível.

1. Selecione o **Possíveis duplicatas** lista inteligente do sistema e clique no botão **Pessoas** guia .

   ![](assets/two.png)

   >[!NOTE]
   >
   >Você também pode [Localizar Pessoas Duplicadas com Lógica Personalizada](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md).

## Unir Pessoas Manualmente {#merge-people-manually}

>[!CAUTION]
>
>Ao mesclar pessoas, se a pessoa perdedora tiver um objeto personalizado Marketo, ele **not** ser reassociado à pessoa vencedora. Recoloque o objeto personalizado antes de executar a mesclagem.

1. Selecione as duplicatas, mantendo pressionada a tecla Ctrl/Cmd e clicando em e, em seguida, clique em **Unir Pessoas**.

   ![](assets/three.png)

   >[!TIP]
   >
   >Você pode ter duas ou mais duplicatas para a mesma pessoa - selecione-as todas de uma vez.

1. Você verá os valores entre os registros que _don&#39;t_ correspondência. Selecione o valor que deseja manter para cada campo. Clique em **Mesclar** quando concluído. Se não quiser nenhum dos valores, você poderá verificar **Personalizado** e insira um valor de sua escolha.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Ao mesclar pessoas manualmente, a primeira pessoa selecionada será o &quot;vencedor&quot;. Portanto, na guia Pessoas, se você estiver mesclando IDs de registro 198 e 199, e clicar em 199 primeiro, 199 será a ID de registro das pessoas mescladas. Isso também se aplica se mais de dois registros forem mesclados.

   >[!TIP]
   >
   >É melhor mesclar do que excluir. Você conservará todo o histórico (visitas à página, cliques em links, aberturas de email, preenchimentos de formulário etc.).

## Efeito no Salesforce {#effect-in-salesforce}

Se você tiver a integração do Salesforce, há algumas observações sobre o efeito dos leads de mesclagem no Salesforce.

* Ao mesclar somente leads ou somente contatos, eles são mesclados de acordo com as regras normais do Salesforce.
* Ao mesclar leads e contatos, todos os leads são convertidos em Contatos antes da mesclagem de acordo com as regras normais do Salesforce.

Para obter detalhes específicos do comportamento do Salesforce ao mesclar leads ou contatos, verifique os seguintes documentos do Salesforce:

* [Mesclando leads duplicados](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US)
* [Mesclando Contatos Duplicados](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US)

## Mesclagem em massa {#bulk-merging}

Se você tiver muitas duplicatas para mesclar manualmente, entre em contato com a Equipe da conta do Adobe (seu Gerente de conta) para discutir suas opções.

Se você estiver conectado a um CRM, os registros serão mesclados lá de acordo com as regras abaixo.
