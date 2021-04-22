---
unique-page-id: 557312
description: Glossário de operadores de filtro de lista inteligente - Documentos do Marketo - Documentação do produto
title: Glossário de operadores de filtro de lista inteligente
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 12%

---

# Glossário de operadores de filtro de lista inteligente {#smart-list-filter-operators-glossary}

Um operador faz parte da lista inteligente que ajuda a obter detalhes específicos. Ele permite descrever o filtro ou acionador em um idioma direto. Os operadores disponíveis são diferentes para cada tipo de campo.

Este é um glossário descrevendo cada conjunto de operadores.

## Campos de data {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Ao escolher um operador, o lado direito será alterado dinamicamente.

| Operador | Lado direito | Descrição |
|---|---|---|
| é | Data única | Correspondência de data exata |
| não é | Data única | Qualquer data, EXCETO a especificada |
| entre | Dois campos de data | Qualquer data incluindo e entre duas datas especificadas |
| no passado | Entrada de linguagem natural* | Consulte o diagrama abaixo |
| no passado antes de | Entrada de linguagem natural* | Consulte o diagrama abaixo |
| no futuro | Entrada de linguagem natural* | Consulte o diagrama abaixo |
| no futuro depois de | Entrada de linguagem natural* | Consulte o diagrama abaixo |
| no período de tempo | Predefinições (último trimestre, ontem etc.) | Definido na lista de seleção |
| depois  | Data única | Todos os registros após a data especificada |
| antes | Data única | Todos os registros antes do especificado |
| sobre ou depois de  | Data única | Igual a &quot;depois&quot;, mas inclusivo |
| em ou antes de | Data única | Igual a &quot;antes&quot;, mas inclusivo |
| está vazio | Nenhum(a) | Todos os registros sem data |
| não está vazio | Nenhum(a) | Todos os registros com qualquer data |

* A entrada de linguagem natural é legal. Estes são alguns dos padrões que você pode inserir:

* 1 hora
* 82 dias
* 3 semanas
* 14 meses
* 1 ano

Basta digitar o número e a unidade juntos e vai funcionar!

>[!NOTE]
>
>&quot;No passado&quot; **faz** inclui o dia (até a hora, não depois) em que você cria sua lista inteligente.

>[!CAUTION]
>
>Ao criar uma lista inteligente usando um filtro de campo de data (por exemplo, Data de nascimento, Data de criação de SFDC) e usar as restrições **before** ou **on or before**, a lista inteligente também incluirá pessoas que não têm valor nesse campo de data.

Use o diagrama a seguir para entender a diferença entre os operadores de data.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Exemplo**
>
>Os campos de data podem ficar complicados quando você está trabalhando com eventos passados e futuros. Aqui estão alguns exemplos.
>
>**Anteriormente antes**
>
>Para sua nova promoção, use esse operador para enviar emails somente para pessoas que não assinaram ou renovaram seu serviço em um ano ou que nunca foram assinantes.
>
>**No futuro, após**
>
>Digamos que você queira ver os clientes que estão prontos para a renovação em 90 dias. Você usaria dois filtros separados. Primeiro use &quot;No futuro após 90 dias&quot; e, segundo, &quot;No futuro, 91 dias&quot;. Isso capturaria quem tiver uma data daqui a 90 dias.

## Campos de string {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operador | Descrição |
|---|---|
| é | Correspondência exata (não diferencia maiúsculas de minúsculas) |
| não é | Qualquer coisa exceto correspondência exata |
| inicia com | As primeiras letras de correspondência da string |
| não inicia com | As primeiras letras da string NÃO correspondem |
| contém | Todas as letras juntas na string correspondem (exemplo: califórnia, fortuna, para o efeito) |
| não contém | Nenhuma letra junto na corda corresponde. (inverso de &quot;contém&quot;) |
| está vazio | Registros que não têm valor (NULL) |
| não está vazio | Registros com QUALQUER valor |

>[!TIP]
>
>Use operadores positivos em vez de negativos. Os filtros &quot;Não é&quot; precisam pesquisar todo o conjunto de dados na sua instância, o que pode ser extremamente demorado. Filtros positivos &quot;is&quot; podem aproveitar algoritmos de pesquisa mais eficazes.

## Campos inteiros {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Operador</th> 
   <th colspan="1" rowspan="1">Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">é</td> 
   <td colspan="1" rowspan="1">Correspondência de número exato ( = 0 retornará ambos os leads com 0 <em>e</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">não é</td> 
   <td colspan="1" rowspan="1">Qualquer coisa exceto número exato corresponde</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">entre</td> 
   <td colspan="1" rowspan="1">Defina dois valores para encontrar todos entre eles (inclusivo)</td> 
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
   <td colspan="1" rowspan="1">no mínimo</td> 
   <td colspan="1" rowspan="1">Acima do especificado (inclusivo)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no máximo</td> 
   <td colspan="1" rowspan="1">Menor que o especificado (inclusivo)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">está vazio</td> 
   <td colspan="1" rowspan="1">Registros que não têm valor (NULL) - zero é um número, <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">não está vazio</td> 
   <td colspan="1" rowspan="1">Registros com QUALQUER valor (incluindo zero)</td> 
  </tr> 
 </tbody> 
</table>

Como você pode ver, esses operadores facilitam a conversa com o Marketo-ese com fluência!
