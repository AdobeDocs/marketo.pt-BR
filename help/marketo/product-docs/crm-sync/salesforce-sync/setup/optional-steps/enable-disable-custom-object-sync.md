---
unique-page-id: 4719297
description: Ativar/desativar a sincronização de objetos personalizados - Documentação do Marketo - Documentação do produto
title: Habilitar/Desabilitar a Sincronização de Objetos Personalizados
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 6293a11b9d48a20da4cb2448c8374c469679abdb
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Habilitar/Desabilitar a Sincronização de Objetos Personalizados {#enable-disable-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketo Engage. Veja como configurar isso.

## Habilitar/Desabilitar a Sincronização de Objetos Personalizados {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. No menu Gerenciamento de Banco de Dados, clique em **[!UICONTROL Sincronização de Objetos do Salesforce]**.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Se este for seu primeiro Objeto Personalizado, clique em **[!UICONTROL Sincronizar esquema]**. Caso contrário, clique em **[!UICONTROL Atualizar esquema]** para verificar se você tem o mais recente.

   ![](assets/enable-disable-custom-object-sync-3.png)

1. Se sua sincronização global estiver em execução, você terá que desabilitá-la clicando em **[!UICONTROL Desabilitar Sincronização Global]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >A sincronização do esquema do objeto personalizado do Salesforce pode levar alguns minutos.

1. Clique em **[!UICONTROL Atualizar Esquema]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selecione o objeto que deseja sincronizar e clique em **[!UICONTROL Habilitar Sincronização]**.

   >[!TIP]
   >
   >O Marketo só pode sincronizar um objeto personalizado se tiver uma relação direta com o objeto Cliente potencial, Contato ou Conta no Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Clique em **[!UICONTROL Habilitar Sincronização]** novamente.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Volte para a guia **[!DNL Salesforce]** e clique em **[!UICONTROL Habilitar Sincronização]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Usar seus objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>Não é possível usar objetos personalizados em Campanhas inteligentes com acionadores.

1. Em sua Smart List, arraste sobre o filtro **[!UICONTROL Tem oportunidade]** e defina como **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Em seguida, use restrições de filtro para restringir o foco.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excelente! Agora você pode usar os dados desse objeto personalizado em Campanhas inteligentes e Smart Lists.

>[!MORELIKETHIS]
>
>[Adicionar/Remover Campo de Objeto Personalizado como Lista Inteligente/Restrições do Acionador](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
