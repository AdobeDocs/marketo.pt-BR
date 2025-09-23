---
unique-page-id: 4719287
description: Editar mapeamentos de campo iniciais - Documentação do Marketo - Documentação do produto
title: Editar mapeamentos de campo iniciais
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 3%

---

# Editar mapeamentos de campo iniciais {#edit-initial-field-mappings}

>[!NOTE]
>
>Esse recurso só é acessível antes da sincronização inicial com o Salesforce. Depois que o botão **[!UICONTROL Sincronizar Agora]** for pressionado, isso não poderá mais ser feito.

Durante a sincronização inicial com o Salesforce, o Marketo Engage combina automaticamente campos personalizados com nomes semelhantes em um único campo no lado do Marketo para garantir que os dados possam ser trocados com objetos de Cliente Potencial e de Contato no CRM. Este artigo explica como personalizar esses mapeamentos.

## Mapear campos não mapeados {#map-unmapped-fields}

Quando você vê um campo na pasta [!UICONTROL Campos não mapeados], significa que ele não está mapeado para um campo semelhante no cliente potencial ou contato no Salesforce. Você pode consertar isso.

1. Clique em **[!UICONTROL Editar Mapeamentos]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Abra a pasta **[!UICONTROL Campos Personalizados Não Mapeados]**.

   ![](assets/two.png)

1. Arraste um campo personalizado não mapeado para outro para mapeá-los juntos.

   >[!NOTE]
   >
   >Você só pode editar mapeamentos de campos personalizados. Não é possível modificar os mapeamentos de campo padrão.

   ![](assets/three.png)

1. Clique em **[!UICONTROL Concluir Mapeamentos]** quando terminar.

   ![](assets/four.png)

## Interromper mapeamento existente {#break-existing-mapping}

Se você tiver campos nomeados de forma semelhante no cliente potencial e no objeto de contato, o Marketo os mapeará automaticamente. Você pode considerá-los diferentes e manter dados diferentes. Quebre o mapeamento assim.

1. Clique em **[!UICONTROL Editar Mapeamentos]**.

   ![](assets/image2014-12-9-13-3a31-3a37.png)

1. Realce um campo mapeado e clique em **[!UICONTROL Quebrar mapeamento]** para separar os campos.

   ![](assets/image2014-12-9-13-3a31-3a47.png)

1. Clique em **[!UICONTROL Concluir Mapeamentos]** quando terminar.

   ![](assets/image2014-12-9-13-3a31-3a58.png)

   Legal! Você está quase terminando a sincronização inicial.

## Redefinir esquema {#reset-schema}

1. Se você fizer algumas alterações no esquema no Salesforce enquanto estiver trabalhando nos mapeamentos, poderá obter as alterações clicando em **[!UICONTROL Redefinir Esquema]**.

   * Todas as alterações de mapeamento serão redefinidas.
   * A redefinição do esquema só adicionará campos, não removerá (mesmo se você os ocultar do usuário de sincronização).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
