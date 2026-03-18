---
unique-page-id: 11371040
description: Saiba mais sobre a sintaxe do modelo de email no Editor de email 2.0. Use a sintaxe correta para módulos e seções editáveis em modelos.
title: Sintaxe do modelo de email
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '2462'
ht-degree: 99%

---

# Sintaxe do modelo de email {#email-template-syntax}

Na nova experiência de Email 2.0 do Marketo, os modelos de email são compostos de qualquer combinação de elementos, variáveis, módulos ou containers. Cada uma é definida adicionando uma sintaxe específica do Marketo ao HTML. Os modelos de email antigos (v1.0) são compatíveis com o Editor de email 2.0, no entanto, eles não incluirão todos os recursos do novo editor.

A sintaxe de email do Marketo só funciona em modelos e emails individuais. Ela **não** funciona se estiver incorporada em trechos ou tokens Rich Text.

>[!NOTE]
>
>O suporte do Marketo não está configurado para auxiliar com CSS/HTML. Se você não estiver familiarizado com CSS/HTML, consulte seu desenvolvedor.

>[!CAUTION]
>
>Os valores de classe que contêm a sintaxe do Marketo (ou seja, mktoModule, mktoContainer, mktoText) diferenciam maiúsculas de minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não fazem essa diferenciação.

## Elementos {#elements}

Os elementos são regiões de conteúdo definidas como editáveis no modelo de email. A experiência de edição de um elemento é exclusiva a seu tipo e oferece uma maneira simples de trabalhar com conteúdo. Os possíveis elementos que podem ser incluídos em um modelo de email são:

* Rich text
* Imagens
* Trechos
* Vídeos

## Rich text {#rich-text}

Se você definir uma região como Rich text, os usuários poderão editar seu conteúdo [usando o Editor de Rich Text do Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Há duas maneiras de definir um elemento de Rich Text dentro de um modelo de email: mktEditable e mktoText. Lembre-se, um elemento Rich Text sempre pode ser convertido em um trecho no editor de email.

### Opção 1: mktEditable {#option-mkteditable}

Como o Editor de email 2.0 é compatível com versões anteriores, alguns modelos de email antigos podem especificar elementos Rich Text adicionando class=&quot;mktEditable&quot; em qualquer elemento do HTML. Ele ainda é compatível, e a ID do elemento é o que será usado como o nome de exibição dentro do editor de email.

Atributos obrigatórios

* **classe**: &quot;mktEditable&quot;.
* **id**: string de ID. Contém apenas letras, números, traço “-” e sublinhado “_”. Espaços não são permitidos. Precisa ser exclusivo.

Atributos opcionais

* **mktoName** : string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktEditable&quot; será usado como valor padrão para o elemento Rich Text.

Exemplo:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Opção 2: mktoText {#option-mktotext}

É recomendável especificar elementos Rich Text usando a sintaxe class=&quot;mktoText&quot;. Isso garante que sempre haja um nome de exibição apropriado para o elemento.

Atributos obrigatórios

* **classe**: &quot;mktoText&quot;
* **id**: string da ID. Contém apenas letras, números, traço “-” e sublinhado “_”. Espaços não são permitidos. Precisa ser exclusivo.
* **mktoName** : string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktoText&quot; será usado como valor padrão para o elemento Rich Text.

Exemplo:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Imagens {#images}

Você tem duas opções para definir elementos de imagem editáveis. Você pode usar um `<div>`, que especifica um container no qual o `<img>` será inserido, ou uma tag de `<img>`. Caso queira que o usuário final simplesmente escolha uma imagem que retornará o URL da imagem (em vez do DOM), consulte “variáveis de imagem” na seção abaixo. As duas opções a seguir inserirão um elemento `<img>` em HTML.

### Opção 1: usar um `<div>` {#option-use-a-div}

Atributos obrigatórios

* **classe:** “mktoImg”.
* **id:** string de ID. Contém apenas letras, números, traço “-” e sublinhado “_”. Espaços não são permitidos. Precisa ser exclusivo.
* **mktoName :** string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** string. O valor aqui será adicionado ao atributo de classe do elemento `<img>` dentro da div.
* **mktoImgSrc:** para ser usado como valor padrão para a imagem colocada nesta div. Se for omitido, um espaço reservado será usado.
* **mktoImgLink:** indique que o `<img>` deve estar rodeado por uma tag de `<a>` com este URL de destino. O usuário pode alterar isso no editor de email.
* **mktoImgLinkTarget:** indique que a tag de `<a>` do atributo mktoImgLink deve usar este destino. Não surte efeito se mktoImgLink também não for usado.
* **mktoImgWidth:** usado como a largura no `<img>` delimitado.
* **mktoImgHeight:** usado como a altura no `<img>` delimitado.
* **mktoLockImgSize:** usado para desbloquear a propriedade de altura e largura do elemento `<img>`, para que o usuário final possa modificar (o padrão é verdadeiro, se omitido).
* **mktoLockImgStyle:** usado para bloquear a propriedade de estilo do elemento `<img>` (o padrão é falso).

Valor padrão (opcional)

**`<img>`**: para ser usado como o elemento `<img>` no qual a imagem será colocada. É útil quando você quer adicionar um estilo em linha à imagem. Lembre-se de incluir tags de `<a> </a>` ao redor. Assim, se o usuário adicionar um link, o seu estilo não será removido.

Exemplo:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Opção 2: usar um \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Esta opção não permite que os usuários finais adicionem um link à imagem. Se isso for importante para o seu modelo, use a Opção 1.

Atributos obrigatórios

* **classe:** “mktoImg”.
* **id:** string de ID. Contém apenas letras, números, traço “-” e sublinhado “_”. Espaços não são permitidos. Precisa ser exclusivo.
* **mktoName:** string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.  Valor padrão (opcional)
* **src:** para ser usado como valor padrão da imagem. Se for omitido, um espaço reservado será usado.
* **mktoLockImgSize:** usado para desbloquear a propriedade de altura e largura do elemento `<img>`, para que o usuário final possa modificar (o padrão é verdadeiro, se omitido).
* **mktoLockImgStyle:** usado para bloquear a propriedade de estilo do elemento `<img>` (o padrão é falso).

Exemplo:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Trechos {#snippets}

Se você definir uma região como um trecho, os usuários finais poderão escolher qual [Trecho](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)aprovado querem inserir nesta região. Embora os elementos de Rich Text possam ser convertidos em trechos a partir do editor de email, ao se definir uma região especificamente como um trecho, ela não pode ser convertida em Rich Text. Você pode especificar uma região de trecho, usando um `<div>` com classe=“mktoSnippet”

Atributos obrigatórios

* **id:** string de ID. Contém apenas letras, números, traço “-” e sublinhado “_”. Espaços não são permitidos. Precisa ser exclusivo.
* **mktoName:** string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão (opcional)

**mktoDefaultSnippetId**: a ID numérica do trecho do Marketo que deve aparecer por padrão (funcionará somente se um trecho com essa ID existir e for aprovado nesse espaço de trabalho).

Exemplo:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Vídeo {#video}

Se você definir uma região como um vídeo, os usuários finais poderão inserir um URL do YouTube ou do Vimeo para ser exibido como uma imagem em miniatura (com o botão de reproduzir) dentro do email. Você pode especificar uma região de vídeo, usando um `<div>` com classe=“mktoVideo”

Atributos obrigatórios

* **id:** string de ID. Contém apenas letras, números, traço “-” e sublinhado “_”. Espaços não são permitidos. Precisa ser exclusivo.
* **mktoName:** string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** string. O valor aqui será adicionado ao atributo de classe da miniatura do vídeo `<img>` dentro da div.

Exemplo:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variáveis {#variables}

As variáveis são como tokens. Primeiro, você as define na seção `<head>` do seu modelo de email, usando as tags de `<meta>`, e depois as usa quantas vezes quiser em todo o modelo. Como são definidas no modelo, o usuário final pode modificar seus valores de acordo com suas regras. Observe que você pode definir uma variável como local ou global no escopo. Se você usar uma variável em um “Módulo” (confira abaixo) e um usuário final duplicar esse módulo, as variáveis locais terão valores independentes, enquanto as variáveis globais se aplicarão a ambos os módulos.

## String {#string}

Se você especificar uma variável como string, o usuário final poderá inserir um texto em uma caixa de texto no editor de email. Para especificar uma variável de string, use `<meta>` com classe=“mktoString”

Atributos obrigatórios

* **id:** como você referencia a variável no seu modelo de email.
* **mktoName:** string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **allowHTML:** booleano. Controla se o valor da variável tem escape de HTML. O padrão é falso, se omitido.
* **padrão**: valor padrão da string. Em branco, se omitido.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Exemplo de uso:

`${textHeader}`

## Lista {#list}

Se você especificar uma variável como uma lista, o usuário final poderá escolher a partir de um conjunto de valores definidos no editor de email. Para especificar uma variável de lista, use `<meta>` com classe=“mktoList”

Atributos obrigatórios

* **id**: como você referencia a variável no seu modelo de email.
* **mktoName:** string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **valores:** lista de valores separados por vírgulas. Precisa ter pelo menos uma string.

Atributos opcionais

* **padrão:** valor padrão da lista suspensa de seleção. Se omitido, o primeiro valor do atributo “valores” será usado.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Exemplo de uso:

`${textFontFamily}`

## Número {#number}

Se você especificar uma variável como um número, o usuário final poderá inserir um número no editor de email. Para especificar uma variável de número, use `<meta>` com classe=“mktoNumber”

Atributos obrigatórios

* **id**: como você referencia a variável no seu modelo de email.
* **mktoName**: string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **padrão:** valor numérico padrão da variável.

Atributos opcionais

* **mín:** valor mínimo aceito.
* **máx:** valor máximo aceito.
* **unidades:** unidades a serem anexadas ao valor numérico (por exemplo: px, pt, em, etc.) quando exibidas no editor de email, bem como no código resultante.
* **Incremento:** em quantas unidades a variável de número deve aumentar/diminuir (0,1, 1, 10 etc.). Se omitido, o padrão será 1.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

Exemplo de uso:

`${textFontSize}`

## Cor {#color}

Se você especificar uma variável como uma cor, o usuário final poderá inserir um valor de cor hexadecimal ou escolher uma cor no seletor de cores do editor de email. Para especificar uma variável de cor, use `<meta>` com classe=“mktoColor”

Atributos obrigatórios

* **id**: como você referencia a variável no seu modelo de email.
* **mktoName**: string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** valor padrão da cor. Código de cor hexadecimal de seis dígitos. Exemplo: #ffffff.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Exemplo de uso:

`${textColor}`

## Booleano {#boolean}

Se você especificar uma variável como booleana, o usuário final poderá ativar/desativar a opção no editor de email. Você especifica uma variável booleana usando `<meta>` com class=&quot;mktoBoolean&quot;

Atributos obrigatórios

* **id**: como você referencia a variável no seu modelo de email.
* **mktoName**: string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** valor booleano que determina o estado padrão do botão de alternância. Falso, se omitido.
* **false_value:** valor a ser inserido quando o botão de alternância estiver na posição DESLIGADO. Falso, se omitido.
* **true_value:** valor a ser inserido quando o botão de alternância estiver na posição LIGADO. Verdadeiro, se omitido.
* **false_value_name:** interface mostrada no botão de alternância quando na posição DESLIGADO. Falso, se omitido.
* **true_value_name:** interface mostrada no botão de alternância quando na posição LIGADO. Verdadeiro, se omitido.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Exemplo de uso:

`${showFooter}`

## Bloco de HTML {#html-block}

Se você especificar uma variável como um Bloco de HTML, o usuário final poderá inserir o HTML literal no editor de email. Você especifica uma variável de bloco HTML usando `<meta>` com class=&quot;mktoHTML&quot;

Atributos obrigatórios

* **id**: como você referencia a variável no seu modelo de email.
* **mktoName**: string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** valor codificado de HTML para servir como conteúdo padrão do bloco.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Exemplo de uso:

`${trackingPixel}`

## Variável de imagem {#image-variable}

Se você especificar uma variável como uma imagem, o usuário final poderá escolher uma imagem no seletor de imagens no editor de email. O URL da imagem selecionada será o valor da variável. Você especifica uma variável de imagem usando `<meta>` com class=&quot;mktoImg&quot;

Atributos obrigatórios

* **id**: como você referencia a variável no seu modelo de email.
* **mktoName**: string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **Padrão:** URL da imagem padrão do elemento.
* **mktoModuleScope**: booleano. Controla se a variável é local (verdadeira) ou global (falsa) quando usada em um módulo. O padrão é falso, se omitido.

Exemplo de declaração:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Exemplo de uso:

`${heroBackgroundImage}`

## Módulos {#modules}

Os módulos são seções de modelos definidas no nível do modelo que serão exibidas para os usuários finais inserirem em seus emails. Como você pré-criou esses módulos, é possível garantir que eles interajam com o restante do conteúdo do email normalmente (de uma maneira totalmente responsiva). Você só pode colocar um módulo em um container.

>[!IMPORTANT]
>
>Quando um email é gerado a partir de um modelo de email que contém componentes definidos do módulo, todas as alterações feitas nos módulos do modelo **não** serão enviadas para esse email.

**Para containers do tipo `<table>`, `<tbody>`, `<thead>` ou `<tfoot>`:**

Especificado usando `<tr>` com class=&quot;mktoModule&quot;

**Para containers do tipo `<td>`:**

Especificado usando `<table>` com class=&quot;mktoModule&quot;

Atributos obrigatórios

* **id**: como você faz referência ao módulo no seu modelo de email.
* **mktoName**: string. Este é o nome de exibição que será mostrado no editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoActive:** determina se este módulo aparece na lista de módulos no editor de email. O padrão é verdadeiro. Se for falso, o módulo não poderá ser adicionado por um usuário final a um email.
* **mktoAddByDefault:** determina se este módulo estará na tela de um novo email que usa o modelo após a criação. O padrão é verdadeiro (se mktoActive for falso, esse valor será ignorado).

>[!NOTE]
>
>Os valores de classe que contêm a sintaxe do Marketo (ou seja, mktoModule, mktoContainer, mktoText) diferenciam maiúsculas de minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não fazem essa diferenciação.

## Containers {#containers}

Um container contém módulos e define onde eles podem ser colocados. Quando os usuários finais estão reorganizando e inserindo módulos em seus emails, o container controla para onde eles podem ir.

**Especificado usando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` ou `<td>` com class=&quot;mktoContainer&quot;**

Atributos obrigatórios

**id**: como você referencia o módulo no seu modelo de email.

>[!CAUTION]
>
>Os containers só podem conter módulos. Se houver algo mais presente, o container será considerado inválido. Somente um container é permitido por modelo.
