---
unique-page-id: 2360217
description: Como definir as opções de atribuição de primeiro e de multitoque, conversão de leads e oportunidades influenciadas pelo marketing no Revenue Cycle Analytics.
title: Alterar configurações de atribuição do Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 5%

---

# Alterar configurações de atribuição do Analytics {#change-attribution-settings-for-analytics}

Você pode alterar a maneira como a Marketo vincula contatos a oportunidades para atribuição de primeiro e de vários contatos, métricas de conversão de clientes potenciais e o sinalizador de oportunidade influenciada por marketing.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Clique em **[!UICONTROL Análise do ciclo de receita]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Clique no link **[!UICONTROL Editar]** em **[!UICONTROL Atribuição]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >A alteração dessa configuração não modifica nenhum dado do Marketo; ela altera a forma como seus relatórios são executados. Isso pode ser revertido a qualquer momento.

1. Selecione uma opção e clique em **[!UICONTROL Salvar]**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >**[!UICONTROL Explícito]**: somente contatos com funções (padrão).
   >
   >**[!UICONTROL Híbrido]**: contatos com funções, se disponíveis. Se nenhum estiver disponível, ele usará todos os contatos nas contas.
   >
   >**[!UICONTROL Implícito]**: todos os contatos, independentemente da função.

>[!CAUTION]
>
>Ao usar **[!UICONTROL Implícito]**, o Marketo sempre examinará todos os contatos associados à conta, independentemente da função. A **Marketo recomenda usar o modo [!UICONTROL Explicit]**. Usar [!UICONTROL Implícito] pode criar falsos positivos, ou seja, pessoas com crédito por uma oportunidade, apesar de não terem influência real na oportunidade. Use [!UICONTROL Implícito] com cuidado.
