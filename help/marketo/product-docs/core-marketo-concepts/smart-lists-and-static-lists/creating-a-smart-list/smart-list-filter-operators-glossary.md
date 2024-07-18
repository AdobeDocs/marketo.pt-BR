---
unique-page-id: 557312
description: Glossário de operadores de filtro de lista inteligente - Documentação do Marketo - Documentação do produto
title: Glossário de operadores de filtro de lista inteligente
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 13%

---

# Glossário de operadores de filtro de lista inteligente {#smart-list-filter-operators-glossary}

Um operador é parte da Smart List que ajuda a obter informações específicas. Ele permite descrever o filtro ou acionador em uma linguagem simples. Os operadores disponíveis são diferentes para cada tipo de campo.

Aqui está um glossário descrevendo cada conjunto de operadores.

## Campos de data {#date-fields}

![](assets/smart-list-filter-operators-glossary-1.png)

Quando você escolhe um operador, o lado direito muda dinamicamente.

<table><thead>
  <tr>
    <th>Operador</th>
    <th>Lado direito</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>é</td>
    <td>Data única</td>
    <td>Correspondência de data exata</td>
  </tr>
  <tr>
    <td>não é</td>
    <td>Data única</td>
    <td>Qualquer data, EXCETO a especificada</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Dois campos de data</td>
    <td>Qualquer data incluindo e entre duas datas especificadas</td>
  </tr>
  <tr>
    <td>no passado</td>
    <td>Entrada de linguagem natural*</td>
    <td>Consulte o diagrama abaixo</td>
  </tr>
  <tr>
    <td>no passado antes de</td>
    <td>Entrada de linguagem natural*</td>
    <td>Consulte o diagrama abaixo</td>
  </tr>
  <tr>
    <td>no futuro</td>
    <td>Entrada de linguagem natural*</td>
    <td>Consulte o diagrama abaixo</td>
  </tr>
  <tr>
    <td>no futuro depois de</td>
    <td>Entrada de linguagem natural*</td>
    <td>Consulte o diagrama abaixo</td>
  </tr>
  <tr>
    <td>no período de tempo</td>
    <td>Predefinições (último trimestre, ontem etc.)</td>
    <td>Definido na lista de opções</td>
  </tr>
  <tr>
    <td>depois</td>
    <td>Data única</td>
    <td>Todos os registros após a data especificada</td>
  </tr>
  <tr>
    <td>antes</td>
    <td>Data única</td>
    <td>Todos os registros antes do especificado</td>
  </tr>
  <tr>
    <td>em ou depois de</td>
    <td>Data única</td>
    <td>O mesmo que "depois", mas inclusivo</td>
  </tr>
  <tr>
    <td>em ou antes de</td>
    <td>Data única</td>
    <td>O mesmo que "antes", mas inclusivo</td>
  </tr>
  <tr>
    <td>está vazio</td>
    <td>Nenhum</td>
    <td>Todos os registros sem data</td>
  </tr>
  <tr>
    <td>não está vazio</td>
    <td>Nenhum</td>
    <td>Todos os registros com qualquer data</td>
  </tr>
</tbody></table>

**&#42;** A entrada de linguagem natural é legal. Estes são alguns dos padrões que você pode inserir:

* 1 hora
* 82 dias
* 3 semanas
* 14 meses
* 1 ano

Basta digitar o número e a unidade juntos e vai funcionar!

>[!NOTE]
>
>&quot;No passado&quot; _inclui_ o dia (até o momento, não depois) em que você cria sua Lista Inteligente.

>[!CAUTION]
>
>Ao criar uma Smart List usando um filtro de campo de data (por exemplo, Data de Nascimento, Data de Criação do SFDC) e usar as restrições **[!UICONTROL antes]**, **[!UICONTROL em ou antes]** ou **[!UICONTROL no passado antes]**, a Smart List também incluirá pessoas que não têm valor nesse campo de data.

Use o diagrama a seguir para entender a diferença entre os operadores de data.

![](assets/smart-list-filter-operators-glossary-2.png)

>[!NOTE]
>
>**Exemplo**
>
>Os campos de data podem complicar quando você está trabalhando com eventos passados e futuros. Veja alguns exemplos.
>
>**[!UICONTROL No passado antes]**
>
>Na nova promoção, use esse operador para enviar emails somente para pessoas que não assinaram ou renovaram seu serviço em um ano ou que nunca foram assinantes.
>
>**[!UICONTROL No futuro após]**
>
>Digamos que você queira ver os clientes que estão prontos para renovação em 90 dias. Você usaria dois filtros separados. Primeiro use &quot;No futuro, após 90 dias&quot; e, segundo, &quot;No futuro, 91 dias&quot;. Isso capturaria quem tiver uma data daqui a 90 dias.

## Campos de string {#string-fields}

![](assets/smart-list-filter-operators-glossary-3.png)

<table><thead>
  <tr>
    <th>Operador</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>é</td>
    <td>Correspondência exata (não diferencia maiúsculas de minúsculas)</td>
  </tr>
  <tr>
    <td>não é</td>
    <td>Qualquer coisa, EXCETO a correspondência exata</td>
  </tr>
  <tr>
    <td>inicia com</td>
    <td>As primeiras letras da correspondência de sequência de caracteres</td>
  </tr>
  <tr>
    <td>não inicia com</td>
    <td>As primeiras letras da sequência DE caracteres NÃO correspondem</td>
  </tr>
  <tr>
    <td>contém</td>
    <td>Todas as letras juntas na correspondência de sequência de caracteres (exemplo: california, fortune, portanto)</td>
  </tr>
  <tr>
    <td>não contém</td>
    <td>Nenhuma letra junto na sequência de caracteres corresponde. (reverso de "contém")</td>
  </tr>
  <tr>
    <td>está vazio</td>
    <td>Registros que não têm valor (NULL)</td>
  </tr>
  <tr>
    <td>não está vazio</td>
    <td>Registros com qualquer valor</td>
  </tr>
</tbody>
</table>

>[!TIP]
>
>Use operadores positivos em vez de negativos. Os filtros &quot;Não é&quot; precisam pesquisar todo o conjunto de dados na sua instância, o que pode ser extremamente demorado. Os filtros positivos &quot;is&quot; podem utilizar algoritmos de pesquisa mais eficazes.

## Campos inteiros {#integer-fields}

![](assets/smart-list-filter-operators-glossary-4.png)

<table><thead>
  <tr>
    <th>Operador</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>é</td>
    <td>Correspondência de número exato ( = 0 retornará ambos os leads com 0 e NULL)</td>
  </tr>
  <tr>
    <td>não é</td>
    <td>Qualquer coisa, EXCETO o número exato, corresponde</td>
  </tr>
  <tr>
    <td>entre</td>
    <td>Defina dois valores para encontrar todos entre eles (inclusivo)</td>
  </tr>
  <tr>
    <td>maior que</td>
    <td>Acima do especificado</td>
  </tr>
  <tr>
    <td>menor que</td>
    <td>Menor que o especificado</td>
  </tr>
  <tr>
    <td>no mínimo</td>
    <td>Acima do especificado (inclusive)</td>
  </tr>
  <tr>
    <td>no máximo</td>
    <td>Menor que o especificado (inclusive)</td>
  </tr>
  <tr>
    <td>está vazio</td>
    <td>Registros que não têm valor (NULL) - zero é um número, ele não é NULL</td>
  </tr>
  <tr>
    <td>não está vazio</td>
    <td>Registros com qualquer valor (incluindo zero)</td>
  </tr>
</tbody>
</table>

Como você pode ver, esses operadores facilitam a fala em Marketo com fluência!
