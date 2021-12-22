---
unique-page-id: 2953384
description: Habilitar sincronização para uma entidade personalizada - Documentos do Marketo - Documentação do produto
title: Ativar Sincronização para uma Entidade Personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: a5bc634bd3b5ec0849617a9fe366a106691ce149
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Ativar Sincronização para uma Entidade Personalizada {#enable-sync-for-a-custom-entity}

Se você precisar que dados de entidade personalizados do Dynamics estejam disponíveis no Marketo, veja como habilitar a sincronização para ela:

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Quando a sincronização é ativada para uma entidade personalizada, o Marketo executa uma sincronização inicial para trazer todos os dados do Objeto personalizado.

1. Vá para o **Administrador** seção.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Selecionar **Microsoft Dynamics** e clique em **Desativar Sincronização**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Você deve desativar temporariamente a sincronização global para ativar ou desativar uma entidade personalizada.

1. Em Gerenciamento de banco de dados, clique no botão **Sincronização de entidades do Dynamics** link .

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Clique no botão **Esquema de sincronização** link .

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Selecione a entidade que deseja sincronizar e clique em **Ativar Sincronização**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Selecione os campos que deseja sincronizar ou usar como [restrições](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/ou acionadores em listas inteligentes. Quando terminar, clique em **Ativar Sincronização**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante o processo de sincronização, você pode notar que o item &quot;Sincronização de entidades dinâmicas&quot; desaparece da árvore de navegação. Esse é um comportamento esperado e reaparecerá após a conclusão da sincronização.

1. A entidade agora tem uma marca de seleção verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Não se esqueça de reativar a sincronização global!

   ![](assets/enable-sync-for-a-custom-entity-8.png)

