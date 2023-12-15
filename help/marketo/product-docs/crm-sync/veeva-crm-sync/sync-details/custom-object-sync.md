---
description: Sincronização de objeto personalizado - Documentação do Marketo - Documentação do produto
title: Sincronização de objeto personalizado
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Sincronização de objeto personalizado {#custom-object-sync}

Objetos personalizados criados em sua instância do Veeva CRM também podem fazer parte do Marketo Engage. Veja como configurar isso.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve ser associado a um contato ou objeto de conta no Veeva CRM.

## Habilitar objeto personalizado {#enable-custom-object}

1. No Marketo, clique em **[!UICONTROL Admin]**, depois **[!UICONTROL Sincronização de objetos Veeva]**.

   ![](assets/custom-object-sync-1.png)

1. Se este for seu primeiro Objeto Personalizado, clique em **[!UICONTROL Esquema de sincronização]**.

   ![](assets/custom-object-sync-2.png)

1. Clique em **[!UICONTROL Desabilitar Sincronização Global]**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >A sincronização inicial do esquema do objeto personalizado Veeva pode levar alguns minutos.

1. Arraste o objeto personalizado que você deseja sincronizar para a tela de desenho.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Os objetos personalizados devem ter nomes exclusivos. O Marketo não oferece suporte a dois objetos personalizados diferentes com o mesmo nome.

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/custom-object-sync-5.png)

1. Clique em **[!UICONTROL Habilitar sincronização]** novamente.

   ![](assets/custom-object-sync-6.png)

1. Volte para o **[!UICONTROL Veeva]** guia.

   ![](assets/custom-object-sync-7.png)

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/custom-object-sync-8.png)

1. Para exibir todos os objetos personalizados Veeva, clique em **[!UICONTROL Admin]** e **[!UICONTROL Sincronização de objetos Veeva]**.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >O Marketo só oferece suporte a entidades personalizadas vinculadas a entidades padrão de um a dois níveis de profundidade.

Excelente! Agora você pode usar dados desse objeto personalizado em Campanhas inteligentes e Smart Lists.

>[!MORELIKETHIS]
>
>* [Sincronizando Mensagens de Chamada e Chave de Chamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Adicionar/Remover Campo de Objeto Personalizado como Smart List/Restrições do Acionador](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
