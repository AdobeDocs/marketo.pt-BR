---
unique-page-id: 2953132
description: Noções básicas sobre Campanhas inteligentes em lote e acionador - Documentos do Marketing - Documentação do produto
title: Noções básicas sobre Campanhas inteligentes em lote e acionador
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---


# Noções básicas sobre Campanhas inteligentes em lote e acionador {#understanding-batch-and-trigger-smart-campaigns}

Há dois tipos de campanhas inteligentes: Lote e Acionador.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Campanha inteligente em lote {#batch-smart-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma campanha em lote é aberta em um horário específico e afeta um conjunto específico de pessoas de uma só vez. Um exemplo seria enviar um email para todas as pessoas na Califórnia.

Campanhas inteligentes em lote terão apenas filtros na seção lista inteligente (ou seja, sem acionadores).

![](assets/batch-filter.png)

Clicar na guia **Agendamento** confirmará que a campanha inteligente está definida como &quot;Lote&quot;.

![](assets/batch-c4.png)

**Campanhas inteligentes em lote**

* Pode ser agendado para recorrências, como diário, semanal e mensal. Você também pode fazê-los funcionar apenas uma vez.
* São visíveis na visualização [do](../../../../product-docs/core-marketo-concepts/programs/program-schedule-view/navigating-the-program-schedule-view.md)cronograma do programa.\
   *Observe que qualquer item depois de uma etapa de &quot;Espera&quot; dentro da campanha inteligente não será incluído na visualização.

<br> 

## Acionar Campanha inteligente {#trigger-smart-campaign}

>[!NOTE]
>
>**Definição**
>
>Uma campanha inteligente de disparo afeta uma pessoa de cada vez com base em um evento acionado. Um exemplo de acionador seria clicar em um link em um email.

Se uma campanha inteligente usar pelo menos um acionador na seção lista inteligente, o modo será automaticamente definido como acionado.

![](assets/trigger.png)

Clicar na guia **Agendamento** confirmará que a campanha inteligente está definida como &quot;Acionada&quot;.

![](assets/trigger2.png)

**Acionar Campanhas inteligentes**

* Não pode ser agendado para recursões. Eles só podem ser definidos como ativos ou inativos.
* É possível definir mais de um acionador. No entanto, se qualquer disparador for acionado, as ações de campanha serão executadas.

## Assista a um vídeo sobre como criar Campanhas de e-mail acionadas {#watch-a-video-on-creating-triggered-email-campaigns}

`<iframe width="630" height="470" src="//play.vidyard.com/6zNazwTgt2LNeCjPAt3W9K.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

>[!TIP]
>
>Use o log [de](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md) atividades para ver o que ocorreu passo a passo dentro das campanhas inteligentes. Você pode encontrar o log de atividades na última guia da página de detalhes de uma pessoa.

