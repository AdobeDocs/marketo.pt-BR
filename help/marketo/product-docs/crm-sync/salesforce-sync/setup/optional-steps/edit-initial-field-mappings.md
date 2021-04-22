---
unique-page-id: 4719287
description: Editar mapeamentos de campo inicial - Documentos do Marketo - Documentação do produto
title: Editar mapeamentos de campo inicial
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Editar Mapeamentos de Campo Iniciais {#edit-initial-field-mappings}

>[!NOTE]
>
>Esse recurso só pode ser acessado antes da sincronização inicial com o Salesforce! Depois que o botão **Sync Now** é pressionado, isso não pode mais ser feito.

Durante a sincronização inicial com o Salesforce, o Marketo combina automaticamente campos personalizados com nomes semelhantes em um único campo no lado do Marketo para garantir que os dados possam ser trocados com os objetos Lead e Contact no CRM. Este artigo explica como personalizar esses mapeamentos.

## Mapear campos não mapeados {#map-unmapped-fields}

Ao visualizar um campo na pasta Campos não mapeados, significa que ele não está mapeado para um campo semelhante no Lead ou Contato no Salesforce. Você pode consertar isso.

1. Clique em **Editar mapeamentos**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Abra a pasta **Campos personalizados não mapeados**.

   ![](assets/two.png)

1. Arraste um campo personalizado não mapeado até outro para mapeá-lo.

   >[!NOTE]
   >
   >Você só pode editar mapeamentos de campos personalizados. Não é possível modificar mapeamentos de campo padrão.

   ![](assets/three.png)

1. Clique em **Concluir mapeamentos** quando terminar.

   ![](assets/four.png)

## Quebrar Mapeamento Existente {#break-existing-mapping}

Se você tiver campos com nomes semelhantes no objeto de lead e contato, o Marketo os mapeará automaticamente. Você pode considerá-las diferentes e manter dados diferentes. Quebre o mapeamento assim.

1. Clique em **Editar mapeamentos**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Realce um campo mapeado e clique em **Break Mapping** para separar os campos.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Clique em **Concluir mapeamentos** quando terminar.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Legal! Você está quase terminando a sincronização inicial.

## Redefinir esquema {#reset-schema}

1. Se você fizer algumas alterações no esquema no Salesforce ao trabalhar nos mapeamentos, poderá obter as alterações clicando em **Redefinir esquema**.

   * Todas as alterações de mapeamento serão redefinidas!
   * A redefinição do esquema só adicionará campos, e não removerá (mesmo se você ocultá-los do usuário de sincronização).
   ![](assets/image2014-12-9-13-3a32-3a8.png)
