---
description: Ativar/desativar a sincronização de objetos personalizados - Documentação do Marketo - Documentação do produto
title: Habilitar/Desabilitar a Sincronização de Objetos Personalizados
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Habilitar/Desabilitar a Sincronização de Objetos Personalizados {#enable-disable-custom-object-sync}

Objetos personalizados criados em sua instância do Veeva CRM também podem fazer parte do Marketo Engage. Veja como configurar isso.

## Ativar ou desativar a sincronização de objetos personalizados {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. No Marketo, clique em **[!UICONTROL Admin]** e depois em **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Se este for seu primeiro Objeto personalizado, clique em Sincronizar esquema. Caso contrário, clique em **[!UICONTROL Atualizar esquema]** para garantir que você tenha o mais recente.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Se sua sincronização global estiver em execução, desabilite-a clicando em **[!UICONTROL Desabilitar Sincronização Global]**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >Uma sincronização do esquema de objeto personalizado Veeva pode levar alguns minutos.

1. Clique em **[!UICONTROL Atualizar Esquema]**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Selecione o objeto que deseja sincronizar e clique em Habilitar Sincronização.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>O Marketo só pode sincronizar um objeto personalizado se tiver uma relação direta com o objeto Contato ou Conta no Veeva CRM.

1. Clique em **[!UICONTROL Habilitar Sincronização]** novamente.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Volte para a guia Veeva e clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Usar seus objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>Não é possível usar objetos personalizados em campanhas inteligentes com acionadores.

1. Em sua Smart List, arraste sobre o filtro &quot;Tem oportunidade&quot; e defina como **[!UICONTROL Verdadeiro]**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Como opção, use restrições de filtro para restringir o foco.

   ![](assets/enable-disable-custom-object-sync-9.png)

Excelente! Agora você pode usar os dados desse objeto personalizado em Campanhas inteligentes e Smart Lists.

>[!MORELIKETHIS]
>
>[Adicionar/Remover Campo de Objeto Personalizado como Lista Inteligente/Restrições do Acionador](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
