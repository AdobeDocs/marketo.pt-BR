---
unique-page-id: 2953132
description: Saiba mais sobre Campanhas inteligentes em lote e acionadas. Entenda quando usar cada tipo e como eles são executados.
title: Noções básicas sobre campanhas inteligentes em lote e acionáveis
exl-id: 84a7b38c-b79c-4360-bd0b-3beb8ca35ac7
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/48wdmRPcrjaIavo4EQG3nkQNcUMH33tuISSqU2VouTM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 5%

---

# Noções básicas sobre campanhas inteligentes em lote e acionáveis {#understanding-batch-and-trigger-smart-campaigns}

Há dois tipos de campanhas inteligentes: Em lote e Acionador.

## Campanha em lote {#batch-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma Campanha em lote é iniciada em um horário específico e afeta um conjunto específico de pessoas, todas de uma só vez. Um exemplo seria o envio de um email para todas as pessoas na Califórnia.

As campanhas em lote só terão filtros na seção de lista inteligente (ou seja, nenhum acionador).

![](assets/understanding-batch-and-trigger-smart-campaigns-1.png)

Clicar na guia **[!UICONTROL Agendamento]** confirmará que a Campanha inteligente está definida como &quot;Em lote&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campanhas inteligentes em lote**

* Pode ser programado para recorrências, como diariamente, semanalmente e mensalmente. Você também pode executá-las apenas uma vez.
* Estão visíveis na [exibição de agendamento de programa](/help/marketo/product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md){target="_blank"}. Qualquer item depois de uma etapa &quot;Aguardar&quot; na Campanha inteligente não será incluído na visualização.

<br> 

## Campanha com acionador {#trigger-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma Campanha de acionador afeta uma pessoa de cada vez com base em um evento acionado. Um exemplo de um acionador seria clicar em um link em um email.

Se uma Campanha inteligente usar pelo menos um acionador na seção Smart List, o modo será automaticamente definido como acionado.

![](assets/understanding-batch-and-trigger-smart-campaigns-3.png)

Clicar na guia **[!UICONTROL Agendamento]** confirmará que a Campanha inteligente está definida como &quot;Acionado&quot;.

![](assets/understanding-batch-and-trigger-smart-campaigns-4.png)

**Acionar Campanhas**

* Não é possível agendar recorrências. Elas só podem ser definidas como ativas ou inativas.
* É possível definir mais de um acionador. No entanto, se algum acionador for acionado, as ações da campanha serão executadas.

>[!TIP]
>
>Use o [log de atividades](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"} para ver o que ocorreu passo a passo em suas Campanhas Inteligentes. Você pode encontrar o log de atividades na última guia da página de detalhes de uma pessoa.
