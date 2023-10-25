---
unique-page-id: 10098379
description: Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado - Documentação do Marketo - Documentação do produto
title: Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 1%

---

# Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing ou Vendas quer um novo campo. Ou talvez tenha esquecido um na seleção de campo inicial. Ou suas necessidades mudaram. Em qualquer caso, você pode usar a Sincronização rápida para ressincronizar campos específicos.

Normalmente, você usará a Sincronização rápida para adicionar um novo campo e atualizar os valores. No entanto, há casos em que você pode querer sincronizar um campo existente. Você pode restringir a sincronização de campo com base em um intervalo de datas atualizado ou criado. Consulte [Opções de Sincronização Avançadas](#Advanced_Sync_Options) abaixo para obter detalhes.

A Sincronização Rápida pode sincronizar valores nulos. Por exemplo, se você estiver usando os valores A e B e alterar um valor B em Dinâmica para nulo, ele sincronizará o valor nulo com o Marketo.

## Sincronização rápida para todos os registros {#quick-sync-for-all-records}

Veja como usar a Sincronização rápida para ressincronizar novos campos.

1. No Marketo Engage, clique em **[!UICONTROL Admin]**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Clique em **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Em Detalhes da sincronização de campo, clique em **[!UICONTROL Editar]**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Selecione os campos para sincronização rápida e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >É possível selecionar campos de várias entidades.

1. Você receberá uma notificação quando a sincronização estiver concluída.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >A sincronização é executada lado a lado com outras sincronizações e, dependendo do tamanho do banco de dados, pode levar muito tempo para ser concluída. Quando um campo está em uma fila para sincronização, não é possível desmarcá-lo.

## Opções de Sincronização Avançadas {#advanced-sync-options}

E se você quiser sincronizar um campo existente, mas isso apenas para um conjunto limitado de dados? Veja como.

1. Desmarque a caixa de seleção de um campo existente. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Abra o pop-up novamente e selecione o campo novamente.

   ![](assets/select-field-reselect-hand.png)

1. Clique em **[!UICONTROL Sincronização avançada]**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Escolher **[!UICONTROL Atualizado]** e selecione um intervalo de datas usando os seletores de data. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Somente os registros atualizados entre 19/08/2016 e 19/09/2016 serão Sincronizados rapidamente para o campo.

## Correção de campos fora de sincronia {#fixing-out-of-sync-fields}

No raro caso em que um campo do Dynamics e do Marketo está fora de sincronia, há uma maneira rápida e fácil de ressincronizá-los.

1. Desmarque o campo e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Selecione o campo novamente e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Isso deve resolver isso!
