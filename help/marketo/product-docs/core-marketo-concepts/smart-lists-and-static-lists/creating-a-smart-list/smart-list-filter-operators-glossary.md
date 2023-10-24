---
unique-page-id: 557312
description: Glossário de operadores de filtro de lista inteligente - Documentação do Marketo - Documentação do produto
title: Glossário de operadores de filtro de lista inteligente
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 12%

---

# Glossário de operadores de filtro de lista inteligente {#smart-list-filter-operators-glossary}

Um operador é parte da Smart List que ajuda a obter informações específicas. Ele permite descrever o filtro ou acionador em uma linguagem simples. Os operadores disponíveis são diferentes para cada tipo de campo.

Aqui está um glossário descrevendo cada conjunto de operadores.

## Campos de data {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Quando você escolhe um operador, o lado direito muda dinamicamente.

| Operador | Lado direito | Descrição |
|---|---|---|
| é | Data única | Correspondência de data exata |
| não é | Data única | Qualquer data, EXCETO a especificada |
| entre | Dois campos de data | Qualquer data incluindo e entre duas datas especificadas |
| no passado | Entrada de linguagem natural&#42; | Consulte o diagrama abaixo |
| no passado antes de | Entrada de linguagem natural&#42; | Consulte o diagrama abaixo |
| no futuro | Entrada de linguagem natural&#42; | Consulte o diagrama abaixo |
| no futuro depois de | Entrada de linguagem natural&#42; | Consulte o diagrama abaixo |
| no intervalo de tempo | Predefinições (último trimestre, ontem etc.) | Definido na lista de opções |
| depois | Data única | Todos os registros após a data especificada |
| antes | Data única | Todos os registros antes do especificado |
| em ou depois de | Data única | O mesmo que &quot;depois&quot;, mas inclusivo |
| em ou antes de | Data única | O mesmo que &quot;antes&quot;, mas inclusivo |
| está vazio | Nenhum | Todos os registros sem data |
| não está vazio | Nenhum | Todos os registros com qualquer data |

&#42; A entrada da linguagem natural é legal. Estes são alguns dos padrões que você pode inserir:

* 1 hora
* 82 dias
* 3 semanas
* 14 meses
* 1 ano

Basta digitar o número e a unidade juntos e vai funcionar!

>[!NOTE]
>
>&quot;No passado&quot; _faz_ inclua o dia (até a hora, não depois) em que você criou sua Smart List.

>[!CAUTION]
>
>Ao criar uma Smart List usando um filtro de campo de data (por exemplo, Data de nascimento, Data de criação do SFDC) e usar as restrições **[!UICONTROL antes]**, **[!UICONTROL em ou antes de]** ou **[!UICONTROL no passado antes]**, a Smart List também incluirá pessoas que não têm valor no campo de data.

Use o diagrama a seguir para entender a diferença entre os operadores de data.

![](assets/image2014-9-10-17-3a15-3a58.png)

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
>**[!UICONTROL No futuro, após]**
>
>Digamos que você queira ver os clientes que estão prontos para renovação em 90 dias. Você usaria dois filtros separados. Primeiro use &quot;No futuro, após 90 dias&quot; e, segundo, &quot;No futuro, 91 dias&quot;. Isso capturaria quem tiver uma data daqui a 90 dias.

## Campos de string {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operador | Descrição |
|---|---|
| é | Correspondência exata (não diferencia maiúsculas de minúsculas) |
| não é | Qualquer coisa, EXCETO a correspondência exata |
| inicia com | As primeiras letras da correspondência de sequência de caracteres |
| não inicia com | As primeiras letras da sequência DE caracteres NÃO correspondem |
| contém | Todas as letras juntas na correspondência de sequência de caracteres (exemplo: california, fortune, portanto) |
| não contém | Nenhuma letra junto na sequência de caracteres corresponde. (reverso de &quot;contém&quot;) |
| está vazio | Registros que não têm valor (NULL) |
| não está vazio | Registros com qualquer valor |

>[!TIP]
>
>Use operadores positivos em vez de negativos. Os filtros &quot;Não é&quot; precisam pesquisar todo o conjunto de dados na sua instância, o que pode ser extremamente demorado. Os filtros positivos &quot;is&quot; podem utilizar algoritmos de pesquisa mais eficazes.

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
   <td colspan="1" rowspan="1">A correspondência exata do número ( = 0) retornará ambos os leads com 0 <em>e</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">não é</td> 
   <td colspan="1" rowspan="1">Qualquer coisa, EXCETO o número exato, corresponde</td> 
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
   <td colspan="1" rowspan="1">Acima do especificado (inclusive)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">no máximo</td> 
   <td colspan="1" rowspan="1">Menor que o especificado (inclusive)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">está vazio</td> 
   <td colspan="1" rowspan="1">Registros que não têm valor (NULL) - zero é um número, é <em>não</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">não está vazio</td> 
   <td colspan="1" rowspan="1">Registros com qualquer valor (incluindo zero)</td> 
  </tr> 
 </tbody> 
</table>

Como você pode ver, esses operadores facilitam a fala em Marketo com fluência!
