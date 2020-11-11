---
title: campanhas inteligentes de compreensão de lote e acionador
description: Noções básicas sobre Campanhas inteligentes em lote e acionador
translation-type: tm+mt
source-git-commit: cd1b7e65c73de0b31f20289402f1c0832c382b33
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Noções básicas sobre Campanhas inteligentes em lote e acionador

<br> 

Há dois tipos de campanhas inteligentes: Lote e Acionador.

## Campanha inteligente em lote

Uma campanha em lote é aberta em um horário específico e afeta um conjunto específico de pessoas de uma só vez. Um exemplo seria enviar um e-mail para todos em seu banco de dados que moram na Califórnia.

Campanhas inteligentes em lote terão apenas filtros na seção lista inteligente (ou seja, sem acionadores).

![Imagem Um](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-1.png)

Clicar na guia [!UICONTROL **Agendamento**] confirmará que a campanha inteligente está definida como &quot;Lote&quot;.

![Imagem dois](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-2.png)

**Campanhas inteligentes em lote**

* Pode ser agendado para recorrências, como diário, semanal e mensal. Você também pode fazê-los funcionar apenas uma vez.
* São visíveis na visualização [do](https://docs.marketo.com/display/DOCS/Navigating+the+Program+Schedule+View)cronograma do programa.
* Qualquer coisa depois de uma etapa de &quot;Espera&quot; dentro da campanha inteligente não será incluída na visualização.

## Acionar Campanha inteligente

Uma campanha inteligente de disparo afeta uma pessoa de cada vez com base em um evento acionado. Um exemplo de acionador seria clicar em um link em um email.

Se uma campanha inteligente usar pelo menos um acionador na seção lista inteligente, o modo será automaticamente definido como acionado.

![Imagem Três](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-3.png)

Clicar na guia [!UICONTROL **Agendamento**] confirmará que a campanha inteligente está definida como &quot;Acionador&quot;.

![Imagem quatro](/help/sky/assets/smart-campaigns/understanding-batch-and-trigger-smart-campaigns/understanding-batch-and-trigger-smart-campaigns-4.png)

**Acionar Campanhas inteligentes**

* Não pode ser agendado para recursões. Eles só podem ser definidos como ativos ou inativos.
* É possível definir mais de um acionador. No entanto, se _algum_ acionador for acionado, as ações de campanha serão executadas.

>[!TIP]
>
>Use o log [de](https://docs.marketo.com/display/DOCS/Locate+the+Activity+Log+for+a+Person) atividades para ver o que ocorreu passo a passo dentro das campanhas inteligentes. Você pode encontrar o log de atividades na última guia da página de detalhes de uma pessoa.
