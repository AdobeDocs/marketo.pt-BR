---
description: Gerenciamento OP-Lead - Documentação do Marketo - Documentação do produto
title: OP-Gerenciamento de leads
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 16%

---

# OP-Gerenciamento de leads {#op-lead-management}

Este é um exemplo de fluxos de trabalho de práticas recomendadas de gerenciamento de clientes potenciais, utilizando um Programa padrão do Marketo Engage para ajudá-lo a gerenciar registros no banco de dados do Marketo Engage para o seu CRM.

>[!NOTE]
>
>No Marketo Engage, os registros no banco de dados são chamados de pessoas/pessoa. O gerenciamento de clientes potenciais neste exemplo refere-se aos registros em seu CRM.

Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a Equipe de Conta da Adobe ou visite a página [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html).

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
   <td>01 - Sincronizar Novas Pessoas com o CRM</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>02 - Qualificado para marketing</td>
  </tr>
  <tr>
   <td>Email</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de email de início rápido</a></td>
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
   <td>Alerta de email</td>
  </tr>
 </tbody>
</table>

![](assets/op-lead-management-1.png)

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

* Considere adicionar outras Campanhas inteligentes para atender a cada uma das necessidades de status do ciclo de vida que você possa estar rastreando em sua organização. Cada campanha integrada neste programa deve ser um exemplo da criação de práticas recomendadas e não específica para todos os casos de uso. Lembre-se de atualizar as Campanhas inteligentes para lidar com o processo específico de gerenciamento do ciclo de vida dos clientes potenciais.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar com a sua.
