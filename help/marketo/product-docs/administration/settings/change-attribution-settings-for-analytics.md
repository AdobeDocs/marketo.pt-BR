---
unique-page-id: 2360217
description: Alterar configurações de atribuição para o Analytics - Documentação do Marketo - Documentação do produto
title: Alterar configurações de atribuição do Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 5%

---

# Alterar configurações de atribuição do Analytics {#change-attribution-settings-for-analytics}

Você pode alterar a maneira como a Marketo vincula contatos a oportunidades para atribuição de primeiro e de vários contatos, métricas de conversão de clientes potenciais e o sinalizador de oportunidade influenciada por marketing.

Essas configurações afetarão os relatórios do [!UICONTROL Explorador de Receita] nas áreas [Análise de Oportunidade do Programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análise de Oportunidade](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) e Análise de Cliente Potencial. Isso também afetará o relatório do [!UICONTROL Program Analyzer].

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Clique em **[!UICONTROL Análise do ciclo de receita]**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Clique no link **[!UICONTROL Editar]** em **[!UICONTROL Atribuição]**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >A alteração dessa configuração não modifica nenhum dado do Marketo; ela simplesmente altera a forma como seus relatórios são executados. Isso pode ser revertido a qualquer momento.

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
