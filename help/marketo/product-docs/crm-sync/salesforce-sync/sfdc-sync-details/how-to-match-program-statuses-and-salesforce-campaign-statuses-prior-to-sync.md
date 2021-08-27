---
unique-page-id: 2360370
description: Como fazer a correspondência dos status do programa e dos status da campanha do Salesforce antes de sincronizar - Documentos do Marketo - Documentação do produto
title: Como corresponder aos status do programa e status da campanha do Salesforce antes da sincronização
exl-id: 623676ff-ce63-484f-8467-71127fa40fe0
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Como corresponder aos status do programa e status da campanha do Salesforce antes da sincronização {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Este artigo descreve como corrigir um erro de status incompatível e mapear status antes da sincronização entre o Programa Marketo e o Salesforce Campaign.

## O que fazer se receber uma mensagem de erro {#what-do-you-do-if-you-received-an-error-message}

Se você tentar sincronizar com uma campanha Salesforce existente que contenha leads e a campanha contenha um ou mais status incompatíveis, uma mensagem de erro será exibida. Um Programa Marketo e uma Campanha Salesforce *não sincronizarão* se os status não forem uma correspondência exata.

![](assets/image2015-7-22-9-3a23-3a29.png)

Nessa mensagem de erro, é possível optar por:

1. Selecione uma campanha diferente para sincronizar no menu suspenso OU
1. Você pode cancelar, corrigir os erros de status e tentar sincronizar assim que os erros forem reparados. Para corrigir os erros de status, execute um dos seguintes procedimentos:

   * Faça logon no Salesforce e remova ou renomeie os Estados membros da campanha incompatíveis para mapear para os Status do Programa Marketo usados para o tipo de canal associado ao seu Programa Marketo.
   * Modifique os Status do Programa no Marketo para mapear para os Estados Membros da Campanha do Salesforce que você tem em vigor. Esta é uma função de administrador do Marketo. Para obter detalhes, consulte [Criar um canal de programa](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).
