---
unique-page-id: 3571846
description: Microsoft Dynamics Sync - Sincronização de Entidade Personalizada - Documentos do Marketing - Documentação do Produto
title: Microsoft Dynamics Sync - Sincronização de Entidade Personalizada
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização de entidade personalizada {#microsoft-dynamics-sync-custom-entity-sync}

Se você precisar ativar a sincronização de entidade personalizada inicial para disponibilizar os dados do Dynamics no Marketo, veja como fazê-lo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>**Pré-requisitos**
>
>Para usar um objeto personalizado, ele deve estar associado a um [cliente potencial](microsoft-dynamics-sync-lead-sync.md), [contato](microsoft-dynamics-sync-contact-sync.md)ou [](microsoft-dynamics-sync-account-sync.md)contador no Dynamics.

>[!CAUTION]
>
>Verifique se a sincronização inicial foi concluída (você será notificado por email) antes de iniciar a sincronização para entidades personalizadas.

1. Vá para a seção Admin.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Clique em **Desativar sincronização** para desativar temporariamente a sincronização global padrão.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Instale uma versão do Microsoft Dynamics que suporte sincronização de entidade personalizada (após 2_0_0_2). Consulte Versões de plug-in [do Marketo para o Microsoft Dynamics](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).
1. Dê ao usuário de sincronização de marketing acesso de leitura a quaisquer entidades que você planeja sincronizar.
1. Em Gerenciamento de banco de dados, clique no link** Dynamics Entities Sync**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Clique no link **Sincronizar schema** para trazer a lista de entidades personalizadas disponíveis.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Após a sincronização da lista, selecione os campos que deseja sincronizar e os que deseja usar como [restrições](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/ou acionadores em listas inteligentes. Quando terminar, clique em **Ativar sincronização**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. Reative a sincronização global.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >O Marketo oferece suporte apenas a entidades personalizadas que estão vinculadas a entidades padrão de um ou dois níveis de profundidade.

   >[!NOTE]
   >
   >Os nomes das entidades podem ter no máximo** 33 caracteres**.

Você é bom!