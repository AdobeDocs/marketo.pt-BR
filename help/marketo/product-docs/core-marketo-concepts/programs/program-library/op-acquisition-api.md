---
description: Modelo do programa operacional da API de aquisição. Use-a para capturar leads por meio da API.
title: OP-Aquisição-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
TQID: https://experienceleague.adobe.com/a-4w7mJg44cvotVtX2qwx1e4p8SKIbQU1jPWyQ0BzUA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: df401a2a-327d-468c-a5e4-b7b7ccd071a0
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 21%

---

# OP-Aquisição-API {#op-acquisition-api}

Este programa de exemplo é para processos operacionais para rastrear a aquisição de registros de fontes de API utilizando um Programa padrão do Marketo Engage.

## Resumo do canal {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Canal</th>
   <th>Status da associação</th>
   <th>Comportamento das análises</th>
   <th>Tipo de programa</th>
  </tr>
  <tr>
   <td>Operacional</td>
   <td>01-Membro</td>
   <td>Operacional</td>
   <td>Padrão</td>
  </tr>
 </tbody>
</table>

## O programa contém o seguinte Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nome do modelo</th>
   <th>Nome do ativo</th>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>Definir aquisição - Lote</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>Definir aquisição - Acionador</td>
  </tr>
  <tr>
   <td>Pasta</td>
   <td> </td>
   <td>Campanhas (contém todas as Campanhas inteligentes)</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

## Regras de conflito {#conflict-rules}

* **Marcas do programa**
   * Criar marcas nesta assinatura - _Recomendado_
   * Ignorar

* **Modelo de página de aterrissagem com o mesmo nome**
   * Copiar modelo original - _Recomendado_
   * Usar modelo de destino

* **Imagens com o mesmo nome**
   * Manter ambos os arquivos - _Recomendado_
   * Substituir item desta inscrição

* **Modelos de email com o mesmo nome**
   * Manter ambos os modelos - _Recomendado_
   * Substituir modelo existente

## Práticas recomendadas {#best-practices}

* Execute a Campanha em lote primeiro se precisar acompanhar o gerenciamento de dados.

* Considere utilizar programas semelhantes para garantir o alinhamento às práticas recomendadas em todas as fontes de entrada para incluir seu CRM ou Integrações de dados.

* Nas iniciativas de marketing de canal específicas, certifique-se de que a aquisição seja capturada quando necessário.
