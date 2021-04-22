---
unique-page-id: 2953132
description: Noções básicas sobre campanhas inteligentes em lote e acionadoras - Documentos do Marketo - Documentação do produto
title: Como entender campanhas inteligentes em lote e acionar
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Como entender as campanhas inteligentes em lote e acionar {#understanding-batch-and-trigger-smart-campaigns}

Há dois tipos de campanhas inteligentes: Lote e Acionador.

## Campanha inteligente em lote {#batch-smart-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma campanha em lote é iniciada em um horário específico e afeta um conjunto específico de pessoas ao mesmo tempo. Um exemplo seria enviar um email para todas as pessoas na Califórnia.

As campanhas inteligentes em lote terão apenas filtros na seção da lista inteligente (ou seja, sem acionadores).

![](assets/batch-filter.png)

Clicar na guia **Schedule** confirmará que a campanha inteligente está definida como &quot;Lote&quot;.

![](assets/batch-c4.png)

**Campanhas inteligentes em lote**

* Pode ser programado para recorrências, como diário, semanal e mensal. Você também pode executá-los apenas uma vez.
* São visíveis no [modo de exibição do agendamento do programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md). Qualquer coisa depois de uma etapa &quot;Aguardar&quot; na campanha inteligente não será incluída na visualização.

<br> 

## Acionar Campanha Inteligente {#trigger-smart-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma campanha inteligente de acionador afeta uma pessoa de cada vez, com base em um evento acionado. Um exemplo de acionador seria clicar em um link em um email.

Se uma campanha inteligente usar pelo menos um acionador na seção da lista inteligente, o modo será automaticamente definido como acionado.

![](assets/trigger.png)

Clicar na guia **Schedule** confirmará que a campanha inteligente está definida como &quot;Acionada&quot;.

![](assets/trigger2.png)

**Acionar campanhas inteligentes**

* Não pode ser agendado para recorrências. Eles só podem ser definidos como ativos ou inativos.
* É possível definir mais de um acionador. No entanto, se qualquer acionador for acionado, as ações da campanha serão executadas.

>[!TIP]
>
>Use o [log de atividades](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) para ver o que aconteceu passo a passo em suas campanhas inteligentes. Você pode encontrar o log de atividades na última guia da página de detalhes de uma pessoa.
