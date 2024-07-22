---
unique-page-id: 557339
description: Localizar e mesclar pessoas duplicadas - Documentação do Marketo - Documentação do produto
title: Localizar e Mesclar Pessoas Duplicadas
exl-id: a6d46096-587a-4e3a-b37a-917c0d2098b1
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Localizar e Mesclar Pessoas Duplicadas {#find-and-merge-duplicate-people}

O Marketo Engage remove a duplicação automaticamente quando novas pessoas entram no sistema. No entanto, seu CRM pode ter enviado inicialmente duplicatas. Veja como uni-los.

>[!CAUTION]
>
>Mesclar pessoas é permanente, não há opção para &quot;desfazer&quot;.

>[!PREREQUISITES]
>
>Encontrar e mesclar duplicatas envolverá o uso de [Smart Lists integradas/do sistema](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-built-in-system-smart-lists.md){target="_blank"}.

>[!NOTE]
>
>A Marketo não eliminará a duplicação automaticamente em relação a uma sincronização do Salesforce ou do Microsoft Dynamics, ou quando você inserir pessoas manualmente.

## Localizar duplicados {#find-duplicates}

1. Vá para a área **[!UICONTROL Banco de Dados]**.

   ![](assets/find-and-merge-duplicate-people-1.png)

   >[!CAUTION]
   >
   >A mesclagem de pessoas no Marketo pode não funcionar se você usar uma conta pessoal do Salesforce. Mescle os registros no Salesforce, se possível.

1. Selecione a **[!UICONTROL Possíveis duplicatas]** da Smart List do Sistema e clique na guia **[!UICONTROL Pessoas]**.

   ![](assets/find-and-merge-duplicate-people-2.png)

   >[!NOTE]
   >
   >Você também pode [Localizar Pessoas Duplicadas com Lógica Personalizada](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-duplicate-people-with-custom-logic.md){target="_blank"}.

## Mesclar Pessoas Manualmente {#merge-people-manually}

>[!CAUTION]
>
>Ao mesclar pessoas, se a pessoa perdida tiver um objeto personalizado Marketo, ela _não_ será reassociada à pessoa vencedora. Reordene o objeto personalizado antes de executar a mesclagem.

1. Selecione as duplicatas mantendo pressionada a tecla Ctrl/Cmd e clicando em e depois clique em **[!UICONTROL Mesclar pessoas]**.

   ![](assets/find-and-merge-duplicate-people-3.png)

   >[!TIP]
   >
   >Você pode ter duas ou mais duplicatas para a mesma pessoa - selecione-as todas de uma vez.

1. Você verá os valores entre os registros que _não_ correspondem. Selecione o valor que deseja manter para cada campo. Clique em **[!UICONTROL Mesclar]** quando terminar. Se você não quiser nenhum valor, marque **[!UICONTROL Personalizado]** e insira um valor de sua escolha.

   ![](assets/find-and-merge-duplicate-people-4.png)

   >[!NOTE]
   >
   >Ao mesclar pessoas manualmente, a primeira pessoa selecionada será o &quot;vencedor&quot;. Portanto, na guia Pessoas, se você estiver mesclando as IDs de registro 198 e 199 e clicar primeiro em 199, 199 será a ID de registro das pessoas mescladas. Isso também se aplica se mais de dois registros forem mesclados.

   >[!TIP]
   >
   >Mesclar é melhor do que excluir. Você conservará todo o histórico (visitas à página, cliques em links, aberturas de email, preenchimentos de formulário etc.).

## Efeito no Salesforce {#effect-in-salesforce}

Se você tiver a integração do Salesforce, há algumas observações sobre o efeito da mesclagem de clientes em potencial no Salesforce.

* Ao mesclar somente clientes em potencial ou somente contatos, eles são mesclados de acordo com as regras normais do Salesforce.
* Ao mesclar clientes em potencial e contatos, todos os clientes em potencial são convertidos em contatos antes da mesclagem de acordo com as regras normais do Salesforce.

Para obter detalhes específicos do comportamento do Salesforce ao mesclar clientes em potencial ou contatos, verifique os seguintes documentos do Salesforce:

* [Mesclando Clientes Potenciais Duplicados](https://help.salesforce.com/HTViewHelpDoc?id=leads_merge.htm&amp;language=en_US){target="_blank"}
* [Mesclando Contatos Duplicados](https://help.salesforce.com/HTViewHelpDoc?id=contacts_merge.htm&amp;language=en_US){target="_blank"}

## Mesclagem em Massa {#bulk-merging}

Se você tiver muitas duplicatas para mesclar manualmente, entre em contato com a equipe de conta do Adobe (seu gerente de conta) para discutir suas opções.
