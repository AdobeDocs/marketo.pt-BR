---
unique-page-id: 2953471
description: Sincronização de SFDC - Sincronização de objeto personalizado - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de Objeto Personalizado
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 0%

---

# Sincronização do SFDC: Sincronização de Objeto Personalizado {#sfdc-sync-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketo Engage. Veja como configurar isso.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve estar associado a um [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}, or [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"} objeto no Salesforce.

>[!IMPORTANT]
>
>O usuário de sincronização do Marketo precisa de acesso de leitura ao objeto personalizado para listá-lo e executar uma sincronização nele.

## Habilitar objeto personalizado  {#enable-custom-object}

1. Clique em **[!UICONTROL Admin]** e a variável **[!UICONTROL Sincronização de objetos do Salesforce]** link.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se este for seu primeiro Objeto Personalizado, clique em **[!UICONTROL Esquema de sincronização]**.

   ![](assets/rtaimage-2.png)

1. Clique em **[!UICONTROL Desabilitar Sincronização Global]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Uma sincronização inicial do esquema de objeto personalizado do Salesforce pode levar alguns minutos.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Arraste o objeto personalizado que você deseja sincronizar para a tela de desenho.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Os objetos personalizados devem ter nomes exclusivos. O Marketo não oferece suporte a dois objetos personalizados diferentes com o mesmo nome.

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Clique em **[!UICONTROL Habilitar sincronização]** novamente.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Não se esqueça de reativar a sincronização global.

1. Volte para o **Salesforce** guia.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Para exibir todos os objetos personalizados do Salesforce, clique em **[!UICONTROL Admin]** e a variável **[!UICONTROL Sincronização de objetos do Salesforce]** (igual à etapa 1 acima).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >O Marketo só oferece suporte a entidades personalizadas vinculadas a entidades padrão com um ou dois níveis de profundidade.

### O que vem a seguir: {#whats-next}

[Adicionar/Remover Campo de Objeto Personalizado como Smart List/Restrições do Acionador](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Excelente! Agora você pode usar dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.
