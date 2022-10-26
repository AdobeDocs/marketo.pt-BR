---
description: Sincronizar um público-alvo do Adobe Experience Cloud - Marketo Docs - Documentação do produto
title: Sincronizar um público-alvo do Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 492f21f090dc2478271172cf7db470e16f202366
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Sincronizar um público-alvo do Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.

>[!PREREQUISITES]
>
>[Configurar Mapeamento de Organização do Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target=&quot;_blank&quot;}

## Como sincronizar um público-alvo {#how-to-sync-an-audience}

1. Em Minha Marketo, clique no botão **Banco de dados** mosaico.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Clique no botão **Novo** e selecione **Sincronizar do público-alvo do Experience Cloud**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Clique no botão **Pasta da biblioteca de público-alvo** e selecione a pasta de origem desejada.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Selecione um **Nome do público-alvo**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Para o destino, você pode selecionar uma lista existente ou digitar o nome de uma nova. Neste exemplo, estamos criando um novo. Clique em **Sincronizar** quando concluído.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Clique em **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Perguntas frequentes {#faq}

**Como a sincronização de cookies funciona?**

Quando a sincronização de cookies estiver ativada para sua assinatura do Marketo, o Marketo munchkin.js tentará capturar e armazenar Adobe ECIDs para a organização do Adobe IMS especificada durante a configuração da integração e corresponder essas ECIDs ao identificador de cookie do Marketo correspondente. Isso permite que perfis de usuário anônimos do Marketo sejam enriquecidos com Adobe ECIDs.

É necessária uma nova etapa para associar o perfil de usuário anônimo a um Perfil de cliente potencial, que é identificado usando um email de texto simples. Exatamente como isso funciona [é descrito aqui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target=&quot;_blank&quot;}.

**Por que o tamanho da lista no Marketo é diferente do do Adobe?**

Uma pessoa também não será sincronizada se não formos capazes de vincular uma ID de cookie ECID a uma pessoa conhecida no Marketo.

**Isso é uma sincronização única?**

Você só precisa iniciar a sincronização uma vez. Depois disso, os registros serão sincronizados automaticamente. A sincronização inicial pode demorar até 24 horas; a partir de agora, novos registros serão sincronizados em 2 a 3 horas.
