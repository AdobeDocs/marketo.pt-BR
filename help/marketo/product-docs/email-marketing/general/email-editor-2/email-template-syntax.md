---
unique-page-id: 11371040
description: Sintaxe de modelo de email - Documentação do Marketo - Documentação do produto
title: Sintaxe do modelo de email
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 1%

---

# Sintaxe do modelo de email {#email-template-syntax}

Na nova experiência do Email 2.0 da Marketo, os modelos de email são compostos de qualquer combinação de elementos, variáveis, módulos ou contêineres. Cada um é definido adicionando uma sintaxe específica do Marketo ao seu HTML. Os modelos de email antigos (v1.0) são suportados no Editor de email 2.0; no entanto, eles não incluirão todos os recursos do novo Editor.

A sintaxe de email do Marketo só funciona em modelos e emails individuais; ela **não** funciona se estiver incorporada em trechos ou tokens Rich Text.

>[!NOTE]
>
>O Suporte da Marketo não está configurado para auxiliar com CSS/HTML. Se você não estiver familiarizado com CSS/HTML, consulte o desenvolvedor.

>[!CAUTION]
>
>Os valores de classe que contêm a sintaxe do Marketo (ou seja, mktoModule, mktoContainer, mktoText) fazem distinção entre maiúsculas e minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não são.

## Elementos {#elements}

Os elementos são regiões de conteúdo definidas como editáveis no modelo de email. A experiência de edição de um elemento é exclusiva a seu tipo e oferece uma maneira simples de trabalhar com conteúdo. Os possíveis elementos que podem ser incluídos em um template de email são:

* Texto formatado
* Imagens
* Bl. conteúdo
* Vídeos

## Texto formatado {#rich-text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [usando o Editor de Rich Text do Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Há duas maneiras de definir um elemento de Rich Text dentro de um modelo de email: mktEditable e mktoText. Lembre-se, um elemento Rich Text sempre pode ser convertido em um trecho no editor de email.

### Opção 1 - mktEditable {#option-mkteditable}

Como o Editor de email 2.0 é compatível com versões anteriores, alguns modelos de email antigos podem especificar elementos rich text adicionando class=&quot;mktEditable&quot; em qualquer elemento HTML. Isso ainda é compatível, e a ID do elemento é o que será usado como o nome de exibição dentro do editor de email.

Atributos obrigatórios

* **classe**: &quot;mktEditable&quot;.
* **id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.

Atributos opcionais

* **mktoName** : cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktEditable&quot; será usado como valor padrão para o elemento Rich Text.

Exemplo:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Opção 2 - mktoText {#option-mktotext}

É recomendável especificar elementos Rich Text usando a sintaxe class=&quot;mktoText&quot;. Isso garante que sempre haja um nome de exibição apropriado para o elemento.

Atributos obrigatórios

* **classe**: &quot;mktoText&quot;
* **id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName** : cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktoText&quot; será usado como valor padrão para o elemento Rich Text.

Exemplo:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Imagens {#images}

Você tem duas opções para definir elementos de Imagem editáveis. Você pode usar um `<div>`, que especifica um contêiner no qual o `<img>` será inserido, ou uma marca `<img>`. Se você pretende que o usuário final simplesmente escolha uma imagem que retornará o URL da imagem (em vez do DOM), consulte &quot;variáveis de imagem&quot; na seção abaixo. As duas opções a seguir inserirão um elemento HTML `<img>`.

### Opção 1 - Usar um `<div>` {#option-use-a-div}

Atributos obrigatórios

* **classe:** &quot;mktoImg&quot;.
* **id:** cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName :** Cadeia de Caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** Cadeia de Caracteres. O valor aqui será adicionado ao atributo de classe do elemento `<img>` dentro de div.
* **mktoImgSrc:** Para ser usado como valor padrão para a imagem colocada nesta div. Um espaço reservado será usado se isso for omitido.
* **mktoImgLink:** Indique que `<img>` deve estar rodeado por uma marca `<a>` com esta URL de destino. O usuário pode alterar isso no Editor de email.
* **mktoImgLinkTarget:** Indique que a marca `<a>` do atributo mktoImgLink deve usar este destino. Não tem efeito se mktoImgLink também não for usado.
* **mktoImgWidth:** Usado como a largura no `<img>` delimitado.
* **mktoImgHeight:** Usado como a altura no `<img>` delimitado.
* **mktoLockImgSize:** usado para desbloquear a propriedade de altura e largura do elemento `<img>` para que o usuário final possa modificar (o padrão é verdadeiro, se omitido).
* **mktoLockImgStyle:** usado para bloquear a propriedade style do elemento `<img>` (o padrão é falso).

Valor padrão (opcional)

**`<img>`**: Para ser usado como o elemento `<img>` no qual a imagem será colocada. Útil se você quiser adicionar um estilo em linha à imagem. Lembre-se de incluir `<a> </a>` tags ao redor, portanto, se o usuário adicionar um link, seu estilo não será removido!

Exemplo:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Opção 2 - Usar um \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Essa opção não permite que os usuários finais adicionem um link a sua imagem. Use a Opção 1 se isso for importante para o seu modelo.

Atributos obrigatórios

* **classe:** &quot;mktoImg&quot;.
* **id:** cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* Cadeia de Caracteres **mktoName:**. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.  Valor padrão (opcional)
* **src:** Para ser usado como valor padrão para a imagem. Um espaço reservado será usado se isso for omitido.
* **mktoLockImgSize:** usado para desbloquear a propriedade de altura e largura do elemento `<img>` para que o usuário final possa modificar (o padrão é verdadeiro, se omitido).
* **mktoLockImgStyle:** usado para bloquear a propriedade style do elemento `<img>` (o padrão é falso).

Exemplo:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Bl. conteúdo {#snippets}

Se você definir uma região como um Trecho, os usuários finais poderão escolher qual [Trecho](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)aprovado gostaria de inserir nessa região. Embora os elementos Rich Text possam ser convertidos em trechos a partir do editor de email, ao definir uma região especificamente como um trecho, ela não pode ser convertida em Rich Text. Você pode especificar uma região de trecho usando um `<div>` com class=&quot;mktoSnippet&quot;

Atributos obrigatórios

* **id:** cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* Cadeia de Caracteres **mktoName:**. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão (opcional)

**mktoDefaultSnippetId**: a ID numérica do Trecho do Marketo que deve aparecer por padrão (funcionará somente se um Trecho com essa ID existir e for aprovado nesse espaço de trabalho).

Exemplo:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Vídeo {#video}

Se você definir uma região como um Vídeo, os usuários finais poderão inserir um URL do YouTube ou do Vimeo que será exibido como uma imagem em miniatura (com o botão &quot;reproduzir&quot;) dentro do email. Você pode especificar uma região de Vídeo usando um `<div>` com class=&quot;mktoVideo&quot;

Atributos obrigatórios

* **id:** cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* Cadeia de Caracteres **mktoName:**. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** Cadeia de Caracteres. O valor aqui será adicionado ao atributo de classe da miniatura do vídeo `<img>` dentro de div.

Exemplo:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variáveis {#variables}

As variáveis são como tokens. Primeiro, você os define na seção `<head>` do seu modelo de email usando as tags `<meta>` e depois os usa quantas vezes quiser em todo o modelo. Como são definidos no template, o usuário final poderá modificar seus valores de acordo com suas regras. Observe que você pode definir uma variável como local ou global no escopo. Se você usar uma variável em um &quot;Módulo&quot; (veja abaixo) e um usuário final duplicar esse módulo, as variáveis locais terão valores independentes, enquanto as variáveis globais se aplicarão a ambos os módulos.

## String {#string}

Se você especificar uma variável como String, o usuário final poderá inserir texto em uma caixa de texto no editor de email. Você especifica uma variável String usando `<meta>` com class=&quot;mktoString&quot;

Atributos obrigatórios

* **id:** como você faz referência à variável em seu modelo de email.
* Cadeia de Caracteres **mktoName:**. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **allowHTML:** Booleano. Controla se o valor da variável tem escape de HTML. O padrão é Falso, caso seja omitido.
* **padrão**: valor padrão para a cadeia de caracteres. Em branco, se omitido.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Exemplo de uso:

`${textHeader}`

## Lista {#list}

Se você especificar uma variável como uma Lista, o usuário final poderá escolher a partir de um conjunto de valores definidos no editor de email. Você especifica uma variável de lista usando `<meta>` com class=&quot;mktoList&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* Cadeia de Caracteres **mktoName:**. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **Valores:** Lista de valores separados por vírgulas. Deve ter pelo menos uma sequência de caracteres.

Atributos opcionais

* **padrão:** Valor padrão da lista suspensa de seleção. Se omitido, o primeiro valor do atributo &quot;values&quot; será usado.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Exemplo de uso:

`${textFontFamily}`

## Número {#number}

Se você especificar uma variável como um Número, o usuário final poderá inserir um número no editor de email. Você especifica uma variável Number usando `<meta>` com class=&quot;mktoNumber&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **padrão:** Valor numérico padrão para a variável.

Atributos opcionais

* **min:** Valor mínimo aceito.
* **max:** Valor máximo aceito.
* **unidades:** Unidades a serem anexadas ao valor numérico (por exemplo: px, pt, em, etc.) quando exibidas no Editor de email, bem como no código resultante.
* **etapa:** Quantas unidades a variável de número deve aumentar/diminuir (0,1, 1, 10, etc.). Se omitido, o padrão será 1.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> `

Exemplo de uso:

`${textFontSize}`

## Cor {#color}

Se você especificar uma variável como uma Cor, o usuário final poderá inserir um valor de cor hexadecimal ou escolher uma cor no seletor de cores do editor de email. Você especifica uma variável Color usando `<meta>` com class=&quot;mktoColor&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor padrão da cor. Código de cor hexadecimal de 6 dígitos. Exemplo: #ffffff.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Exemplo de uso:

`${textColor}`

## Booleano {#boolean}

Se você especificar uma variável como Booleana, o usuário final poderá ativar/desativar a opção no editor de email. Você especifica uma variável booleana usando `<meta>` com class=&quot;mktoBoolean&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** valor booleano determinando o estado padrão da opção de alternância. Falso, se omitido.
* **false_value:** Valor a ser inserido quando o botão de alternância estiver na posição OFF. Falso, se omitido.
* **true_value:** Valor a ser inserido quando a alternância estiver na posição LIGADA. True se omitido.
* **false_value_name:** interface mostrada no botão de alternância quando na posição OFF. Falso, se omitido.
* **true_value_name:** IU mostrada na alternância quando na posição LIGADO. True se omitido.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Exemplo de uso:

`${showFooter}`

## Bloco HTML {#html-block}

Se você especificar uma variável como um Bloco de HTML, o usuário final poderá inserir o HTML textual no editor de email. Você especifica uma variável de HTML Block usando `<meta>` com class=&quot;mktoHTML&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** valor codificado em HTML para servir como conteúdo padrão do bloco.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Exemplo de uso:

`${trackingPixel}`

## Variável de imagem {#image-variable}

Se você especificar uma variável como uma Imagem, o usuário final poderá escolher uma imagem no seletor de imagens no editor de email. A URL da imagem selecionada será o valor da variável. Você especifica uma variável de imagem usando `<meta>` com class=&quot;mktoImg&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **Padrão:** URL da imagem padrão do elemento.
* **mktoModuleScope**: booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Exemplo de uso:

`${heroBackgroundImage}`

## Módulos {#modules}

Os módulos são seções de modelos definidas no nível do modelo que serão exibidas para os usuários finais inserirem em seus emails. Como você pré-criou esses módulos, pode garantir que eles interajam com o restante do conteúdo de email normalmente (de uma maneira totalmente responsiva). Você só pode colocar um módulo em um container.

>[!IMPORTANT]
>
>Quando um email é gerado a partir de um modelo de email que contém componentes definidos do módulo, todas as alterações feitas nos módulos do modelo **não** serão enviadas para esse email.

**Para contêineres do tipo `<table>`, `<tbody>`, `<thead>` ou `<tfoot>`:**

Especificado usando `<tr>` com class=&quot;mktoModule&quot;

**Para contêineres do tipo `<td>`:**

Especificado usando `<table>` com class=&quot;mktoModule&quot;

Atributos obrigatórios

* **id**: como você faz referência ao módulo no seu modelo de email.
* **mktoName**: cadeia de caracteres. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoActive:** determina se este módulo aparece na lista de módulos no editor de email. O padrão é true. Se false, o módulo não poderá ser adicionado por um usuário final a um email.
* **mktoAddByDefault:** Determina se este módulo estará na tela de um novo email que usa o modelo após a criação. O padrão é true (se mktoActive for false, esse valor será ignorado).

>[!NOTE]
>
>Os valores de classe que contêm a sintaxe do Marketo (ou seja, mktoModule, mktoContainer, mktoText) fazem distinção entre maiúsculas e minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não são.

## Contêineres {#containers}

Um container contém Módulos e define onde eles podem ser colocados. Quando os usuários finais estão reorganizando e inserindo módulos em seus emails, o container controla para onde eles podem ir.

**Especificado usando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` ou `<td>` com class=&quot;mktoContainer&quot;**

Atributos obrigatórios

**id**: como você faz referência ao módulo no seu modelo de email.

>[!CAUTION]
>
>Os contêineres só podem conter módulos. Se houver algo mais presente, o contêiner é considerado inválido. Somente um contêiner é permitido por modelo.
