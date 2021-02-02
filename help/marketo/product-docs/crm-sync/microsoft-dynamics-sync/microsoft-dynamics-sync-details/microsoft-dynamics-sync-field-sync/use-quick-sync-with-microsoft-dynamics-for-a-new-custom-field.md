---
unique-page-id: 10098379
description: Usar sincronização rápida com o Microsoft Dynamics para um novo campo personalizado - Documentos de marketing - Documentação do produto
title: Usar sincronização rápida com o Microsoft Dynamics para um novo campo personalizado
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Usar sincronização rápida com o Microsoft Dynamics para um novo campo personalizado {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing ou Vendas querem um novo campo. Ou, talvez você tenha esquecido um na sua seleção inicial de campo. Ou suas necessidades mudaram. Em qualquer caso, você pode usar a Sincronização rápida para ressincronizar campos específicos.

Normalmente, você usa a sincronização rápida para adicionar um novo campo e atualizar os valores. No entanto, há casos em que você pode querer sincronizar um campo existente. É possível restringir a sincronização de campos com base em um intervalo de datas atualizado ou criado. Consulte [Opções de sincronização avançadas](#Advanced_Sync_Options) abaixo para obter detalhes.

A sincronização rápida pode sincronizar valores nulos. Por exemplo, se você estiver usando os valores A e B e alterar um valor B no Dynamics para nulo, ele sincronizará o valor nulo para Marketo.

## Sincronização rápida para todos os registros {#quick-sync-for-all-records}

Veja como usar a sincronização rápida para ressincronizar novos campos.

1. Em Marketo, clique em **Admin**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Clique em **Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Em Detalhes de sincronização de campo, clique em **Editar**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Selecione os campos para sincronização rápida e clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >É possível selecionar campos de várias entidades.

1. Você receberá uma notificação quando a sincronização for concluída.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >A sincronização é executada lado a lado com outras sincronizações e, dependendo do tamanho do banco de dados, pode levar muito tempo para ser concluída. Quando um campo está em uma fila para sincronização, não é possível desmarcá-lo.

## Opções de sincronização avançadas {#advanced-sync-options}

E se você quiser sincronizar um campo existente, mas somente para um conjunto limitado de dados? Veja como.

1. Desmarque a caixa de seleção de um campo existente. Clique em **Salvar**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Abra o pop-up novamente e selecione novamente o campo.

   ![](assets/select-field-reselect-hand.png)

1. Clique em **Sincronização avançada**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Escolha **Atualizado** e selecione um intervalo de datas usando os seletores de datas. Clique em **Salvar**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Somente os registros atualizados entre 19/08/16 e 19/09/16 serão sincronizados rapidamente para o campo.

## Correção de campos fora de sincronização {#fixing-out-of-sync-fields}

No raro caso em que um campo Dinâmico e de Mercado está fora de sincronia, há uma maneira rápida e fácil de ressincronizá-los.

1. Desmarque o campo e clique em **Salvar**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Selecione novamente o campo e clique em **Salvar**. Isso é tudo!

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Isso deveria consertar isso!
