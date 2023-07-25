---
unique-page-id: 11371040
description: Sintaxe de modelo de email - Documentação do Marketo - Documentação do produto
title: Sintaxe do modelo de email
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 1%

---

# Sintaxe do modelo de email {#email-template-syntax}

Na nova experiência do Email 2.0 da Marketo, os modelos de email são compostos de qualquer combinação de elementos, variáveis, módulos ou contêineres. Cada um é definido adicionando uma sintaxe específica do Marketo ao seu HTML. Os modelos de email antigos (v1.0) são suportados no Editor de email 2.0; no entanto, eles não incluirão todos os recursos do novo Editor.

A sintaxe de email do Marketo só funciona em modelos e emails individuais; ela funciona **não** funcionam se estiverem incorporados em trechos ou tokens Rich Text.

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
* Blocos de conteúdo
* Vídeos

## Texto formatado {#rich-text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [uso do editor de rich text do Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Há duas maneiras de definir um elemento de Rich Text dentro de um modelo de email: mktEditable e mktoText. Lembre-se, um elemento Rich Text sempre pode ser convertido em um trecho no editor de email.

### Opção 1 - mktEditable {#option-mkteditable}

Como o Editor de email 2.0 é compatível com versões anteriores, alguns modelos de email antigos podem especificar elementos rich text adicionando class=&quot;mktEditable&quot; em qualquer elemento HTML. Isso ainda é compatível, e a ID do elemento é o que será usado como o nome de exibição dentro do editor de email.

Atributos obrigatórios

* **classe**: &quot;mktEditable&quot;.
* **id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.

Atributos opcionais

* **mktoName** : String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktEditable&quot; será usado como valor padrão para o elemento Rich Text.

Exemplo:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opção 2 - mktoText {#option-mktotext}

É recomendável especificar elementos Rich Text usando a sintaxe class=&quot;mktoText&quot;. Isso garante que sempre haja um nome de exibição apropriado para o elemento.

Atributos obrigatórios

* **classe**: &quot;mktoText&quot;
* **id**: cadeia de caracteres de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName** : String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktoText&quot; será usado como valor padrão para o elemento Rich Text.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Imagens {#images}

Você tem duas opções para definir elementos de Imagem editáveis. Você pode usar um `<div>`, que especifica um contêiner que `<img>` será inserida no, ou em um `<img>` tag. Se você pretende que o usuário final simplesmente escolha uma imagem que retornará o URL da imagem (em vez do DOM), consulte &quot;variáveis de imagem&quot; na seção abaixo. As duas opções a seguir inserirão um HTML `<img>` elemento.

### Opção 1 - Usar um `<div>` {#option-use-a-div}

Atributos obrigatórios

* **classe:** &quot;mktoImg&quot;.
* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName:** String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** String. O valor aqui será adicionado ao atributo de classe de `<img>` elemento dentro da div.
* **mktoImgSrc:** Para ser usado como valor padrão para a imagem colocada dentro dessa div. Um espaço reservado será usado se isso for omitido.
* **mktoImgLink:** Indique que a variável `<img>` deve estar rodeada por uma `<a>` com este URL de destino. O usuário pode alterar isso no Editor de email.
* **mktoImgLinkTarget:** Indique que a variável `<a>` a tag do atributo mktoImgLink deve usar esse destino. Não tem efeito se mktoImgLink também não for usado.
* **mktoImgWidth:** Usado como a largura no delimitado `<img>`.
* **mktoImgHeight:** Usado como a altura no `<img>`.
* **mktoLockImgSize:** Usado para desbloquear o `<img>` a propriedade height e width do elemento para que o usuário final possa modificar (o padrão é verdadeiro se omitido).
* **mktoLockImgStyle:** Usado para bloquear o `<img>` propriedade style do elemento (o padrão é false).

Valor padrão (opcional)

**`<img>`**: Para ser usado como o `<img>` elemento no qual a imagem será colocada. Útil se você quiser adicionar um estilo em linha à imagem. Lembre-se de incluir `<a> </a>` tags, portanto, se o usuário adicionar um link, seu estilo não será removido!

Exemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opção 2 - Usar um \&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Essa opção não permite que os usuários finais adicionem um link a sua imagem. Use a Opção 1 se isso for importante para o seu modelo.

Atributos obrigatórios

* **classe:** &quot;mktoImg&quot;.
* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName:** String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.  Valor padrão (opcional)
* **src:** Para ser usado como o valor padrão da imagem. Um espaço reservado será usado se isso for omitido.
* **mktoLockImgSize:** Usado para desbloquear o `<img>` a propriedade height e width do elemento para que o usuário final possa modificar (o padrão é verdadeiro se omitido).
* **mktoLockImgStyle:** Usado para bloquear o `<img>` propriedade style do elemento (o padrão é false).

Exemplo:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Blocos de conteúdo {#snippets}

Se você definir uma região como um trecho, os usuários finais poderão escolher qual região aprovada [Trecho](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)eles gostariam de inserir nesta região. Embora os elementos Rich Text possam ser convertidos em trechos a partir do editor de email, ao definir uma região especificamente como um trecho, ela não pode ser convertida em Rich Text. Você pode especificar uma região de trecho usando uma `<div>` com class=&quot;mktoSnippet&quot;

Atributos obrigatórios

* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName:** String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão (opcional)

**mktoDefaultSnippetId**: a ID numérica do trecho do Marketo que deve aparecer por padrão (funcionará somente se um trecho com essa ID existir e for aprovado nesse espaço de trabalho).

Exemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vídeo {#video}

Se você definir uma região como um Vídeo, os usuários finais poderão inserir um URL do YouTube ou do Vimeo que será exibido como uma imagem em miniatura (com o botão &quot;reproduzir&quot;) dentro do email. Você pode especificar uma região de Vídeo usando um `<div>` com class=&quot;mktoVideo&quot;

Atributos obrigatórios

* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser única.
* **mktoName:** String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** String. O valor aqui será adicionado ao atributo de classe da miniatura do vídeo `<img>` dentro da div.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variáveis {#variables}

As variáveis são como tokens. Primeiro, você os define dentro da variável `<head>` do seu modelo de email usando `<meta>` tags, em seguida, use-as quantas vezes desejar em seu modelo. Como são definidos no modelo, o usuário final poderá modificar seus valores de acordo com suas regras. Observe que você pode definir uma variável como local ou global no escopo. Se você usar uma variável em um &quot;Módulo&quot; (veja abaixo) e um usuário final duplicar esse módulo, as variáveis locais terão valores independentes, enquanto as variáveis globais se aplicarão a ambos os módulos.

## Sequência de caracteres {#string}

Se você especificar uma variável como String, o usuário final poderá inserir texto em uma caixa de texto no editor de email. Especifique uma variável de string usando `<meta>` com class=&quot;mktoString&quot;

Atributos obrigatórios

* **id:** Como você faz referência à variável no seu modelo de email.
* **mktoName:** String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **allowHTML:** Booleano. Controla se o valor da variável tem escape de HTML. O padrão é Falso, caso seja omitido.
* **padrão**: Valor padrão para a cadeia de caracteres. Em branco, se omitido.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Lista {#list}

Se você especificar uma variável como uma Lista, o usuário final poderá escolher a partir de um conjunto de valores definidos no editor de email. Você especifica uma variável de lista usando `<meta>` com class=&quot;mktoList&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName:** String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **valores:** Lista de valores separados por vírgulas. Deve ter pelo menos uma sequência de caracteres.

Atributos opcionais

* **padrão:** Valor padrão da lista suspensa de seleção. Se omitido, o primeiro valor do atributo &quot;values&quot; será usado.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Número {#number}

Se você especificar uma variável como um Número, o usuário final poderá inserir um número no editor de email. Especifique uma variável Number usando `<meta>` com class=&quot;mktoNumber&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **padrão:** Valor numérico padrão para a variável.

Atributos opcionais

* **min.:** Valor mínimo aceito.
* **máx:** Valor máximo aceito.
* **unidades:** Unidades a serem acrescentadas ao valor numérico (por exemplo: px, pt, em, etc.) quando exibido no Editor de email, bem como no código resultante.
* **etapa:** Quantas unidades a variável de número deve aumentar/diminuir em (0,1, 1, 10, etc.). Se omitido, o padrão será 1.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Cor {#color}

Se você especificar uma variável como uma Cor, o usuário final poderá inserir um valor de cor hexadecimal ou escolher uma cor no seletor de cores do editor de email. Especifique uma variável Cor usando `<meta>` com class=&quot;mktoColor&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor padrão da cor. Código de cor hexadecimal de 6 dígitos. Exemplo: #ffffff.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Se você especificar uma variável como Booleana, o usuário final poderá ativar/desativar a opção no editor de email. Você especifica uma variável booleana usando `<meta>` com class=&quot;mktoBoolean&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor booleano que determina o estado padrão da opção de alternância. Falso, se omitido.
* **valor_falso:** Valor a ser inserido quando o botão de alternância estiver na posição DESLIGADO. Falso, se omitido.
* **valor_verdadeiro:** Valor a ser inserido quando o botão de alternância estiver na posição LIGADO. True se omitido.
* **nome_do_valor_falso:** Interface mostrada no botão de alternância quando estiver na posição DESLIGADO. Falso, se omitido.
* **nome_valor_verdadeiro:** Interface mostrada no botão de alternância quando na posição LIGADO. True se omitido.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloco HTML {#html-block}

Se você especificar uma variável como um Bloco de HTML, o usuário final poderá inserir o HTML textual no editor de email. Você especifica uma variável de HTML Block usando `<meta>` com class=&quot;mktoHTML&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor codificado em HTML para servir como conteúdo padrão do bloco.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variável de imagem {#image-variable}

Se você especificar uma variável como uma Imagem, o usuário final poderá escolher uma imagem no seletor de imagens no editor de email. A URL da imagem selecionada será o valor da variável. Especifique uma variável de imagem usando `<meta>` com class=&quot;mktoImg&quot;

Atributos obrigatórios

* **id**: como você faz referência à variável no seu modelo de email.
* **mktoName**: String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** URL da imagem padrão do elemento.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso, caso seja omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Módulos {#modules}

Os módulos são seções de modelos definidas no nível do modelo que serão exibidas para os usuários finais inserirem em seus emails. Como você pré-criou esses módulos, pode garantir que eles interajam com o restante do conteúdo de email normalmente (de uma maneira totalmente responsiva). Você só pode colocar um módulo em um container.

>[!IMPORTANT]
>
>Quando um email é gerado a partir de um modelo de email que contém os componentes definidos do módulo, todas as alterações feitas nos módulos do modelo serão **não** ser encaminhado para o email.

**Para contêineres do tipo `<table>`, `<tbody>`, `<thead>`ou `<tfoot>`:**

Especificado usando `<tr>` com class=&quot;mktoModule&quot;

**Para contêineres do tipo `<td>`:**

Especificado usando `<table>` com class=&quot;mktoModule&quot;

Atributos obrigatórios

* **id**: como você faz referência ao módulo no seu modelo de email.
* **mktoName**: String. Este é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoActive:** Determina se este módulo aparece na lista de módulos no editor de email. O padrão é true. Se false, o módulo não poderá ser adicionado por um usuário final a um email.
* **mktoAddByDefault:** Determina se esse módulo estará na tela de um novo email que usa esse template após a criação. O padrão é true (se mktoActive for false, esse valor será ignorado).

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
