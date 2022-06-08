---
unique-page-id: 2953471
description: Sincronização SFDC - Sincronização de Objeto Personalizado - Documentos do Marketo - Documentação do produto
title: Sincronização SFDC - Sincronização de Objeto Personalizado
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---

# Sincronização SFDC: Sincronização de Objeto Personalizado {#sfdc-sync-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketo.  Veja como configurar.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve estar associado a um [cliente potencial](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contato](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)ou [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) no Salesforce.

## Ativar Objeto Personalizado  {#enable-custom-object}

1. Clique em **Administrador** e **Sincronização de Objetos do Salesforce** link .

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se este for seu primeiro Objeto Personalizado, clique em **Esquema de sincronização**.

   ![](assets/rtaimage-2.png)

1. Clique em **Desativar Sincronização Global**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Uma sincronização inicial do esquema de objeto personalizado do Salesforce pode levar alguns minutos.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Arraste o objeto personalizado que deseja sincronizar na tela.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Os objetos personalizados devem ter nomes exclusivos. O Marketo não suporta dois objetos personalizados diferentes com o mesmo nome.

1. Clique em **Ativar Sincronização**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Clique em **Ativar Sincronização** novamente.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Não se esqueça de reativar sua sincronização global!

1. Volte para o **Salesforce** guia .

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Clique em **Ativar Sincronização**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Para exibir todos os objetos personalizados do Salesforce, clique em **Administrador** e **Sincronização de Objetos do Salesforce** link (o mesmo que na etapa 1 acima).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >O Marketo suporta apenas entidades personalizadas vinculadas a entidades padrão com profundidade de um ou dois níveis.

### O que vem a seguir: {#whats-next}

[Adicionar/remover campo de objeto personalizado como restrições de lista inteligente/acionador](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Excelente! Agora é possível usar dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.
