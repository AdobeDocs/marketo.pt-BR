---
unique-page-id: 4719297
description: Ativar/desativar a sincronização de objetos personalizados - Documentação do Marketo - Documentação do produto
title: Habilitar/Desabilitar a Sincronização de Objetos Personalizados
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

---

# Habilitar/Desabilitar a Sincronização de Objetos Personalizados {#enable-disable-custom-object-sync}

Os objetos personalizados criados na sua instância do Salesforce também podem fazer parte do Marketo. Veja como configurar isso.

## Habilitar/Desabilitar a Sincronização de Objetos Personalizados {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>É necessário ter direitos de administrador.

1. Clique em **Admin**.

   ![](assets/one.png)

1. No menu Gerenciamento de banco de dados, clique em **Sincronização de objetos do Salesforce**.

   ![](assets/two-2.png)

1. Se este for seu primeiro Objeto Personalizado, clique em **Sincronizar esquema.** Caso contrário, clique **Atualizar esquema** para garantir que você tenha a versão mais recente.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se sua sincronização global estiver em execução, será necessário desabilitá-la clicando em **Desabilitar Sincronização Global.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >A sincronização do esquema de objeto personalizado do Salesforce pode levar alguns minutos.

1. Clique em **Atualizar esquema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selecione o objeto que deseja sincronizar e clique em **Habilitar sincronização**.

   >[!TIP]
   >
   >O Marketo só pode sincronizar um objeto personalizado se tiver uma relação direta com o objeto Cliente potencial, Contato ou Conta no Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Clique em **Habilitar sincronização** novamente.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Volte para o **Salesforce** e clique em **Habilitar sincronização**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Usar seus objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>Não é possível usar objetos personalizados em campanhas inteligentes com acionadores.

1. Na lista inteligente, arraste sobre a **Tem oportunidade** filtrar e definir como **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Em seguida, use restrições de filtro para restringir o foco.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excelente! Agora você pode usar os dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.

>[!MORELIKETHIS]
>
>[Adicionar/Remover Campo de Objeto Personalizado como Smart List/Restrições do Acionador](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
