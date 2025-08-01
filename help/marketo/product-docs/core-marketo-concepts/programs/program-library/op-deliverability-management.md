---
description: OP-Deliverability Management - Documentação do Marketo - Documentação do produto
title: Gerenciamento de Entregabilidade OP
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 19%

---

# Gerenciamento de Entregabilidade OP {#op-deliverability-management}

Este é um exemplo de workflows de práticas recomendadas de gerenciamento de entrega que utilizam um Programa padrão do Marketo Engage, para analisar seu estado atual de capacidade de entrega de email e gerenciar rejeições crônicas e usuários que não respondem.

>[!NOTE]
>
>Exige que o campo de sequência personalizado &quot;Motivo da suspensão de marketing&quot; seja importado. [Saiba mais](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a Equipe de Conta da Adobe ou visite a página [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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

## Campos de pré-requisito {#prerequisite-fields}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nome intuitivo</th>
   <th>Nome da API</th>
  </tr>
  <tr>
   <td>String</td>
   <td>Motivo da suspensão de marketing</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Não-respondedores crônicos de suspensão de marketing</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>Suspensão de marketing: emails com rejeição crônica</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>Redefinir "Email inválido" após a atualização de email</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>Redefinir "Marketing suspenso" após a atualização de email</td>
  </tr>
  <tr>
   <td>Pasta</td>
   <td> </td>
   <td>Gerenciar</td>
  </tr>
  <tr>
   <td>Pasta</td>
   <td> </td>
   <td>Revisar</td>
  </tr>
 </tbody>
</table>

![](assets/op-deliverability-management-1.png)

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

* Cada campanha criada deve ser um exemplo na criação de práticas recomendadas e não específica para seus casos de uso. Lembre-se de atualizar as Campanhas inteligentes para lidar com seus pontos problemáticos específicos e desafios de dados.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar-se à sua convenção de nomenclatura.
