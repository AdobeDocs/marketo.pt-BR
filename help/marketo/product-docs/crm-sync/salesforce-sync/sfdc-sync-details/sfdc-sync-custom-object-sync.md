---
unique-page-id: 2953471
description: SFDC Sync - Sincronização de objeto personalizado - Documentação do Marketo - Documentação do produto
title: Sincronização do SFDC - Sincronização de objeto personalizado
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 79ae0d56dd4bb8bf563c6546cba54b89b5841425
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Sincronização do SFDC: Sincronização de Objeto Personalizado {#sfdc-sync-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketo Engage. Veja como configurar isso.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve ser associado a um objeto [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"} ou [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"} na Salesforce.

>[!IMPORTANT]
>
>O usuário de sincronização do Marketo precisa de acesso de leitura ao objeto personalizado para listá-lo e executar uma sincronização nele.

## Habilitar objeto personalizado  {#enable-custom-object}

1. Clique em **[!UICONTROL Admin]** e no link **[!UICONTROL Salesforce Objects Sync]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se este for seu primeiro Objeto Personalizado, clique em **[!UICONTROL Sincronizar Esquema]**.

   ![](assets/rtaimage-2.png)

1. Clique em **[!UICONTROL Desabilitar sincronização global]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >A sincronização inicial do esquema do objeto personalizado do Salesforce pode levar alguns minutos.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Arraste o objeto personalizado que você deseja sincronizar para a tela de desenho.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Os objetos personalizados devem ter nomes exclusivos. O Marketo não oferece suporte a dois objetos personalizados diferentes com o mesmo nome.

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Clique em **[!UICONTROL Habilitar Sincronização]** novamente.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Não se esqueça de reativar a sincronização global.

1. Volte para a guia **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Para exibir todos os objetos personalizados do Salesforce, clique em **[!UICONTROL Admin]** e no link **[!UICONTROL Salesforce Objects Sync]** (o mesmo que a etapa 1 acima).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* O Marketo só oferece suporte a entidades personalizadas vinculadas a entidades padrão com um ou dois níveis de profundidade.
   >
   >* A árvore de objetos personalizados pode mostrar o mesmo objeto mais de uma vez, devido às suas conexões diretas com um dos objetos principais (por exemplo, clientes potenciais, contatos ou contas, ou conexões indiretas por meio de objetos intermediários). Nesses casos, escolha o objeto mais próximo do objeto principal e escolha apenas um. Escolher o mesmo objeto várias vezes pode dificultar a sincronização desse objeto personalizado.

### O que vem a seguir: {#whats-next}

[Adicionar/Remover Campo de Objeto Personalizado como Lista Inteligente/Restrições do Acionador](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Excelente! Agora você pode usar dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.
