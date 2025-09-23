---
description: Sincronizar um público-alvo do Adobe Experience Cloud - Documentação do Marketo - Documentação do produto
title: Sincronizar um público-alvo da Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 6%

---

# Sincronizar um público-alvo da Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.

>[!PREREQUISITES]
>
>[Configurar o Adobe Organization Mapping](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Como sincronizar um público-alvo {#how-to-sync-an-audience}

1. Em Meu Marketo, clique no bloco **[!UICONTROL Banco de Dados]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Sincronizar a partir do Público-alvo da Experience Cloud]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Clique no menu suspenso **[!UICONTROL Pasta da biblioteca de público-alvo]** e selecione a pasta de origem desejada.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Selecione um **[!UICONTROL Nome do Público]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Para o destino, você pode selecionar uma lista existente ou digitar o nome de uma nova. Neste exemplo, estamos criando um novo. Clique em **[!UICONTROL Sincronizar]** quando terminar.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Clique em **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Perguntas frequentes {#faq}

**Como funciona a sincronização de cookies?**

Quando a sincronização de cookies está ativada para sua assinatura do Marketo, o munchkin.js da Marketo tenta capturar e armazenar ECIDs do Adobe para a Organização IMS da Adobe especificada durante a configuração de integração e corresponder essas ECIDs ao identificador de cookie do Marketo correspondente. Isso permite que perfis de usuários anônimos da Marketo sejam enriquecidos com ECIDs do Adobe.

Uma outra etapa é necessária para associar o perfil de usuário anônimo a um Perfil principal, que é identificado usando um email de texto sem formatação. [está descrito aqui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"} como funciona exatamente.

**Por que o tamanho da lista no Marketo é diferente do tamanho da lista no Adobe?**

Uma pessoa também não será sincronizada se não for possível vincular uma ID de cookie da ECID a uma pessoa conhecida no Marketo.

**Esta é uma sincronização única?**

Você só precisa iniciar a sincronização uma vez. Depois disso, os registros serão sincronizados automaticamente. A sincronização inicial pode levar até 24 horas; a partir de agora, novos registros serão sincronizados em 2 a 3 horas.
