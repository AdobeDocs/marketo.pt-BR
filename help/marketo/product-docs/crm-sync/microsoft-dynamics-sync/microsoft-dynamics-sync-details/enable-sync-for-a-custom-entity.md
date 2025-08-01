---
unique-page-id: 2953384
description: Habilitar sincronização para uma entidade personalizada - Documentação do Marketo - Documentação do produto
title: Habilitar Sincronização para uma Entidade Personalizada
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 4f36194fb76fd8e26c2fd6fe49526d88d355a24a
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Habilitar Sincronização para uma Entidade Personalizada {#enable-sync-for-a-custom-entity}

Se você precisa que os dados de entidade personalizados de [!DNL Dynamics] estejam disponíveis no Marketo Engage, veja como habilitar a sincronização para eles.

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve ser associado a um objeto [lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md){target="_blank"} ou [account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md){target="_blank"} na Microsoft Dynamics.

>[!NOTE]
>
>* Quando você habilita a sincronização de uma entidade personalizada, o Marketo executa uma sincronização inicial para trazer todos os dados do Objeto personalizado.
>* A Lista de Marketing e os Membros da Lista de Marketing _não são suportados_ no momento.

>[!IMPORTANT]
>
>O usuário de sincronização do Marketo precisa de acesso de leitura ao objeto personalizado para listá-lo e executar uma sincronização nele.

1. Vá para a seção **[!UICONTROL Admin]**.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Selecione **[!UICONTROL Microsoft Dynamics]** e clique em **[!UICONTROL Desabilitar sincronização]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Você deve desabilitar a sincronização global temporariamente para habilitar ou desabilitar uma entidade personalizada.

1. Em [!UICONTROL Gerenciamento de Banco de Dados], clique no link **[!UICONTROL Sincronização de Entidades do Dynamics]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Clique no link **[!UICONTROL Sincronizar esquema]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Selecione a entidade que deseja sincronizar e clique em **[!UICONTROL Habilitar Sincronização]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Selecione os campos que deseja sincronizar ou usar como [restrições](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/ou acionadores em listas inteligentes. Quando terminar, clique em **[!UICONTROL Habilitar Sincronização]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante o processo de sincronização, você pode notar que o item &quot;[!UICONTROL Sincronização de Entidades Dinâmicas]&quot; desaparece da árvore de navegação. Esse comportamento é esperado e reaparecerá após a conclusão da sincronização.

1. A entidade agora tem uma marca de seleção verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Não se esqueça de reativar a sincronização global!

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* O Marketo só oferece suporte a entidades personalizadas vinculadas a entidades padrão com um ou dois níveis de profundidade.
   >
   >* A árvore de objetos personalizados pode mostrar o mesmo objeto mais de uma vez, devido às suas conexões diretas com um dos objetos principais (por exemplo, clientes potenciais, contatos ou contas, ou conexões indiretas por meio de objetos intermediários). Nesses casos, escolha o objeto mais próximo do objeto principal e escolha apenas um. Escolher o mesmo objeto várias vezes pode dificultar a sincronização desse objeto personalizado.
