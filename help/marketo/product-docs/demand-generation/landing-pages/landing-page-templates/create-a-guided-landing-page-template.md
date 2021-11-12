---
unique-page-id: 7515401
description: Criar um modelo de página de aterrissagem guiada - Documentos do Marketo - Documentação do produto
title: Criar um modelo de página de aterrissagem guiada
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
source-git-commit: 115b6e97978778a1d1e13478adf6fee625aa5257
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 2%

---

# Criar um modelo de página de aterrissagem guiada {#create-a-guided-landing-page-template}

Os modelos de página de aterrissagem guiada têm uma sintaxe especial. Use essa sintaxe para especificar o que é personalizável e onde o conteúdo acabará em cada página de aterrissagem criada a partir do modelo. Somente as regiões ou variáveis especificadas como editáveis estarão disponíveis para personalização no editor de páginas de aterrissagem &quot;Guiado&quot;.

>[!TIP]
>
>Use boas convenções de nomenclatura e sua equipe de marketing se apaixonará por você.

Há duas maneiras de declarar que algo em sua página deve ser editável:

* Declarar um objeto como &quot;elemento&quot;. O criador da landing page poderá adicionar imagens, texto ou ativos do Marketo nessas regiões especificadas.
* Declare uma cadeia de caracteres como &quot;variável&quot;. O criador da landing page poderá substituir essa variável por uma string, cor ou estado booleano de uma alavanca true/false.

## Elementos editáveis {#editable-elements}

Os elementos são declarados adicionando um elemento DOM normal ao modelo e, em seguida, decorando o elemento com um nome de classe específico do Marketo.

## Texto {#text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [usando o Editor de Rich Text do Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Atributos obrigatórios:\
**classe**: &quot;mktoText&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
O conteúdo de um elemento com a classe mktoText (se fornecido) será usado como o valor padrão para a região editável.

Exemplo:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Imagem {#image}

Você tem duas opções para definir Elementos de imagem editáveis. Você pode usar um dos `<div>`, que especifica um contêiner no qual a imagem será inserida, ou um `<img>` .

## Opção 1 - Usar um `<div>` {#option-use-a-div}

Atributos obrigatórios:

classe: &quot;mktoImg&quot;\
id: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
mktoName : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
mktoImgClass: Sequência de caracteres. O valor aqui será adicionado ao atributo de classe do `<img>` dentro do div.

Exemplo:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Opção 2 - Usar um `<img>` {#option-use-a-img}

Atributos obrigatórios:\
classe: &quot;mktoImg&quot;\
id: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
mktoName : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
src: URL da string. Isso será usado como o valor padrão da imagem.

Exemplo:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Ao usar a variável `<img>` versão, o HTML renderizado conterá um wrapper div gerado em torno da variável `<img>` . Ele será definido como class .&quot;mktoImg.mktoGen,&quot; e será display:inline-block.

## Formulário {#form}

Exemplo:Atributos obrigatórios:\
**classe**: &quot;mktoForm&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Bloco de conteúdo {#snippet}

Atributos obrigatórios:\
**classe**: &quot;mktoSnippet&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Compartilhar botão {#share-button}

Atributos obrigatórios:\
**classe**: &quot;mktoShareButton&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Vídeo {#video}

>[!NOTE]
>
>Ao usar o elemento de vídeo em uma página de aterrissagem, o Marketo só oferece suporte a vídeos do YouTube. Se você usar outro serviço, recomendamos utilizar uma caixa Rich Text e colar no código incorporado do vídeo.

Atributos obrigatórios:
**classe**: &quot;mktoVideo&quot;
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Pesquisa {#poll}

Atributos obrigatórios:\
**classe**: &quot;mktoPoll&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Indicação {#referral}

Atributos obrigatórios:\
**classe**: &quot;mktoReferral&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Sorteios {#sweepstakes}

Atributos obrigatórios:\
**classe**: &quot;mktoSweepstakes&quot;\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Variáveis editáveis {#editable-variables}

Todos os tipos de variáveis são usados referenciando o valor de seu atributo de id encapsulado dentro de uma sequência de caracteres ${ } . Eles podem ser usados em qualquer lugar no documento, exceto para dentro de outras declarações de variável.

Exemplo:

`${var1}`

**Declaração:**

As variáveis são declaradas como meta tags dentro da variável `<head>` elemento do template. Há três tipos de variáveis disponíveis para uso: Sequência de caracteres, cor e booleano.

## Sequência de caracteres {#string}

Atributos obrigatórios:\
**classe** : &quot;mktoString&quot;,\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
**default**: Valor da string para o atributo. Em branco se nenhum tiver fornecido.\
**allowHtml**: &quot;true&quot; ou &quot;false&quot;. Controla se o valor será impresso sem escape de HTML. O padrão é &quot;false&quot; se não estiver definido.

Exemplo básico:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Exemplo com todos os atributos:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Cor {#color}

Atributos obrigatórios:\
**classe** : &quot;mktoColor&quot;,\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
**default**: Um código de cor de caractere HEX de 7 dígitos. Por exemplo: &quot;#336699&quot;

Exemplo básico:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Exemplo com todos os atributos:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booleano {#boolean}

Atributos obrigatórios:\
**classe** : &quot;mktoBoolean&quot;,\
**id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : Sequência de caracteres. Esse é o nome de exibição que será mostrado no editor de landing page. A prática recomendada é usar um nome descritivo.

Opcional:\
**default**: Sequência booleana. &quot;true&quot; ou &quot;false&quot; controla se o valor começa na posição ON ou OFF. &quot;false&quot; se não fornecido.\
**false_value**: Sequência de caracteres. O valor a ser inserido para a variável quando ela estiver na posição OFF. &quot;false&quot; se não fornecido.\
**true_value**: Sequência de caracteres. O valor a ser inserido para a variável quando ela estiver na posição ATIVADA. &quot;true&quot; se não for fornecido.\
**false_value_name**: Sequência de caracteres. O nome de exibição a ser exibido no editor de landing page quando o valor estiver na posição OFF. &quot;OFF&quot; se não fornecido.\
**true_value_name**: Sequência de caracteres. O nome de exibição a ser exibido no editor de landing page quando o valor estiver na posição ON. &quot;ON&quot; se não for fornecido.

Exemplo básico:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Exemplo com todos os atributos:

Este exemplo mostra um caso de uso comum em que uma variável booleana controla a visibilidade de um elemento css ao definir o valor da propriedade de exibição css como &quot;block&quot; ou &quot;none&quot; para mostrar/ocultar um elemento pela id com CSS. O editor de landing page usará o nome de exibição Mostrar/Ocultar em vez de OFF/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>Os tokens de programa (my.token) também podem ser usados em qualquer lugar das páginas de aterrissagem guiadas ou de forma livre.
