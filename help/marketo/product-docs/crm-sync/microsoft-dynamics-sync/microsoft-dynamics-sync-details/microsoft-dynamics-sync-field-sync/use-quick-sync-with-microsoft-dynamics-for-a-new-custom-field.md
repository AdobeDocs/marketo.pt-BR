---
unique-page-id: 10098379
description: Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado - Documentos do Marketo - Documentação do produto
title: Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# Usar a sincronização rápida com o Microsoft Dynamics para um novo campo personalizado {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing ou Vendas querem um novo campo. Ou talvez você tenha esquecido um na seleção inicial de campo. Ou suas necessidades mudaram. Em qualquer caso, você pode usar a Sincronização rápida para ressincronizar campos específicos.

Normalmente, você usará a Sincronização rápida para adicionar um novo campo e ter os valores atualizados. No entanto, há casos em que você pode querer sincronizar um campo existente. Você pode restringir a sincronização de campos com base em um intervalo de datas atualizado ou criado. Consulte [Opções de sincronização avançadas](#Advanced_Sync_Options) abaixo para obter detalhes.

O Quick Sync pode sincronizar valores nulos. Por exemplo, se você estiver usando os valores A e B e alterar um valor B no Dynamics para nulo, o valor nulo será sincronizado com o Marketo.

## Sincronização rápida para todos os registros {#quick-sync-for-all-records}

Veja como usar a Sincronização rápida para ressincronizar novos campos.

1. No Marketo, clique em **Administrador**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Clique em **Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. Em Detalhes de Sincronização de Campo, clique em **Editar**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Selecione os campos para sincronização rápida e clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >Você pode selecionar campos de várias entidades.

1. Você receberá uma notificação quando a sincronização for concluída.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >A sincronização é executada lado a lado com outras sincronizações e, dependendo do tamanho do banco de dados, pode levar muito tempo para ser concluída. Quando um campo está em uma fila para sincronização, você não pode desmarcá-lo.

## Opções de sincronização avançadas {#advanced-sync-options}

E se você quiser sincronizar um campo existente, mas fizer isso apenas para um conjunto limitado de dados? Veja como.

1. Desmarque a caixa de seleção de um campo existente. Clique em **Salvar**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Abra a pop-up novamente e selecione novamente o campo.

   ![](assets/select-field-reselect-hand.png)

1. Clique em **Sincronização avançada**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Choose **Atualizado** e selecione um intervalo de datas usando os seletores de data. Clique em **Salvar**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Somente os registros atualizados entre 19/8/16 e 19/09/16 serão sincronizados rapidamente para o campo .

## Correção de campos fora de sincronização {#fixing-out-of-sync-fields}

No raro caso em que um campo do Dynamics e do Marketo está fora de sincronia, há uma maneira rápida e fácil de ressincronizá-los.

1. Desmarque o campo e clique em **Salvar**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Remarque o campo e clique em **Salvar**. Isso é tudo!

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Isso deveria consertar!
