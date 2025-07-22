---
unique-page-id: 10092977
description: Filtro de sincronização Microsoft Dynamics - Qualificar - Documentação do Marketo - Documentação do produto
title: Filtro de sincronização Microsoft Dynamics - Qualificar
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 0%

---

# Filtro de Sincronização [!DNL Microsoft Dynamics]: Qualificar {#microsoft-dynamics-sync-filter-qualify}

Quando quiser converter um cliente potencial em um contato em [!DNL Microsoft Dynamics], certifique-se de usar esse processo de Qualificação padrão. Em seguida, sincronize-o com o Marketo.

## O processo de conversão {#the-conversion-process}

Veja como os filtros funcionam durante o processo de conversão.

| Se o filtro de sincronização de leads for: | e o filtro de sincronização de contatos é: | Este é o resultado no Marketo |
|---|---|---|
| [!UICONTROL Falso] | [!UICONTROL Falso] | Nada é sincronizado no Marketo |
| [!UICONTROL Verdadeiro] | [!UICONTROL Verdadeiro] | O contato é sincronizado no Marketo |
| [!UICONTROL Falso] | [!UICONTROL Verdadeiro] | O novo registro de contato é criado no Marketo |
| [!UICONTROL Verdadeiro] | [!UICONTROL Falso] | [!DNL MS Dynamics] atualiza as informações do cliente potencial no Marketo, mas o registro do contato não está sincronizado |

>[!CAUTION]
>
>Oferecemos suporte apenas ao processo de conversão Qualify pronto para uso.
