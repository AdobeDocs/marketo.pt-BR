---
unique-page-id: 2953384
description: Habilitar sincronização para uma entidade personalizada - Documentação do Marketo - Documentação do produto
title: Habilitar Sincronização para uma Entidade Personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Habilitar Sincronização para uma Entidade Personalizada {#enable-sync-for-a-custom-entity}

Se você precisar que os dados de entidade personalizados do Dynamics estejam disponíveis no Marketo, veja como habilitar a sincronização para eles.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>* Quando você habilita a sincronização de uma entidade personalizada, o Marketo executa uma sincronização inicial para trazer todos os dados do Objeto personalizado.
>* A Lista de marketing e os Membros da Lista de marketing são **não suportado** neste momento.

>[!IMPORTANT]
>
>O usuário de sincronização do Marketo precisa de acesso de leitura ao objeto personalizado para listá-lo e executar uma sincronização nele.

1. Vá para a **Admin** seção.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Selecionar **Microsoft Dynamics** e clique em **Desativar sincronização**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Você deve desabilitar a sincronização global temporariamente para habilitar ou desabilitar uma entidade personalizada.

1. Em Gerenciamento de Banco de Dados, clique na guia **Sincronização de Entidades do Dynamics** link.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Clique em **Sincronizar esquema** link.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Selecione a entidade que deseja sincronizar e clique em **Habilitar sincronização**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Selecione os campos que deseja sincronizar ou usar como [restrições](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/ou acionadores em smart lists. Quando terminar, clique em **Habilitar sincronização**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante o processo de sincronização, você pode notar que o item &quot;Sincronização dinâmica de entidades&quot; desaparece da árvore de navegação. Esse comportamento é esperado e reaparecerá após a conclusão da sincronização.

1. A entidade agora tem uma marca de seleção verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Não se esqueça de reativar a sincronização global!

   ![](assets/enable-sync-for-a-custom-entity-8.png)
