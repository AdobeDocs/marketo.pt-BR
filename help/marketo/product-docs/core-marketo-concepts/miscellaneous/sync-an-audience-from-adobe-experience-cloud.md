---
description: Sincronizar um público-alvo da Adobe Experience Cloud - Documentos do Marketo - Documentação do produto
title: Sincronizar um público-alvo da Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: 05c2e89222f9316241a3929642998bddb02ff7a5
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# Sincronizar um público-alvo da Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.

>[!PREREQUISITES]
>
>[Configurar o compartilhamento de público na Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Como sincronizar um público-alvo {#how-to-sync-an-audience}

1. Em Meu Marketo, clique no bloco **Banco de dados**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Clique no menu suspenso **New** e selecione **Sync from Experience Cloud Audience**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Clique no menu suspenso **Audience Library Folder** e selecione a pasta de origem desejada.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Selecione um **Nome de público-alvo**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Para o destino, você pode selecionar uma lista existente ou digitar o nome de uma nova. Neste exemplo, estamos criando um novo. Clique em **Sincronizar** quando terminar.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Clique em **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Perguntas frequentes {#faq}

**Como a sincronização de cookies funciona?**

Quando a sincronização de cookies estiver ativada para sua assinatura do Marketo, o munchkin.js do Marketo tentará capturar e armazenar Adobe ECIDs para a organização Adobe IMS especificada durante a configuração da integração e combinar essas ECIDs com o identificador de cookie do Marketo correspondente. Isso permite que os perfis de usuário anônimos do Marketo sejam enriquecidos com Adobe ECIDs.

É necessária uma nova etapa para associar o perfil de usuário anônimo a um Perfil de cliente potencial, que é identificado usando um email de texto simples. Exatamente como isso funciona [está descrito aqui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Por que o tamanho da lista no Marketo é diferente daquele na Adobe?**

Uma pessoa também não será sincronizada se não formos capazes de vincular uma ID de cookie ECID a uma pessoa conhecida no Marketo.

**Isso é uma sincronização única?**

Você só precisa iniciar a sincronização uma vez. Depois disso, os registros serão sincronizados automaticamente. A sincronização inicial pode demorar até 24 horas; a partir de agora, novos registros serão sincronizados em 2 a 3 horas.
