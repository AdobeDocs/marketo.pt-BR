---
unique-page-id: 2360217
description: Alterar configurações de atribuição do Analytics - Documentos de marketing - Documentação do produto
title: Alterar configurações de atribuição do Analytics
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Alterar configurações de atribuição do Analytics {#change-attribution-settings-for-analytics}

Você pode alterar a forma como o Marketo vincula os contatos a oportunidades para atribuição de primeiro e multitoque, métricas de conversão de lead e o sinalizador de oportunidade influenciado pelo marketing.

Essas configurações afetarão os relatórios do Revenue Explorer nas áreas [Análise de oportunidade de Programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análise de oportunidade](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md) e Análise de cliente potencial. Isso também afetará o relatório do Analisador de Programas.

1. Na seção **Admin**, clique em **Análises do ciclo de receita**.

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. Clique no link **Editar** em **Atribuição**.

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >Alterar essa configuração não modifica nenhum dado de marketing; isso simplesmente muda a forma como seus relatórios são executados. Isso pode ser revertido a qualquer momento.

1. Selecione uma opção e clique em **Salvar**.

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >**Explícita**: Somente contatos com funções (padrão).
   >
   >**Híbrido**: Contatos com funções, se disponíveis. Se nenhum estiver disponível, ele usará todos os contatos nas contas.
   >
   >**Implícita**: Todos os contatos, independentemente da função.

>[!CAUTION]
>
>Ao usar **Implicit**, o Marketo sempre examinará todos os contatos associados à conta, independentemente da função. **O Marketo recomenda o uso do modo** Explícito. A utilização de Implicit pode criar falsos positivos; Ou seja, pessoas com crédito por uma oportunidade, apesar de não terem influência real na oportunidade. Use Implicit com cautela.
