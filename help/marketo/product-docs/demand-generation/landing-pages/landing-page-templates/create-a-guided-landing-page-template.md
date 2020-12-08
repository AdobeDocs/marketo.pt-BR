---
unique-page-id: 7515401
description: Criar um modelo de Landing page guiada - Documentos do Marketing - Documentação do produto
title: Criar um modelo de Landing page guiada
translation-type: tm+mt
source-git-commit: 975e048271dae6a877ae9ff5d39360b159afcc8a
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---


# Criar um modelo de Landing page guiada {#create-a-guided-landing-page-template}

>[!NOTE]
>
>**Mergulho profundo:** Cansado de ler? [Assista a este vídeo](https://youtu.be/3O7e4GdZKsM) interessante com instruções passo a passo.

Os modelos de landing page guiada têm uma sintaxe especial. Use essa sintaxe para especificar o que é personalizável e onde o conteúdo terminará em cada landing page criada a partir do modelo. Somente as regiões ou variáveis especificadas como editáveis estarão disponíveis para personalização no editor de landings page &quot;Guiado&quot;.

>[!TIP]
>
>Use boas convenções de nomenclatura e sua equipe de marketing se apaixonará por você.

Há duas maneiras de declarar que algo em sua página deve ser editável:

* Declarar um objeto como &quot;elemento&quot;. O criador da landing page poderá adicionar imagens, texto ou ativos de marketing nessas regiões especificadas.
* Declarar uma string como uma &quot;variável&quot;. O criador da landing page poderá substituir essa variável por uma string, cor ou estado booleano de uma alavanca true/false.

## Elementos editáveis {#editable-elements}

Os elementos são declarados adicionando um elemento DOM normal ao modelo e, em seguida, decorando o elemento com um nome de classe específico de Marketing.

## Texto {#text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [usando o Editor](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)de Rich Text do Marketo.

Atributos necessários:\
**classe**: &quot;mktoText&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Opcional:\
O conteúdo de um elemento com classe mktoText (se fornecido) será usado como valor padrão para a região editável.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Imagem {#image}

Você tem duas opções para definir elementos de imagem editáveis. Você pode usar um `<div>`, que especifica um container no qual a imagem será inserida, ou uma `<img>` tag.

## Opção 1 - Use uma <div> {#option-use-a-div}

Atributos necessários:

classe: &quot;mktoImg&quot;\
id: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
mktoName : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Opcional:\
mktoImgClass: String. O valor aqui será adicionado ao atributo class do `<img>` elemento dentro de div.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Opção 2 - Use uma `<img>` {#option-use-a-img}

Atributos necessários:\
classe: &quot;mktoImg&quot;\
id: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
mktoName : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Opcional:\
src: URL da cadeia de caracteres. Isso será usado como valor padrão para a imagem.

Exemplo:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Ao usar a `<img>` versão, o HTML renderizado conterá um invólucro div gerado ao redor da `<img>` tag. Ele será definido como classe.&quot;mktoImg.mktoGen&quot; e será display:inline-block.

## Formulário {#form}

Exemplo:Atributos obrigatórios:\
**classe**: &quot;mktoForm&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Trecho {#snippet}

Atributos necessários:\
**classe**: &quot;mktoSnippet&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Botão Compartilhar {#share-button}

Atributos necessários:\
**classe**: &quot;mktoShareButton&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Vídeo {#video}

>[!NOTE]
>
>Ao usar o elemento de vídeo em uma landing page, o Marketo só oferece suporte a vídeos do YouTube. Se você usar outro serviço, recomendamos utilizar uma caixa Rich Text e colar no código incorporado do vídeo.

Atributos necessários:
**classe**: &quot;mktoVideo&quot;**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Pesquisa {#poll}

Atributos necessários:\
**classe**: &quot;mktoPoll&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Consulta {#referral}

Atributos necessários:\
**classe**: &quot;mktoReferral&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Sorteio {#sweepstakes}

Atributos necessários:\
**classe**: &quot;mktoSweepstakes&quot;\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variáveis editáveis {#editable-variables}

Todos os tipos de variáveis são usados referenciando o valor de seu atributo id encapsulado dentro de uma sequência de caracteres ${ }. Eles podem ser usados em qualquer lugar no documento, exceto para dentro de outras declarações variáveis.

Exemplo:

`<pre data-theme="Confluence">${var1}</pre>`

**Declaração:**

As variáveis são declaradas como meta tags dentro do `<head>` elemento do modelo. Há três tipos de variáveis disponíveis para uso: String, Color e Boolean.

## String {#string}

Atributos necessários:\
**classe** : &quot;mktoString&quot;,\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Opcional:\
**padrão**: Valor da string para o atributo. Em branco se não houver nenhum.\
**allowHtml**: &quot;true&quot; ou &quot;false&quot;. Controla se o valor será impresso sem que o HTML seja escapado. O padrão é &quot;false&quot; se não estiver definido.

Exemplo básico:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Exemplo com todos os atributos:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Cor {#color}

Atributos necessários:\
**classe** : &quot;mktoColor&quot;,\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Opcional:\
**padrão**: Um código de cores de caracteres HEX de 7 dígitos. Por exemplo: &quot;#336699&quot;

Exemplo básico:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Exemplo com todos os atributos:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booleano {#boolean}

Atributos necessários:\
**classe** : &quot;mktoBoolean&quot;,\
**id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.\
**mktoName** : String. Esse é o nome de exibição que será mostrado no editor de landings page. A prática recomendada é usar um nome descritivo.

Opcional:\
**padrão**: Sequência booleana. &quot;true&quot; ou &quot;false&quot; controla se o valor start na posição ON ou OFF. &quot;false&quot; se não fornecido.\
**false_value**: String. O valor a ser inserido para a variável quando ela estiver na posição OFF. &quot;false&quot; se não fornecido.\
**true_value**: String. O valor a ser inserido para a variável quando ela estiver na posição ON. &quot;true&quot; se não fornecido.\
**false_value_name**: String. O nome de exibição a ser exibido no editor de landings page quando o valor estiver na posição OFF. &quot;OFF&quot; se não fornecido.\
**true_value_name**: String. O nome de exibição a ser exibido no editor de landings page quando o valor estiver na posição ON. &quot;ON&quot; se não fornecido.

Exemplo básico:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Exemplo com todos os atributos:

Este exemplo mostra um caso de uso comum em que uma variável booleana controla a visibilidade de um elemento css definindo o valor da propriedade de exibição css como &quot;block&quot; ou &quot;none&quot; para mostrar/ocultar um elemento por id com CSS. O editor de landings page usará o nome de exibição Mostrar/Ocultar em vez de OFF/ON.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>Os tokens de programa (my.token) também podem ser usados em qualquer lugar nas landings page Guiadas ou de forma livre.
