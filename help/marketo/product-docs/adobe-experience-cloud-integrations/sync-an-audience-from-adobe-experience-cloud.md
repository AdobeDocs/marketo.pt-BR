---
description: Sincronizar um público-alvo do Adobe Experience Cloud - Documentação do Marketo - Documentação do produto
title: Sincronizar um público-alvo do Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: dd4fb7dfc92580c58da70d603b6d92bd8f64493c
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Sincronizar um público-alvo do Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.

>[!PREREQUISITES]
>
>[Configurar Mapeamento da Organização Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Como sincronizar um público-alvo {#how-to-sync-an-audience}

1. Em Meu Marketo, clique no link **[!UICONTROL Banco de dados]** bloco.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Sincronizar do público-alvo do Experience Cloud]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Clique em **[!UICONTROL Pasta da biblioteca de público-alvo]** e selecione a pasta de origem desejada.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Selecione um **[!UICONTROL Nome do público]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Para o destino, você pode selecionar uma lista existente ou digitar o nome de uma nova. Neste exemplo, estamos criando um novo. Clique em **[!UICONTROL Sincronizar]** quando terminar.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Clique em **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Perguntas frequentes {#faq}

**Como funciona a sincronização de cookies?**

Quando a sincronização de cookies estiver ativada para sua assinatura do Marketo, o munchkin.js da Marketo tentará capturar e armazenar ECIDs de Adobe para a Organização IMS da Adobe especificada durante a configuração de integração e corresponderá essas ECIDs ao identificador de cookie do Marketo correspondente. Isso permite que perfis de usuários anônimos da Marketo sejam enriquecidos com Adobe ECIDs.

Uma outra etapa é necessária para associar o perfil de usuário anônimo a um Perfil principal, que é identificado usando um email de texto sem formatação. Exatamente como isso funciona [está descrito aqui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Por que o tamanho da lista no Marketo é diferente do tamanho na Adobe?**

Uma pessoa também não será sincronizada se não for possível vincular uma ID de cookie da ECID a uma pessoa conhecida no Marketo.

**Esta é uma sincronização única?**

Você só precisa iniciar a sincronização uma vez. Depois disso, os registros serão sincronizados automaticamente. A sincronização inicial pode levar até 24 horas; a partir de agora, novos registros serão sincronizados em 2 a 3 horas.
