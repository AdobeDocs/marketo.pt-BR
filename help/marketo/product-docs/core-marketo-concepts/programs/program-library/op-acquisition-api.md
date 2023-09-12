---
description: OP-Acquisition-API - Documentação do Marketo - Documentação do produto
title: API de aquisição OP
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 27%

---

# API de aquisição OP {#op-acquisition-api}

Este programa de exemplo é para processos operacionais para rastrear a aquisição de registros de fontes de API utilizando um Programa padrão Marketo Engage.

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

## O programa contém os seguintes ativos {#program-contains-the-following-assets}

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

* **Marcas de programa**
   * Criar tags nesta assinatura - _Recomendado_
   * Ignorar

* **Modelo de landing page com o mesmo nome**
   * Copiar modelo original - _Recomendado_
   * Usar modelo de destino

* **Imagens com o mesmo nome**
   * Manter ambos os arquivos - _Recomendado_
   * Substituir item desta inscrição

* **Modelos de e-mail com o mesmo nome**
   * Manter ambos os modelos - _Recomendado_
   * Substituir modelo existente

## Práticas recomendadas {#best-practices}

* Execute a Campanha em lote primeiro se precisar acompanhar o gerenciamento de dados.

* Considere utilizar programas semelhantes para garantir o alinhamento às práticas recomendadas em todas as fontes de entrada para incluir seu CRM ou Integrações de dados.

* Em iniciativas de marketing de canal específicas, capture a aquisição quando necessário.
