---
unique-page-id: 1147082
description: Excluir pessoa - Documentação do Marketo - Documentação do produto
title: Excluir pessoa
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 3%

---

# Excluir pessoa {#delete-person}

Pessoas erradas às vezes entram no banco de dados. A etapa de fluxo Excluir pessoa pode se livrar delas.

![](assets/delete-person-1.png)

>[!CAUTION]
>
>Quando você exclui uma pessoa, todos os seus dados históricos de RCE também serão excluídos. Ela não pode ser desfeita.

1. Ao arrastar a etapa de fluxo, ela também será automaticamente definida para excluir do seu CRM.

   ![](assets/delete-person-2.png)

1. Você pode excluir do Marketo Engage e não do seu CRM, da seguinte maneira:

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>Remover a pessoa do seu CRM _só funciona com[!DNL Salesforce]_. Se você excluir uma pessoa do Marketo e optar por mantê-la em [!DNL Salesforce], ela será recriada no Marketo se seu registro [!DNL Salesforce] for atualizado.
