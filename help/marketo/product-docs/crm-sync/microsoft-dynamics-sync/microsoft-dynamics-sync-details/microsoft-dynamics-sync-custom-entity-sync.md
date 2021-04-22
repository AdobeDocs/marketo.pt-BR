---
unique-page-id: 3571846
description: Sincronização do Microsoft Dynamics - Sincronização de entidade personalizada - Documentos do Marketo - Documentação do produto
title: Sincronização do Microsoft Dynamics - Sincronização de Entidade Personalizada
exl-id: 1e175bd4-509f-4c1f-a41d-456629e4a8fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Sincronização do Microsoft Dynamics: Sincronização de entidade personalizada {#microsoft-dynamics-sync-custom-entity-sync}

Se você precisar ativar a sincronização de entidade personalizada inicial para disponibilizar dados do Dynamics no Marketo, veja a seguir como fazê-lo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve ser associado a um objeto [lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md), [contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md) ou [account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)no Dynamics.

>[!CAUTION]
>
>Certifique-se de que a sincronização inicial está concluída (você será notificado por email) antes de iniciar a sincronização para entidades personalizadas.

1. Acesse a seção Admin .

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Clique em **Desativar Sincronização** para desativar temporariamente a sincronização global padrão.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Instale uma versão do Microsoft Dynamics que suporta sincronização de entidade personalizada (após 2_0_0_2). Consulte [Versões de plug-in do Marketo para o MIcrosoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).

1. Forneça ao Usuário do Marketo Sync acesso de leitura a quaisquer entidades que você planeja sincronizar.

1. Em Gerenciamento de Banco de Dados, clique no link **Sincronização de Entidades Dinâmicas**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Clique no link **Sync schema** para trazer a lista de entidades personalizadas disponíveis.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Depois que a lista sincronizar, selecione os campos que deseja sincronizar e aqueles que deseja usar como [restrições](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/ou acionadores em listas inteligentes. Quando terminar, clique em **Ativar Sincronização**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. Reative a sincronização global.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >O Marketo suporta apenas entidades personalizadas vinculadas a entidades padrão com profundidade de um ou dois níveis.

   >[!NOTE]
   >
   >Os nomes de entidade podem ter no máximo **33 caracteres**.

Você é bom!
