---
description: Integridade do modelo e validade de dados - Documentos do Marketo - Documentação do produto
title: Integridade do modelo e validade de dados
hide: true
hidefromtoc: true
exl-id: fdb4ae1c-a638-4aa3-aa09-1993760b8be5
source-git-commit: d229d152cbdae4f6b2e35700b85052d9c0b748d6
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Integridade do modelo e validade de dados {#model-health-and-data-validity}

O desempenho de seus modelos depende da qualidade e da integridade dos dados de entrada. Veja o principal fator de influência para cada um de seus modelos de IA de probabilidade. Veja também os principais fatores que resultam em registro de eventos mais alto/menor, participação em eventos ou cancelamento de assinaturas.

>[!NOTE]
>
>Os comportamentos marcados com (+) influenciam as previsões positivamente (e vice-versa).

Aqui está como avaliar sua integridade do modelo.

Navegue até o **[!UICONTROL Modelos e integridade de dados]** seção sob **[!UICONTROL Públicos-alvo preditivos]** no **[!UICONTROL Administrador]** área do Marketo Classic. Aqui você verá todos os seus modelos e seus status.

![Imagem Um](assets/model-health-and-data-validity-1.png)

* **Status de treinamento**: Indica se o modelo está treinando ativamente (melhorando as previsões). O treinamento ocorre automaticamente a cada 2 semanas. Qualquer modelo que _Processamento_ pode levar até 24 horas para terminar. Para qualquer _Falha_ modelos, entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Status da pontuação**: Indica se o modelo está calculando previsões ativamente (porcentagens de probabilidade) para os membros do programa.
* **Desempenho**: Categorização do funcionamento do modelo com base na Integridade dos dados e na Qualidade dos dados (veja abaixo).
* **Integridade dos dados**: Porcentagem de atributos de dados presentes/concluídos.
* **Qualidade dos dados**: Porcentagem de atributos que contêm dados bons e utilizáveis.
