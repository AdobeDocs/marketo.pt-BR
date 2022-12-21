---
unique-page-id: 2951877
description: Noções básicas sobre a área de análise de oportunidade do programa - Documentos da Marketo - Documentação do produto
title: Noções Gerais da Área de Análise de Oportunidades do Programa
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 20%

---

# Noções Gerais da Área de Análise de Oportunidades do Programa {#understanding-the-program-opportunity-analysis-area}

## Visão geral {#overview}

A área Análise de oportunidade do programa permite analisar a eficácia de programas individuais ou ver resultados resumidos por Canal do programa.

**Exemplo de perguntas comerciais que você pode responder usando essa área de análise incluem**:

Quantas oportunidades foram associadas a um programa específico e quantas delas ganhámos?

![](assets/one-1.png)

Quanta receita um determinado Programa ou Canal ajudou a gerar?

![](assets/two-1.png)

Qual é minha receita para o investimento em um determinado programa ou canal?

![](assets/three-1.png)

Que oportunidades influenciou um programa específico?

![](assets/four-1.png)

## Medidas de atribuição da análise de oportunidade do programa (pontos azuis) {#program-opportunity-analysis-attribution-measures-blue-dots}

As medidas disponíveis para você usar na análise são geralmente números e são representadas por pontos azuis. Dimension são atributos que oferecem diferentes visualizações das medidas e são representados por pontos amarelos.

Todas as medidas (pontos azuis) estão relacionadas à atribuição - o &quot;crédito&quot; para aquisição de cliente potencial ou para o sucesso de vendas associado a um cliente potencial.

![](assets/six.five.png) ![](assets/seven-1.png)

Existem três tipos de medidas:

* Medidas relacionadas à aquisição, que obtêm atribuição de primeiro toque (FT).
* Medidas relacionadas ao sucesso, que recebem atribuição de multitoque (MT).
* Diversas medidas relacionadas ao Programa, incluindo o número médio de toques de marketing antes da criação ou do fechamento de Oportunidades.

## Aquisição e medidas relacionadas ao sucesso {#acquisition-and-success-related-measures}

As medidas relacionadas com a aquisição dão crédito ao programa através do qual as informações de contato de um cliente potencial são obtidas pela primeira vez. Um cliente potencial não tem de ser bem sucedido num programa de concessão de crédito de aquisição.

O valor de adquirir um determinado lead é alterado ao longo do tempo. É zero até que uma compra seja feita pelo cliente potencial. Em seguida, ele pode aumentar com compras adicionais.

As medidas relacionadas com o sucesso dão crédito a todos os programas que contribuem para os progressos de um cliente potencial no sentido de uma compra.

Assim como com a aquisição, o valor de contribuir com as vendas feitas a um cliente potencial muda ao longo do tempo, e é zero até que alguma compra seja feita pelo cliente potencial.

<table> 
 <tbody> 
  <tr> 
   <th>Medida de atribuição - Relacionada à oportunidade (FT ou MT)*</th> 
   <th>Descrição</th> 
  </tr> 
  <tr> 
   <td>Custo da Oportunidade</td> 
   <td>A parte do custo do programa que influenciou a oportunidade. O custo pode ser dividido se houver vários leads envolvidos.</td> 
  </tr> 
  <tr> 
   <td>Oportunidades criadas</td> 
   <td>A parte do crédito que o programa recebeu por influenciar a criação da oportunidade. Pode ser uma fração, caso haja mais de um lead envolvido.</td> 
  </tr> 
  <tr> 
   <td>Oportunidades conquistadas</td> 
   <td>A parte do crédito que o programa recebeu por influenciar a oportunidade vencedora. Pode ser uma fração, caso haja mais de um lead envolvido.</td> 
  </tr> 
  <tr> 
   <td>Processamento criado</td> 
   <td>Porção de crédito (em valores monetários) recebida pelo programa para influenciar a criação da oportunidade. Pode ser uma fração, caso haja mais de um lead envolvido.</td> 
  </tr> 
  <tr> 
   <td>Pipeline criado - Ainda aberto</td> 
   <td>Porção de crédito (em valores monetários) recebida pelo programa para influenciar a criação da oportunidade atualmente aberta. Pode ser uma fração, caso haja mais de um lead envolvido.</td> 
  </tr> 
  <tr> 
   <td>Receita esperada</td> 
   <td>Porção de crédito (em valores monetários) recebida pelo programa para influenciar a criação da oportunidade. A receita prevista é a probabilidade da oportunidade multiplicada pelo valor da oportunidade. Pode ser uma fração, caso haja mais de um lead envolvido.</td> 
  </tr> 
  <tr> 
   <td>Receitas De Investimento</td> 
   <td>Relação entre a porção de crédito (em valores monetários) recebida pelo programa para influenciar oportunidades conquistadas e o custo do programa.</td> 
  </tr> 
  <tr> 
   <td>Receita conquistada</td> 
   <td>Porção de crédito (em valores monetários) recebida pelo programa para influenciar uma oportunidade conquistada. Pode ser uma fração, caso haja mais de um lead envolvido.</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) = Atribuição de Primeiro Toque, utilizada para medidas de aquisição de chumbo; (MT) = Atribuição multitoque, usada para medidas de sucesso de lead_

Abaixo está um cenário que descreve como as Unidades de Oportunidade são calculadas quando há dois Programas que geraram leads, mas esses levam a uma Oportunidade da mesma conta.

**Programa 1**

* Gera um lead: Lead 1
* O lead 1 é da Conta 1

**Programa 2**

* Gera outro lead: Lead 2
* O lead 2 também é da Conta 1

**Conta 1**

* Gera uma Oportunidade: Oportunidade 1

O Marketo dá crédito adequadamente sem dupla contagem de oportunidades entre programas. Assim, neste caso, cada Programa recebe 0,5 Unidades de Oportunidade. Ou seja, cada Programa recebe metade do crédito pela Oportunidade gerada. Além disso, metade da receita associada à Oportunidade é atribuída a cada Programa.

## Medidas Diversas Relacionadas com Programas {#miscellaneous-program-related-measures}

As outras medidas disponíveis refletem o desempenho global do Programa.

<table> 
 <tbody> 
  <tr> 
   <th>Medida de atribuição - Relacionada ao programa</th> 
   <th>Descrição</th> 
  </tr> 
  <tr> 
   <td>Nº de Oportunidades Associadas ao Programa</td> 
   <td><p>O número total de Oportunidades que tinham dado qualquer tipo de crédito de atribuição a um programa. As oportunidades podem ser influenciadas por um ou mais leads e por um ou mais Programas.</p></td> 
  </tr> 
  <tr> 
   <td>Número Médio de Sucessos por Oportunidade Fechada</td> 
   <td>O número médio de sucessos do Programa antes do encerramento da Oportunidade. <br></td> 
  </tr> 
  <tr> 
   <td>Número médio de sucessos por oportunidade criada</td> 
   <td>O número médio de programas bem-sucedidos antes da criação da Oportunidade.</td> 
  </tr> 
  <tr> 
   <td>Novos nomes</td> 
   <td>O número total de novos nomes, ou seja, novos leads, adquiridos pelo Programa.</td> 
  </tr> 
  <tr> 
   <td>Custo do programa</td> 
   <td>Custo total do Programa.</td> 
  </tr> 
  <tr> 
   <td>Sucesso (total)</td> 
   <td>O número total de membros do Programa que obtiveram sucesso.</td> 
  </tr> 
 </tbody> 
</table>

## Dimension de análise da oportunidade do programa (pontos amarelos) {#program-opportunity-analysis-dimensions-yellow-dots}

Enquanto as medidas (pontos azuis) são calculadas e exigem reflexão e explicação para uso, as dimensões (pontos amarelos) são descritivas. Estas são as dimensões disponíveis.

<table> 
 <tbody> 
  <tr> 
   <th>Categoria</th> 
   <th>Exibir rótulo</th> 
  </tr> 
  <tr> 
   <td>Atributos da oportunidade</td> 
   <td>Oportunidade fechada<br>Nome da Oportunidade*<br>Nome do Proprietário da Oportunidade<br>Estágio da Oportunidade<br>Tipo de Oportunidade</td> 
  </tr> 
  <tr> 
   <td>Cronograma da oportunidade</td> 
   <td>Oportunidade Fechada Ano/Trimestre/Mês<br>Oportunidade Criada Ano/Trimestre/Mês</td> 
  </tr> 
  <tr> 
   <td>Atributos do programa</td> 
   <td>Canal do programa<br>Nome do programa</td> 
  </tr> 
  <tr> 
   <td>Cronograma de custo do programa</td> 
   <td>Ano/Trimestre/Mês de Custo</td> 
  </tr> 
 </tbody> 
</table>

*&#42;Todas as Oportunidades que deram qualquer tipo de crédito de atribuição a um Programa. As oportunidades podem ser influenciadas por um ou mais leads e por um ou mais Programas.*

>[!MORELIKETHIS]
>
>[Criar um relatório do explorador de receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
