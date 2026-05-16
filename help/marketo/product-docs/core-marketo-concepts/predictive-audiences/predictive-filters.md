---
description: Saiba mais sobre filtros preditivos para direcionar públicos-alvo com IA. Use filtros em Smart Lists e campanhas para alcançar as pessoas certas.
title: Filtros preditivos
exl-id: 27736b80-cd8b-455d-9d73-c17d492d0906
feature: Predictive Audiences
TQID: https://experienceleague.adobe.com/-P6jjTHT-YDpoEE6yg23rd48s3YYN4kzABbJwZp4rig
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
  - id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 427
ht-degree: 3%

---

# Filtros preditivos {#predictive-filters}

Como parte do Predictive Audiences, o Marketo oferece um grupo de filtros baseados em IA/ML em Smart Lists nas Campanhas inteligentes.

![Imagem 1](assets/predictive-filters-1.png)

>[!NOTE]
>
>Os filtros &quot;Probabilidade de participação&quot; e &quot;Probabilidade de registro&quot; só podem ser usados em Programas de evento. É possível usar as opções &quot;Probabilidade de cancelamento de inscrição&quot;, &quot;Semelhança de membros de programa&quot; e &quot;Semelhança de membros de lista inteligente&quot; em todos os tipos de programas.

## Probabilidade de participar {#likelihood-to-attend}

Esse filtro é usado para restringir efetivamente seu público-alvo. Isso o ajudará a direcionar e convidar clientes potenciais com maior probabilidade de **participar** do seu webinário ou evento. Observe que o &quot;Programa de probabilidade de participação&quot; será seu programa de evento atual.

![Imagem Dois](assets/predictive-filters-2.png)

## Probabilidade de inscrever-se {#likelihood-to-register}

Semelhante ao filtro _Probabilidade de participação_, use esse filtro para restringir seu público-alvo e os clientes potenciais do público-alvo que tenham uma probabilidade maior de **se registrar** no seu webinário ou evento.

![Imagem três](assets/predictive-filters-3.png)

## Probabilidade de cancelar a inscrição {#likelihood-to-unsubscribe}

Isso filtra o público-alvo determinando se ele tem uma alta ou baixa probabilidade de cancelar a assinatura nas próximas duas semanas. Você pode usá-lo para direcionar condutores de alta fadiga de forma diferente e com mais eficiência. O limite de cancelamento de inscrição é dinâmico e orientado por um modelo de IA que considera vários atributos, incluindo o lead time no banco de dados e as atividades de lead.

![Imagem Quatro](assets/predictive-filters-4.png)

>[!NOTE]
>
>Os filtros Probabilidade de participação/registro/cancelamento de inscrição devem ser usados junto com outros filtros padrão.

## Semelhança de Membros do Programa/Semelhança de Membros da Smart List {#lookalike-of-members}

Esses dois filtros ajudam você a expandir seu público-alvo atual direcionando leads adicionais que são semelhantes aos membros de outro programa ou lista inteligente. Os filtros Semelhantes consideram mais de 50 fatores, incluindo atributos de cliente potencial, atividade de email, atividade da Web e envolvimento.

Clique em **[!UICONTROL Adicionar Restrição]** para escolher os critérios de sucesso para os membros do(s) programa(s) selecionado(s).

Clique no ícone **+** para adicionar vários programas/Smart Lists a um filtro.

![Imagem Cinco](assets/predictive-filters-5.png)

## Itens a Observar {#things-to-note}

* Você pode aplicar filtros preditivos a uma Campanha inteligente, mesmo se o programa principal for criado antes da ativação dos filtros preditivos.
* Os filtros preditivos não estão disponíveis para Campanhas de acionador.
* Não há suporte para clonagem ou movimentação de campanhas que contêm filtros preditivos.
* Você pode usar até 5 filtros preditivos em uma Smart List.
* Se o Marketo Engage encontrar um erro na avaliação de filtros preditivos, a execução da campanha será anulada automaticamente e uma notificação será enviada ao centro de notificações da Marketo.
* Atualmente, os filtros preditivos têm um limite de entrada de 1 milhão de pessoas qualificadas.
* Você pode ter até 50 programas ativos com filtros preditivos.
