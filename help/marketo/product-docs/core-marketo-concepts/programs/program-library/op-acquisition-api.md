---
description: OP-Acquisition-API - Documentação do Marketo - Documentação do produto
title: API de aquisição OP
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 19%

---

# API de aquisição OP {#op-acquisition-api}

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

* Em iniciativas de marketing de canal específicas, capture a aquisição quando necessário.
