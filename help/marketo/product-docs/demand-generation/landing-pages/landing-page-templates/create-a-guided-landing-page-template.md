---
unique-page-id: 7515401
description: Criar um modelo de página de aterrissagem guiada - Documentação do Marketo - Documentação do produto
title: Criar um modelo de página de aterrissagem guiada
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 1%

---

# Criar um modelo de página de aterrissagem guiada {#create-a-guided-landing-page-template}

Os templates de landing page guiados têm uma sintaxe especial. Use essa sintaxe para especificar o que é personalizável e onde o conteúdo acabará em cada página de aterrissagem criada a partir do seu modelo. Somente as regiões ou variáveis especificadas como editáveis estarão disponíveis para personalização no editor de página de aterrissagem &quot;Guiado&quot;.

>[!TIP]
>
>Use boas convenções de nomenclatura e sua equipe de marketing se apaixonará por você.

Há duas maneiras de declarar que algo em sua página deve ser editável:

* Declarar um objeto como um &quot;elemento&quot;. O criador da página de aterrissagem poderá adicionar imagens, texto ou ativos do Marketo nessas regiões especificadas.
* Declarar uma string como &quot;variável&quot;. O criador da página de aterrissagem poderá substituir essa variável por uma cadeia de caracteres, cor ou estado booleano a partir de uma alavanca true/false.

## Elementos editáveis {#editable-elements}

Os elementos são declarados adicionando um elemento DOM normal ao modelo e, em seguida, decorando o elemento com um nome de classe específico do Marketo.

## Texto {#text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [usando o Editor de Rich Text do Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Atributos obrigatórios:\
**classe**: &quot;mktoText&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
O conteúdo de um elemento com a classe mktoText (se fornecido) será usado como o valor padrão da região editável.

Exemplo:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Imagem {#image}

Você tem duas opções para definir Elementos de imagem editáveis. Você pode usar um `<div>`, que especifica um contêiner no qual a imagem será inserida, ou uma marca `<img>`.

## Opção 1 - Usar um `<div>` {#option-use-a-div}

Atributos obrigatórios:

class: &quot;mktoImg&quot;\
id: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
mktoName : Cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
mktoImgClass: String. O valor aqui será adicionado ao atributo de classe do elemento `<img>` dentro de div.

Exemplo:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Opção 2 - Usar um `<img>` {#option-use-a-img}

Atributos obrigatórios:\
class: &quot;mktoImg&quot;\
id: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
mktoName : Cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
src: URL da string. Ele será usado como valor padrão para a imagem.

Exemplo:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Ao usar a versão `<img>`, o HTML renderizado conterá um wrapper div gerado ao redor da tag `<img>`. Ele será definido como classe .&quot;mktoImg.mktoGen,&quot; e será display:inline-block.

## Formulário {#form}

Exemplo:Atributos obrigatórios:\
**classe**: &quot;mktoForm&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Bloco de conteúdo {#snippet}

Atributos obrigatórios:\
**classe**: &quot;mktoSnippet&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Compartilhar botão {#share-button}

Atributos obrigatórios:\
**classe**: &quot;mktoShareButton&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Vídeo {#video}

>[!NOTE]
>
>Ao usar o elemento de vídeo em uma página de aterrissagem, o Marketo só oferece suporte a vídeos do YouTube. Se você usar outro serviço, recomendamos utilizar uma caixa de rich text e colar no código incorporado do vídeo.

Atributos obrigatórios:
**classe**: &quot;mktoVideo&quot;
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Pesquisa {#poll}

Atributos obrigatórios:\
**classe**: &quot;mktoPoll&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Indicação {#referral}

Atributos obrigatórios:\
**classe**: &quot;mktoReferral&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Sorteios {#sweepstakes}

Atributos obrigatórios:\
**classe**: &quot;mktoSweepstakes&quot;\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Variáveis editáveis {#editable-variables}

Todos os tipos de variáveis são usados referenciando o valor de seu atributo id encapsulado dentro de uma sequência de caracteres ${ }. Elas podem ser usadas em qualquer lugar no documento, exceto dentro de outras declarações de variável.

Exemplo:

`${var1}`

**Declaração:**

As variáveis são declaradas como metatags dentro do elemento `<head>` do modelo. Há três tipos de variáveis disponíveis para uso: String, Cor e Booleano.

## Sequência de caracteres {#string}

Atributos necessários:\
**classe** : &quot;mktoString&quot;,\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
**padrão**: valor da cadeia de caracteres para o atributo. Em branco se nenhum for fornecido.\
**allowHtml**: &quot;true&quot; ou &quot;false&quot;. Controla se o valor será impresso sem ser escapado por HTML. O padrão é &quot;false&quot; se não estiver definido.

Exemplo básico:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Exemplo com todos os atributos:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Cor {#color}

Atributos necessários:\
**classe** : &quot;mktoColor&quot;,\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
**padrão**: um código de cor de caractere HEX de 7 dígitos. Por exemplo: &quot;#336699&quot;

Exemplo básico:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Exemplo com todos os atributos:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booleano {#boolean}

Atributos necessários:\
**classe** : &quot;mktoBoolean&quot;,\
**id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.\
**mktoName** : cadeia de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
**padrão**: cadeia de caracteres booleana. &quot;true&quot; ou &quot;false&quot; controla se o valor começa nas posições ON ou OFF. &quot;false&quot; se não fornecido.\
**false_value**: cadeia de caracteres. O valor a ser inserido para a variável quando ela estiver na posição OFF. &quot;false&quot; se não fornecido.\
**valor_verdadeiro**: cadeia de caracteres. O valor a ser inserido para a variável quando ela estiver na posição LIGADO. &quot;true&quot; se não for fornecido.\
**false_value_name**: cadeia de caracteres. O nome de exibição a ser mostrado no editor de landing page quando o valor estiver na posição OFF. &quot;OFF&quot; se não fornecido.\
**true_value_name**: cadeia de caracteres. O nome de exibição a ser mostrado no editor de página de aterrissagem quando o valor estiver na posição LIGADO. &quot;ON&quot; se não fornecido.

Exemplo básico:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Exemplo com todos os atributos:

Este exemplo mostra um caso de uso comum em que uma variável booleana controla a visibilidade de um elemento css definindo o valor da propriedade de exibição css como &quot;bloquear&quot; ou &quot;nenhum&quot; para mostrar/ocultar um elemento por id com CSS. O editor de página de aterrissagem usará o nome de exibição Mostrar/Ocultar em vez de DESATIVAR/ATIVAR.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Os tokens de programa (my.token) também podem ser usados em qualquer lugar nas páginas de aterrissagem guiadas ou de formato livre.
