---
unique-page-id: 2360370
description: Como fazer a correspondência entre os status dos Programas e os status das Campanhas do Salesforce antes da sincronização - Documentos do Marketing - Documentação do produto
title: Como corresponder aos status dos Programas e aos status das Campanhas do Salesforce antes da sincronização
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# Como corresponder aos status dos Programas e aos status das Campanhas do Salesforce antes da sincronização {#how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync}

Este artigo descreve como corrigir um erro de status incompatível e mapear status antes da sincronização de Campanhas do Programa Marketo e Salesforce.

## O que você faz se receber uma mensagem de erro {#what-do-you-do-if-you-received-an-error-message}

Se você tentar sincronizar com uma Campanha Salesforce existente que contenha leads e a campanha contiver um ou mais status incompatíveis, uma mensagem de erro será exibida. Um Programa de marketing e uma Campanha do Salesforce não ** serão sincronizados se os status não forem uma correspondência exata.

![](assets/image2015-7-22-9-3a23-3a29.png)

Nessa mensagem de erro, é possível optar por:

1. Selecione uma campanha diferente para sincronizar no menu suspenso OU
1. Você pode cancelar, corrigir os erros de status e tentar sincronizar assim que os erros forem reparados. Para corrigir os erros de status, execute um dos procedimentos a seguir:

   * Faça logon no Salesforce e remova ou renomeie os Estados-Membros da Campanha incompatíveis para mapear para os Status do Programa de marketing usados para o tipo de canal associado ao Programa de marketing.
   * Modifique os Status do Programa no Marketo para mapear para os Estados-Membros da Campanha do Salesforce que você tem em vigor. Esta é uma função de Administrador de marketing. Para obter detalhes, consulte [Criar um Canal](../../../../../product-docs/administration/tags/create-a-program-channel.md)de Programa.

