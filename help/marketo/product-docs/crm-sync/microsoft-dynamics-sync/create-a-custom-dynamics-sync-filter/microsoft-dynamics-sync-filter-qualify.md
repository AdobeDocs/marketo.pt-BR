---
unique-page-id: 10092977
description: Saiba mais sobre o processo de qualificação de filtro de sincronização do Dynamics ao converter um lead em um contato. Entenda como os valores de filtro de sincronização de lead e contato afetam a sincronização do Marketo.
title: Filtro de sincronização Microsoft Dynamics - Qualificar
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/3jC9Y9fpBNjUzjE1Dy7JBuhNlYQpnc7kjF2LxV-hrp4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 124
ht-degree: 0%

---

# Filtro de Sincronização [!DNL Microsoft Dynamics]: Qualificar {#microsoft-dynamics-sync-filter-qualify}

Quando quiser converter um cliente potencial em um contato em [!DNL Microsoft Dynamics], use este processo de Qualificação padrão. Em seguida, sincronize-o com o Marketo.

## O processo de conversão {#the-conversion-process}

| Se o filtro de sincronização de leads for: | e o filtro de sincronização de contatos é: | Este é o resultado no Marketo |
|---|---|---|
| [!UICONTROL Falso] | [!UICONTROL Falso] | Nada é sincronizado no Marketo |
| [!UICONTROL Verdadeiro] | [!UICONTROL Verdadeiro] | O contato é sincronizado no Marketo |
| [!UICONTROL Falso] | [!UICONTROL Verdadeiro] | O novo registro de contato é criado no Marketo |
| [!UICONTROL Verdadeiro] | [!UICONTROL Falso] | [!DNL MS Dynamics] atualiza as informações do cliente potencial no Marketo, mas o registro do contato não está sincronizado |

>[!CAUTION]
>
>Oferecemos suporte apenas ao processo de conversão Qualify pronto para uso.
