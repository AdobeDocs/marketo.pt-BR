---
title: noções básicas sobre campanhas em lote e acionador inteligente
description: Como entender campanhas inteligentes em lote e acionar
exl-id: 54f38ecc-1b4c-4944-9f42-d8c1190c99d0
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Como entender campanhas inteligentes em lote e acionar

<br> 

Há dois tipos de campanhas inteligentes: Lote e Acionador.

## Campanha inteligente em lote

Uma campanha em lote é iniciada em um horário específico e afeta um conjunto específico de pessoas ao mesmo tempo. Um exemplo seria enviar um email para todos no banco de dados que moram na Califórnia.

As campanhas inteligentes em lote terão apenas filtros na seção da lista inteligente (ou seja, sem acionadores).

![Imagem Um](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Clicar na guia **[!UICONTROL Schedule]** confirmará que a campanha inteligente está definida como &quot;Lote&quot;.

![Imagem dois](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campanhas inteligentes em lote**

* Pode ser programado para recorrências, como diário, semanal e mensal. Você também pode executá-los apenas uma vez.
* São visíveis no [modo de exibição do agendamento do programa](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View).
* Qualquer coisa depois de uma etapa &quot;Aguardar&quot; na campanha inteligente não será incluída na visualização.

## Acionar campanha inteligente

Uma campanha inteligente de acionador afeta uma pessoa de cada vez, com base em um evento acionado. Um exemplo de acionador seria clicar em um link em um email.

Se uma campanha inteligente usar pelo menos um acionador na seção da lista inteligente, o modo será automaticamente definido como acionado.

![Imagem Três](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Clicar na guia **[!UICONTROL Schedule]** confirmará que a campanha inteligente está definida como &quot;Acionador&quot;.

![Imagem quatro](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Acionar campanhas inteligentes**

* Não pode ser agendado para recorrências. Eles só podem ser definidos como ativos ou inativos.
* É possível definir mais de um acionador. No entanto, se _any_ for acionado, as ações da campanha serão executadas.

>[!TIP]
>
>Use o [log de atividades](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) para ver o que aconteceu passo a passo em suas campanhas inteligentes. Você pode encontrar o log de atividades na última guia da página de detalhes de uma pessoa.
