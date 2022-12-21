---
unique-page-id: 4719297
description: Ativar/desativar sincronização de objetos personalizados - Documentos do Marketo - Documentação do produto
title: Ativar/Desativar Sincronização de Objeto Personalizado
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 1%

---

# Ativar/Desativar Sincronização de Objeto Personalizado {#enable-disable-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketo. Veja como configurar.

## Ativar/Desativar Sincronização de Objeto Personalizado {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>É necessário ter direitos de administrador.

1. Clique em **Administrador**.

   ![](assets/one.png)

1. No menu Gerenciamento de Banco de Dados, clique em **Sincronização de Objetos do Salesforce**.

   ![](assets/two-2.png)

1. Se este for seu primeiro Objeto Personalizado, clique em **Esquema de sincronização.** Caso contrário, clique em **Atualizar esquema** para garantir que você tenha o mais recente.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se a sincronização global estiver em execução, você terá que desativá-la clicando em **Desativar Sincronização Global.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Uma sincronização do esquema de objeto personalizado do Salesforce pode levar alguns minutos.

1. Clique em **Atualizar esquema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selecione o objeto que deseja sincronizar e clique em **Ativar Sincronização**.

   >[!TIP]
   >
   >O Marketo só poderá sincronizar um objeto personalizado se ele tiver um relacionamento direto com o objeto de Cliente Potencial, Contato ou Conta no Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Clique em **Ativar Sincronização** novamente.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Volte para o **Salesforce** e clique em **Ativar Sincronização**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Uso de objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>Não é possível usar objetos personalizados em campanhas inteligentes com acionadores.

1. Na sua lista inteligente, arraste o **Tem oportunidade** filtrar e definir como **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Em seguida, use as restrições de filtro para limitar o foco.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excelente! Agora você pode usar os dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.

>[!MORELIKETHIS]
>
>[Adicionar/remover campo de objeto personalizado como restrições de lista inteligente/acionador](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
