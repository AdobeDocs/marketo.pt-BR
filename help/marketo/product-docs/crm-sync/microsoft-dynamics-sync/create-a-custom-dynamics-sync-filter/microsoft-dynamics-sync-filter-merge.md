---
unique-page-id: 10092969
description: Entenda como o filtro de sincronização do Dynamics funciona ao mesclar leads. Saiba como o valor do filtro de sincronização de registro vencedor determina se o registro é sincronizado com o Marketo.
title: Filtro de sincronização Microsoft Dynamics - Mesclar
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Filtro de Sincronização do Dynamics [!DNL Microsoft]: Mesclar {#microsoft-dynamics-sync-filter-merge}

A mesclagem de clientes potenciais em [!DNL Microsoft Dynamics] usa o tipo de Duas Opções - Filtro de sincronização = Sim (TRUE) e Filtro de sincronização = Não (FALSE). Quando você mescla dois registros, o resultado varia, dependendo de qual registro é True e qual é False.

Os registros de lead tornam-se verdadeiros ou falsos com base nas regras de fluxo de trabalho definidas pelo administrador para determinar o vencedor. O filtro de sincronização do registro vencedor é o que determina se o registro [!DNL MS Dynamics] é sincronizado com o Marketo.

É quando um registro é verdadeiro e outro é falso que ele fica complicado.

| Se o filtro de sincronização do registro perdido for: | e o filtro de sincronização do registro vencedor é: | Este é o resultado no Marketo |
|---|---|---|
| [!UICONTROL Verdadeiro] | [!UICONTROL Verdadeiro] | O registro vencedor continua a sincronização com o Marketo |
| [!UICONTROL Falso] | [!UICONTROL Falso] | O registro vencedor continua a **não** sincronizar com o Marketo |
| [!UICONTROL Falso] | [!UICONTROL Verdadeiro] | O registro vencedor será sincronizado com o Marketo |
| [!UICONTROL Verdadeiro] | [!UICONTROL Falso] | O registro vencedor não será sincronizado com o Marketo |
