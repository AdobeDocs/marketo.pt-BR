---
title: modelo-integridade-e-validade de dados
description: Integridade do modelo e validade de dados
exl-id: b14ec648-be1c-467b-b41d-2c53d74e25ea
source-git-commit: 41a51afde7942d6973a01636810bc5862d023e99
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Integridade do modelo e validade de dados

O desempenho de seus modelos depende da qualidade e da integridade dos dados de entrada. Veja o principal fator de influência para cada um de seus modelos de IA de probabilidade. Veja também os principais fatores que resultam em registro de eventos mais alto/menor, participação em eventos ou cancelamento de assinaturas.

>[!NOTE]
>
>Os comportamentos marcados com (+) influenciam as previsões positivamente (e vice-versa).

Aqui está como avaliar sua integridade do modelo.

Navegue até o **[!UICONTROL Modelos e integridade de dados]** seção sob **[!UICONTROL Públicos-alvo preditivos]** no **[!UICONTROL Administrador]** área do Marketo Classic. Aqui você verá todos os seus modelos e seus status.

![Imagem Um](/help/sky/assets/predictive-audiences/model-health-and-data-validity/model-health-and-data-validity-1.png)

* **Status de treinamento**: Indica se o modelo está treinando ativamente (melhorando as previsões). O treinamento ocorre automaticamente a cada 2 semanas. Qualquer modelo que _Processamento_ pode levar até 24 horas para terminar. Para qualquer _Falha_ modelos, entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Status da pontuação**: Indica se o modelo está calculando previsões ativamente (porcentagens de probabilidade) para os membros do programa.
* **Desempenho**: Categorização do funcionamento do modelo com base na Integridade dos dados e na Qualidade dos dados (veja abaixo).
* **Integridade dos dados**: Porcentagem de atributos de dados presentes/concluídos.
* **Qualidade dos dados**: Porcentagem de atributos que contêm dados bons e utilizáveis.
