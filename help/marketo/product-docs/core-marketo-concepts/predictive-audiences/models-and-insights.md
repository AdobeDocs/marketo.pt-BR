---
description: Modelos e insights - Documentação do Marketo - Documentação do produto
title: Modelos e insights
exl-id: 7a01d6f0-000a-4b9a-8abb-9e7f9c4b1679
source-git-commit: e6b6fc5e3414936390a15dfb2034cfa4980169fb
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Modelos e insights {#models-and-insights}

O desempenho de seus modelos depende da qualidade e da integridade dos dados de entrada. Veja o principal fator de influência para cada um de seus modelos de IA de probabilidade. Veja também os principais fatores que resultam em registro de eventos mais alto/menor, participação em eventos ou cancelamento de assinaturas.

>[!NOTE]
>
>Os comportamentos marcados com (+) influenciam as previsões positivamente (e vice-versa).

Aqui está como avaliar sua integridade do modelo.

Navegue até o **[!UICONTROL Modelos e integridade de dados]** seção sob **[!UICONTROL Públicos-alvo preditivos]** no **[!UICONTROL Administrador]** área de Marketo Engage. Aqui você verá todos os seus modelos e seus status.

![Imagem Um](assets/models-and-insights-1.png)

* **Status de treinamento**: Indica se o modelo está treinando ativamente (melhorando as previsões). O treinamento ocorre automaticamente a cada 2 semanas. Qualquer modelo que _Processamento_ pode levar até 24 horas para terminar. Para qualquer _Falha_ modelos, entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target=&quot;_blank&quot;}.
* **Status da pontuação**: Indica se o modelo está calculando previsões ativamente (porcentagens de probabilidade) para os membros do programa.
* **Desempenho**: Categorização do funcionamento do modelo com base na Integridade dos dados e na Qualidade dos dados (veja abaixo).
* **Integridade dos dados**: Porcentagem de atributos de dados presentes/concluídos.
* **Qualidade dos dados**: Porcentagem de atributos que contêm dados bons e utilizáveis.
