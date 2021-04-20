---
title: campanha define-a-smart-list-for-a-batch
description: Definir uma lista inteligente para uma campanha em lote
exl-id: 35130f40-cce5-4677-8eaf-f9d73c995ba3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Definir uma lista inteligente para uma campanha em lote

<br> 

As listas inteligentes são o mecanismo em todo o Marketo para definir &quot;quem&quot; (quais pessoas) a serem incluídas, seja um relatório, uma lista ou uma campanha inteligente. Veja como definir uma lista inteligente para uma campanha em lote.

1. Escolha uma campanha inteligente e clique em **[!UICONTROL Smart List]**.

   ![Imagem Um](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. Digite para procurar um filtro e, em seguida, arraste e solte na tela. Repita o procedimento para vários filtros.

   ![Imagem dois](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >Uma campanha inteligente com apenas filtros é executada no modo Lote. Ele encontra pessoas no banco de dados que se qualificam com base nos filtros e executa todas elas pelo fluxo ao mesmo tempo.

   >[!IMPORTANT]
   >
   >Você pode fazer uma campanha inteligente ser executada em uma pessoa de cada vez com base em eventos ao vivo, adicionando acionadores, o que coloca a campanha inteligente no modo Acionador.

1. Clique na lista suspensa e escolha um operador de filtro (por exemplo, **[!UICONTROL is]**, **[!UICONTROL não é]**, etc.) para o filtro que você escolheu.

   ![Imagem Três](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >As linhas vermelhas indicam erros ou informações ausentes. Se não for corrigida, a campanha será inválida e não será executada.

1. Insira o valor do filtro.

   ![Imagem quatro](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>Por padrão, as pessoas que atendem TODAS as regras da lista inteligente são
>qualificado. Isso pode ser modificado para atender às suas necessidades de campanha. Confira [Regras de Lista Inteligente para Lógica Complexa](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic) para saber mais.
>
>Para acionar eventos ao vivo uma pessoa de cada vez, saiba como [Definir lista inteligente para o Smart Campaign | Acionador](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger).
