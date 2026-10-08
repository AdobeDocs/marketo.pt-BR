---
unique-page-id: 2360370
description: Saiba como corresponder os status do programa Marketo com os status dos membros do Salesforce Campaign antes da sincronização. Corrija erros e mapeie status para que os programas sincronizem com as campanhas.
title: Como fazer a correspondência entre os status do programa e os status de campanha do Salesforce antes da sincronização
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/54XVLabyXlccM45i9yxPRoMqyrCtoDsATu1o1bEy-50'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 5%
---
# Como fazer a correspondência entre os status do programa e [!DNL Salesforce] status da campanha antes da sincronização {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Este artigo descreve como corrigir um erro de status incompatível e mapear status antes da sincronização do Programa Marketo e do [!DNL Salesforce] Campaign.

## O que você faz se receber uma mensagem de erro {#what-do-you-do-if-you-received-an-error-message}

Se você tentar sincronizar com uma Campanha [!DNL Salesforce] existente que contém clientes potenciais e a campanha contém um ou mais status incompatíveis, será exibida uma mensagem de erro. Um Programa Marketo e uma [!DNL Salesforce] Campanha *não* serão sincronizados se os status não forem uma correspondência exata.

![](assets/image2015-7-22-9-3a23-3a29.png)

Nessa mensagem de erro, você pode optar por:

1. Selecione uma campanha diferente para sincronização no menu suspenso OU
1. Você pode cancelar, corrigir os erros de status e tentar sincronizar depois que os erros forem reparados. Para corrigir os erros de status, siga um destes procedimentos:

   * Faça logon no Salesforce e remova ou renomeie os Status de membros incompatíveis do Campaign para mapear para os Status de programa do Marketo usados para o tipo de canal associado ao seu programa do Marketo.
   * Modifique os Status do programa no Marketo para mapear para os Estados membros do Salesforce Campaign que você tem em vigor. Esta é uma função de administrador do Marketo. Para obter detalhes, consulte [Criar um canal de programa](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}.
