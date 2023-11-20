---
unique-page-id: 4719287
description: Editar mapeamentos de campo iniciais - Documentação do Marketo - Documentação do produto
title: Editar mapeamentos de campo iniciais
exl-id: 320613d1-3845-4e05-a704-0db0f8027dc8
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Editar mapeamentos de campo iniciais {#edit-initial-field-mappings}

>[!NOTE]
>
>Esse recurso só pode ser acessado antes da sincronização inicial com o Salesforce. Quando a variável **[!UICONTROL Sincronizar agora]** for pressionado, isso não poderá mais ser feito.

Durante a sincronização inicial com o Salesforce, o Marketo Engage combina automaticamente campos personalizados com nomes semelhantes em um único campo no lado do Marketo para garantir que os dados possam ser trocados com objetos de cliente potencial e de contato no CRM. Este artigo explica como personalizar esses mapeamentos.

## Mapear campos não mapeados {#map-unmapped-fields}

Quando você vir um campo na variável [!UICONTROL Campos não mapeados] significa que não está mapeado para um campo semelhante no cliente potencial ou contato no Salesforce. Você pode consertar isso.

1. Clique em **[!UICONTROL Editar Mapeamentos]**.

![](assets/image2014-12-9-13-3a31-3a0.png)

1. Abra o **[!UICONTROL Campos personalizados não mapeados]** pasta.

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

1. Se fizer algumas alterações no esquema do Salesforce ao trabalhar nos mapeamentos, você poderá extrair as alterações clicando em **[!UICONTROL Redefinir esquema]**.

   * Todas as alterações de mapeamento serão redefinidas.
   * A redefinição do esquema só adicionará campos, não removerá (mesmo se você os ocultar do usuário de sincronização).

   ![](assets/image2014-12-9-13-3a32-3a8.png)
