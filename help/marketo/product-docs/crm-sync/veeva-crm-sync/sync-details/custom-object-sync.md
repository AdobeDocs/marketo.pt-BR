---
description: Saiba como configurar a sincronização de objetos personalizados do Veeva CRM para o Marketo Engage. Habilite objetos personalizados no Admin e use-os em Smart Lists e acionadores.
title: Sincronização de objeto personalizado
hide: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/RmyCIMm3TKbcO3nPcqyZqbWZl1dnJ6Au4HsuURJjcKU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 217
ht-degree: 2%

---

# Sincronização de objeto personalizado {#custom-object-sync}

Objetos personalizados criados em sua instância do CRM [!DNL Veeva] também podem fazer parte do Marketo Engage. Veja como configurar isso.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve estar associado a um contato ou objeto de conta no [!DNL Veeva] CRM.

## Habilitar objeto personalizado {#enable-custom-object}

1. No Marketo, clique em **[!UICONTROL Admin]** e depois em **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/custom-object-sync-1.png)

1. Se este for seu primeiro Objeto Personalizado, clique em **[!UICONTROL Sincronizar Esquema]**.

   ![](assets/custom-object-sync-2.png)

1. Clique em **[!UICONTROL Desabilitar sincronização global]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >A sincronização inicial do esquema do objeto personalizado [!DNL Veeva] pode levar alguns minutos.

1. Arraste o objeto personalizado que você deseja sincronizar para a tela de desenho.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Os objetos personalizados devem ter nomes exclusivos. O Marketo não oferece suporte a dois objetos personalizados diferentes com o mesmo nome.

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/custom-object-sync-5.png)

1. Clique em **[!UICONTROL Habilitar Sincronização]** novamente.

   ![](assets/custom-object-sync-6.png)

1. Volte para a guia **[!UICONTROL Veeva]**.

   ![](assets/custom-object-sync-7.png)

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/custom-object-sync-8.png)

1. Para exibir todos os seus [!DNL Veeva] objetos personalizados, clique em **[!UICONTROL Admin]** e **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >O Marketo só oferece suporte a entidades personalizadas vinculadas a entidades padrão de um a dois níveis de profundidade.

Excelente! Agora você pode usar dados desse objeto personalizado em Campanhas inteligentes e Smart Lists.

>[!MORELIKETHIS]
>
>* [Sincronizando Mensagens de Chamada e Chave de Chamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Adicionar/Remover Campo de Objeto Personalizado como Lista Inteligente/Restrições do Acionador](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
