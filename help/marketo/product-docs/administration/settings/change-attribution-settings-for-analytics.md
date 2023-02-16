---
unique-page-id: 2360217
description: Alterar configurações de atribuição para o Analytics - Documentos do Marketo - Documentação do produto
title: Alterar configurações de atribuição do Analytics
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Alterar configurações de atribuição do Analytics {#change-attribution-settings-for-analytics}

Você pode alterar a maneira como o Marketo vincula contatos a oportunidades para atribuição de primeiro e multitoque, métricas de conversão de leads e o sinalizador de oportunidade influenciado pelo marketing.

Essas configurações afetarão os relatórios do Explorador de receita na seção [Análise de oportunidades do programa](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [Análise de oportunidades](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)e áreas de Análise de lead. Isso também afetará o relatório do Analisador de programa.

1. Vá para o **Administrador** área.

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. Clique em **Análise do ciclo de receita**.

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. Clique no botão **Editar** link em **Atribuição**.

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >Alterar essa configuração não modifica dados do Marketo; isso simplesmente altera a forma como seus relatórios são executados. Isso pode ser revertido a qualquer momento.

1. Selecione uma opção e clique em **Salvar**.

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**Definição**
   >
   >**Explícito**: Somente contatos com funções (padrão).
   >
   >**Híbrido**: Contatos com funções, se disponíveis. Se nenhum estiver disponível, ele usará todos os contatos nas contas.
   >
   >**Implicado**: Todos os contatos independentemente da função.

>[!CAUTION]
>
>Ao usar **Implicado**, o Marketo sempre examinará todos os contatos associados à conta, independentemente da função. **A Marketo recomenda utilizar o modo Explícito**. O uso de Implicit pode criar falsos positivos; ou seja, pessoas com crédito por uma oportunidade apesar de não terem influência real na oportunidade. Use Implicit com cuidado.
