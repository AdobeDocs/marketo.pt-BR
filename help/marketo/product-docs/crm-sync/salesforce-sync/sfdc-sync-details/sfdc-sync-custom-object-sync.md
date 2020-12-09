---
unique-page-id: 2953471
description: Sincronização SFDC - Sincronização de objetos personalizados - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Sincronização de Objeto Personalizado
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# Sincronização SFDC: Sincronização de objetos personalizados {#sfdc-sync-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketing.  Veja como configurar.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Para usar um objeto personalizado, ele deve estar associado a um objeto [de cliente potencial](sfdc-sync-lead-sync.md), [](sfdc-sync-contact-sync.md)contador [](sfdc-sync-account-sync.md)contador no Salesforce.

## Ativar objeto personalizado  {#enable-custom-object}

1. Clique em **Admin** e no **link** de sincronização de objetos do Salesforce.**

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se este for seu primeiro Objeto personalizado, clique em **Sincronizar Schema.**

   ![](assets/rtaimage-2.png)

1. Clique em **Desativar sincronização global.**

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Uma sincronização inicial do schema de objeto personalizado do Salesforce pode levar alguns minutos.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Arraste o objeto personalizado que deseja sincronizar na tela.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Objetos personalizados devem ter nomes exclusivos. O Marketo não suporta dois objetos personalizados diferentes com o mesmo nome.

1. Clique em **Ativar sincronização.**

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Clique em **Ativar sincronização** novamente.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Não se esqueça de reativar sua sincronização global!

1. Volte para a guia **Salesforce **1.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Clique em **Ativar sincronização.**

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Para visualização de todos os objetos personalizados do Salesforce, clique em **Admin** e no link *** Salesforce Objects Sync **(o mesmo que na etapa 1 acima).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >O Marketo oferece suporte apenas a entidades personalizadas que estão vinculadas a entidades padrão de um ou dois níveis de profundidade.

### O que vem a seguir: {#whats-next}

[Adicionar/remover campo de objeto personalizado como restrições de Lista inteligente/acionador](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Excelente! Agora você pode usar dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.

