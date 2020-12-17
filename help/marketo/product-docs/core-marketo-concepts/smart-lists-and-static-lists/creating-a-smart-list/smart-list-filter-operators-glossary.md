---
unique-page-id: 557312
description: Glossário de operadores de filtro de Lista inteligente - Documentos do marketing - Documentação do produto
title: Glossário de operadores de filtro de Lista inteligente
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---


# Glossário de operadores de filtro de Lista inteligente {#smart-list-filter-operators-glossary}

Um operador faz parte da [lista inteligente](http://docs.marketo.com/display/docs/smart+lists+and+static+lists) que ajuda você a obter informações específicas. Ele permite que você descreva seu filtro ou acionador em um idioma simples. Os operadores disponíveis são diferentes para cada tipo de campo.\
Aqui está um glossário descrevendo cada conjunto de operadores.

## Campos de data {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Ao escolher um operador, o lado direito mudará dinamicamente.

| Operador | Lado direito | Descrição |
|---|---|---|
| is | Data única | Correspondência de data exata |
| não é | Data única | Qualquer data, EXCETO a especificada |
| between | Dois campos de data | Qualquer data incluindo e entre duas datas especificadas |
| no passado | Entrada de Idioma Natural* | Consulte o diagrama abaixo |
| anteriormente | Entrada de Idioma Natural* | Consulte o diagrama abaixo |
| no futuro | Entrada de Idioma Natural* | Consulte o diagrama abaixo |
| no futuro, após | Entrada de Idioma Natural* | Consulte o diagrama abaixo |
| no período | Predefinições (último trimestre, ontem etc.) | Definido na lista de seleção |
| after | Data única | Todos os registros após a data especificada |
| before | Data única | Todos os registros antes do especificado |
| em ou após | Data única | Igual a &quot;depois&quot;, mas inclusivo |
| em ou antes | Data única | Igual a &quot;antes&quot;, mas inclusivo |
| está vazio | Nenhum | Todos os registros sem data |
| não está vazio | Nenhum | Todos os registros com qualquer data |

* A entrada de linguagem natural é legal. Estes são alguns dos padrões que você pode inserir:

* 1 hora
* 82 dias
* 3 semanas
* 14 meses
* 1 ano

Basta digitar o número e a unidade juntos e vai funcionar!

>[!NOTE]
>
>No passado, **inclui** o dia (até a hora, não depois) que você cria sua lista inteligente.

>[!CAUTION]
>
>Ao criar uma lista inteligente usando um filtro de campo de data (por exemplo, Data de nascimento, Data de criação SFDC) e usar as restrições **before** ou **em ou antes de**, a lista inteligente também incluirá pessoas que não têm valor nesse campo de data.

Use o diagrama a seguir para entender a diferença entre os operadores de data.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Exemplo**
>
>Os campos de data podem ficar complicados quando você trabalha com eventos passados e futuros. Aqui estão alguns exemplos.
>
>**Antes**
>
>Para sua nova promoção, use este operador para enviar emails somente para pessoas que não se inscreveram ou renovaram seu serviço em um ano ou que nunca foram assinantes.
>
>**No futuro, após**
>
>Diga que você quer ver os clientes que estão prontos para renovação em 90 dias. Você usaria dois filtros separados. Primeira utilização &quot;No futuro após 90 dias&quot; e segunda, &quot;No futuro, 91 dias&quot;. Isso capturaria quem tiver uma data daqui a 90 dias.

## Campos de cadeia de caracteres {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operador | Descrição |
|---|---|
| is | Correspondência exata (não diferencia maiúsculas de minúsculas) |
| não é | Qualquer coisa, exceto correspondência exata |
| start com | As primeiras letras da correspondência de corda |
| não start com | As primeiras letras da string NÃO correspondem |
| contém | Todas as letras juntas na string correspondem (por exemplo: california, fortuna, portanto) |
| not contains | Nenhuma letra junto na corda corresponde. (verso de &quot;contém&quot;) |
| está vazio | Registros sem valor (NULL) |
| não está vazio | Registros com QUALQUER valor |

>[!TIP]
>
>Use operadores positivos em vez de negativos. Os filtros &quot;Não é&quot; precisam pesquisar todo o conjunto de dados em sua instância, o que pode ser extremamente demorado. Filtros positivos &quot;is&quot; podem alavancar algoritmos de pesquisa mais eficazes.

## Campos inteiros {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Operador</th> 
   <th colspan="1" rowspan="1"><p>Descrição</p></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">Correspondência exata de números ( = 0 retornará ambos os clientes potenciais com 0 <em>e</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">não é</td> 
   <td colspan="1" rowspan="1">Qualquer coisa, EXCETO o número exato correspondente</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">between</td> 
   <td colspan="1" rowspan="1">Defina dois valores para encontrar todos entre eles (inclusive)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">maior que</td> 
   <td colspan="1" rowspan="1">Acima do especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">menor que</td> 
   <td colspan="1" rowspan="1">Menor que o especificado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">mínimo</td> 
   <td colspan="1" rowspan="1">Acima do especificado (inclusivo)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no máximo</td> 
   <td colspan="1" rowspan="1">Menor que o especificado (inclusivo)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">está vazio</td> 
   <td colspan="1" rowspan="1">Registros sem valor (NULL) - zero é um número, é <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">não está vazio</td> 
   <td colspan="1" rowspan="1">Registros com QUALQUER valor (incluindo zero)</td> 
  </tr> 
 </tbody> 
</table>

Como podem ver, estes operadores facilitam a fala de Marketo-ese com fluência!
