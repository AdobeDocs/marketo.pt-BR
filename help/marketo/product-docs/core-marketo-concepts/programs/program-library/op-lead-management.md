---
description: Gerenciamento OP-Lead - Documentação do Marketo - Documentação do produto
title: Gerenciamento OP-Lead
feature: Programs
exl-id: 28db1a91-a559-4dcb-b2e3-9cb2c0c23f9f
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 19%

---

# Gerenciamento OP-Lead {#op-lead-management}

Este é um exemplo de fluxos de trabalho de práticas recomendadas de gerenciamento de clientes potenciais, utilizando um Programa padrão de Marketo Engage, para ajudá-lo a gerenciar registros no banco de dados de Marketo Engage para o seu CRM.

>[!NOTE]
>
>No Marketo Engage, os registros no banco de dados são chamados de pessoas/pessoa. O gerenciamento de clientes potenciais neste exemplo refere-se aos registros em seu CRM.

Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a equipe de conta do Adobe ou visite o [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) página.

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
   <td>01 - Sincronizar Novas Pessoas com o CRM</td>
  </tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>02 - Qualificado para marketing</td>
  </tr>
  <tr> 
   <td>Email</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>01 - E-mail - ALERTA - MQL</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Campanhas</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Alerta de e-mail</td>
  </tr>
 </tbody> 
</table>

![](assets/op-lead-management-1.png)

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

* Considere adicionar outras Campanhas inteligentes para atender a cada uma das necessidades de status do ciclo de vida que você possa estar rastreando em sua organização. Cada campanha integrada neste programa deve ser um exemplo da criação de práticas recomendadas e não específica para todos os casos de uso. Lembre-se de atualizar as Campanhas inteligentes para lidar com o processo específico de gerenciamento do ciclo de vida dos clientes potenciais.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar com a sua.
