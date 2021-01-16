---
unique-page-id: 2953132
description: Noções básicas sobre Campanhas inteligentes em lote e acionador - Documentos do Marketing - Documentação do produto
title: Noções básicas sobre Campanhas inteligentes em lote e acionador
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---


# Noções básicas sobre Campanhas inteligentes em lote e acionador {#understanding-batch-and-trigger-smart-campaigns}

Há dois tipos de campanhas inteligentes: Lote e Acionador.

## Campanha inteligente em lote {#batch-smart-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma campanha em lote é aberta em um horário específico e afeta um conjunto específico de pessoas de uma só vez. Um exemplo seria enviar um email para todas as pessoas na Califórnia.

Campanhas inteligentes em lote terão apenas filtros na seção lista inteligente (ou seja, sem acionadores).

![](assets/batch-filter.png)

Clicar na guia **Schedule** confirmará que a campanha inteligente está definida como &quot;Batch&quot;.

![](assets/batch-c4.png)

**Campanhas inteligentes em lote**

* Pode ser agendado para recorrências, como diário, semanal e mensal. Você também pode fazê-los funcionar apenas uma vez.
* Estão visíveis na visualização [do cronograma do programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Qualquer coisa depois de uma etapa de &quot;Espera&quot; dentro da campanha inteligente não será incluída na visualização.

<br> 

## Acionar a Campanha inteligente {#trigger-smart-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma campanha inteligente de disparo afeta uma pessoa de cada vez com base em um evento acionado. Um exemplo de acionador seria clicar em um link em um email.

Se uma campanha inteligente usar pelo menos um acionador na seção lista inteligente, o modo será automaticamente definido como acionado.

![](assets/trigger.png)

Clicar na guia **Schedule** confirmará que a campanha inteligente está definida como &quot;Disparado&quot;.

![](assets/trigger2.png)

**Acionar Campanhas inteligentes**

* Não pode ser agendado para recursões. Eles só podem ser definidos como ativos ou inativos.
* É possível definir mais de um acionador. No entanto, se qualquer disparador for acionado, as ações de campanha serão executadas.

>[!TIP]
>
>Use o [registro de atividades](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) para ver o que ocorreu passo a passo nas campanhas inteligentes. Você pode encontrar o log de atividades na última guia da página de detalhes de uma pessoa.
