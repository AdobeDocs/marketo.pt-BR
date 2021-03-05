---
description: Adicionar ou remover pessoas de sua campanha dinâmica - Documentos do Marketo - Documentação do produto
title: Adicionar ou remover pessoas de sua campanha dinâmica
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# Adicionar ou remover pessoas de sua campanha dinâmica {#add-or-remove-people-from-your-dynamics-campaign}

## Adicionar à Campanha Dinâmica {#add-to-dynamics-campaign}

Esta etapa do fluxo pode ser usada em Campanhas inteligentes do Marketo para adicionar pessoas como leads ou contatos em uma campanha da Microsoft. Se o lead ainda não existir no Dynamics, será sincronizado automaticamente e adicionado à campanha.

>[!NOTE]
>
>Essa ação de fluxo está disponível somente para Campanhas de acionador.

Em sua campanha inteligente, encontre e selecione a campanha Dynamics à qual deseja adicionar suas pessoas.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Se você não conseguir ver uma campanha do Dynamics na lista de campanhas:
>
>* Verifique se a Sincronização de campanha está funcional
>* A campanha não está ativa no Microsoft Dynamics


O sistema cria automaticamente uma Lista de marketing estático específica da campanha, cada uma para leads e contatos, para adicioná-la. É uma ação única e, uma vez, para sincronizações subsequentes da campanha, a mesma Lista de marketing é usada. O padrão de nomenclatura adotado para o nome estático da Lista de marketing é `Mkto-leads-<uniqueID>` para leads e `Mkto-contacts-<uniqueID>` para contatos.

A associação dessas Listas de marketing geradas pelo Marketo a outras campanhas pode levar a comportamentos confusos. Por exemplo: adicionar a uma campanha também resultaria na adição à segunda campanha. Da mesma forma, não é recomendado dissociar a Lista de marketing gerada pelo Marketo da Campanha no Dynamics.

## Remover do Dynamics Campaign {#remove-from-dynamics-campaign}

Esta etapa do fluxo pode ser usada em Campanhas inteligentes do Marketo para remover pessoas de uma campanha da Microsoft. Isso remove somente os leads de uma Campanha que foram adicionados anteriormente à Campanha por meio da ação de fluxo &quot;Adicionado ao Microsoft Campaign&quot;.

>[!NOTE]
>
>Essa ação de fluxo está disponível somente para Campanhas de acionador.

Em sua campanha inteligente, encontre e selecione a campanha Dynamics da qual deseja remover suas pessoas.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Se você não vir uma campanha do Dynamics na lista de campanhas:
>
>* Verifique se a Sincronização de campanha está funcional
>* A campanha não está ativa no Microsoft Dynamics

