---
description: Saiba como adicionar ou remover pessoas de uma campanha do Microsoft Dynamics com uma etapa de fluxo. Sincronizar o Marketo com campanhas do Dynamics.
title: Adicionar ou Remover Pessoas da sua  [!DNL Dynamics] Campanha
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/b6tUqixPGr7ZWTUKVg4L6EKryziHA2IwzpuTepWWEwU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 324
ht-degree: 0%

---

# Adicionar ou Remover Pessoas da sua Campanha [!DNL Dynamics] {#add-or-remove-people-from-your-dynamics-campaign}

## Adicionar ao Dynamics Campaign {#add-to-dynamics-campaign}

Essa etapa do fluxo pode ser usada em Campanhas inteligentes do Marketo Engage para adicionar pessoas como leads ou contatos em uma campanha do Microsoft. Se o lead ainda não existir no Dynamics, ele será sincronizado automaticamente e será adicionado à campanha.

>[!NOTE]
>
>Essa ação de fluxo está disponível somente para Campanhas de acionador.

Na Campanha inteligente, localize e selecione a campanha do Dynamics à qual deseja adicionar seus funcionários.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Se não conseguir ver uma campanha do Dynamics na lista de campanhas:
>
>* Verificar se a sincronização do Campaign está funcionando
>* A campanha não está ativa em [!DNL Microsoft Dynamics]

O sistema cria automaticamente uma Lista de marketing estática específica da campanha, cada uma para leads e contatos, à qual a pessoa será adicionada. É uma ação única e, uma vez para sincronizações subsequentes da campanha, a mesma Lista de marketing é usada. O padrão de nomenclatura adotado para o nome estático da Lista de marketing é `Mkto-leads-<uniqueID>` para clientes potenciais e `Mkto-contacts-<uniqueID>` para contatos.

Associar essas Listas de marketing geradas pela Marketo a outras campanhas pode levar a um comportamento confuso. Por exemplo: adicionar a uma campanha também resultaria em adicionar à segunda campanha. Da mesma forma, não é recomendado desassociar a Lista de marketing gerada pela Marketo da Campanha em [!DNL Dynamics].

## Remover do Dynamics Campaign {#remove-from-dynamics-campaign}

Essa etapa do fluxo pode ser usada em Campanhas inteligentes do Marketo para remover pessoas de uma campanha do Microsoft. Isso remove apenas os clientes em potencial de uma Campanha que foram adicionados anteriormente à Campanha por meio da ação de fluxo &quot;Adicionado à Campanha do Microsoft&quot;.

>[!NOTE]
>
>Essa ação de fluxo está disponível somente para Campanhas de acionador.

Na Campanha inteligente, localize e selecione a campanha do Dynamics da qual deseja remover seus funcionários.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Se você não vir uma campanha [!DNL Dynamics] na lista de campanhas:
>
>* Verificar se a sincronização do Campaign está funcionando
>* A campanha não está ativa em [!DNL Microsoft Dynamics]
