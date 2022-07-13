---
unique-page-id: 11371040
description: Sintaxe de modelo de email - Documentos do Marketo - Documentação do produto
title: Sintaxe do modelo de email
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 1%

---

# Sintaxe do modelo de email {#email-template-syntax}

Na nova experiência de email 2.0 do Marketo, os modelos de email são compostos de qualquer combinação de Elementos, Variáveis, Módulos ou Contêineres. Cada uma é definida adicionando uma sintaxe específica do Marketo ao seu HTML. Os modelos de email antigos (v1.0) são compatíveis com o Editor de email 2.0; no entanto, eles não incluirão todos os recursos do novo Editor.

A sintaxe de email do Marketo só funciona em modelos e emails individuais; faz **not** funcionam se incorporados em trechos ou tokens Rich Text.

>[!NOTE]
>
>O Suporte da Marketo não está configurado para auxiliar com CSS/HTML. Se você não estiver familiarizado com CSS/HTML, consulte seu desenvolvedor.

>[!CAUTION]
>
>Valores de classe contendo a sintaxe Marketo (ou seja, mktoModule, mktoContainer, mktoText) fazem distinção entre maiúsculas e minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não são.

## Elementos {#elements}

Os elementos são regiões de conteúdo que você define como editáveis no seu modelo de email. A experiência de edição de um elemento é exclusiva ao seu tipo e oferece uma maneira simples de trabalhar com conteúdo. Os elementos possíveis que podem ser incluídos em um template de email são:

* Texto formatado
* Imagens
* Blocos de conteúdo
* Vídeos

## Texto formatado {#rich-text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [usando o Editor de Rich Text do Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Há duas maneiras de definir um elemento Rich Text dentro de um template de email: mktEditable e mktoText. Lembre-se de que um elemento Rich Text sempre pode ser convertido em um trecho no editor de email.

### Opção 1 - mktEditable {#option-mkteditable}

Como o Editor de email 2.0 é compatível com versões anteriores, alguns modelos de email antigos podem especificar elementos rich text adicionando class=&quot;mktEditable&quot; em qualquer elemento de HTML. Isso ainda é suportado e a ID do elemento é o que será usado como o nome de exibição dentro do editor de email.

Atributos obrigatórios

* **classe**: &quot;mktEditable&quot;.
* **id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.

Atributos opcionais

* **mktoName** : Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktEditable&quot; será usado como o valor padrão do elemento Rich Text.

Exemplo:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opção 2 - mktoText {#option-mktotext}

É recomendável especificar elementos de Rich Text usando a sintaxe class=&quot;mktoText&quot;. Isso garante que sempre haja um nome de exibição adequado para o elemento.

Atributos obrigatórios

* **classe**: &quot;mktoText&quot;
* **id**: Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName** : Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktoText&quot; será usado como o valor padrão do elemento Rich Text.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Imagens {#images}

Você tem duas opções para definir elementos de Imagem editáveis. Você pode usar um dos `<div>`, que especifica um contêiner que a variável `<img>` será inserido em ou em um `<img>` . Se você pretende que o usuário final simplesmente escolha uma imagem que retorne o URL da imagem (em vez do DOM), consulte &quot;variáveis de imagem&quot; na seção abaixo. As duas opções a seguir inserirão um HTML `<img>` elemento.

### Opção 1 - Usar um `<div>` {#option-use-a-div}

Atributos obrigatórios

* **classe:** &quot;mktoImg&quot;.
* **id:** Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName :** Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** Sequência de caracteres. O valor aqui será adicionado ao atributo de classe do `<img>` dentro do div.
* **mktoImgSrc:** A ser usado como o valor padrão para a imagem que é colocada dentro dessa div. Um espaço reservado é usado se isso for omitido.
* **mktoImgLink:** Indique que a variável `<img>` deve ser cercada por um `<a>` com esse URL de destino. O usuário pode alterar isso no Editor de email.
* **mktoImgLinkTarget:** Indique que a variável `<a>` A tag do atributo mktoImgLink deve usar esse destino. Não tem efeito se mktoImgLink também não for usado.
* **mktoImgWidth:** Usado como a largura no delimitado `<img>`.
* **mktoImgHeight:** Usado como a altura na área delimitada `<img>`.
* **mktoLockImgSize:** Usado para desbloquear o `<img>` propriedade height e width do elemento para que o usuário final possa modificar (o padrão é verdadeiro se omitido).
* **mktoLockImgStyle:** Usado para bloquear o `<img>` propriedade style do elemento (o padrão é false).

Valor padrão (opcional)

**`<img>`**: Para ser usado como o `<img>` elemento no qual a imagem será colocada. Útil se você quiser adicionar estilo em linha à imagem. Lembre-se de incluir ao redor `<a> </a>` , portanto, se o usuário adicionar um link, seu estilo não será removido!

Exemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opção 2 - Usar um \&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Essa opção não permite que usuários finais adicionem um link à imagem. Use a Opção 1 se isso for importante para o seu modelo.

Atributos obrigatórios

* **classe:** &quot;mktoImg&quot;.
* **id:** Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName:** Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.  Valor padrão (opcional)
* **src:** A ser usado como o valor padrão da imagem. Um espaço reservado é usado se isso for omitido.
* **mktoLockImgSize:** Usado para desbloquear o `<img>` propriedade height e width do elemento para que o usuário final possa modificar (o padrão é verdadeiro se omitido).
* **mktoLockImgStyle:** Usado para bloquear o `<img>` propriedade style do elemento (o padrão é false).

Exemplo:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Blocos de conteúdo {#snippets}

Se você definir uma região como um Snippet, os usuários finais poderão escolher qual aprovada [Snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)eles gostariam de inserir nesta região. Embora os elementos de Rich Text possam ser convertidos em Trechos no editor de email, quando você define uma região especificamente como um Snippet, ele não pode ser convertido em Rich Text. Você pode especificar uma região de Snippet usando uma `<div>` com class=&quot;mktoSnippet&quot;

Atributos obrigatórios

* **id:** Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName:** Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão (opcional)

**mktoDefaultSnippetId**: A ID numérica do trecho do Marketo que deve ser exibido por padrão (funcionará somente se um trecho com essa ID existir e for aprovado nesse espaço de trabalho).

Exemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vídeo {#video}

Se você definir uma região como um Vídeo, os usuários finais poderão inserir um URL de YouTube ou Vimeo que será exibido como uma imagem em miniatura (com o botão &quot;reproduzir&quot;) dentro do email. Você pode especificar uma região de Vídeo usando uma `<div>` com class=&quot;mktoVideo&quot;

Atributos obrigatórios

* **id:** Sequência de caracteres da ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName:** Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** Sequência de caracteres. O valor aqui será adicionado ao atributo de classe da miniatura do vídeo `<img>` dentro da div.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variáveis {#variables}

As variáveis são como tokens. Primeiro, defina-as na variável `<head>` seção do modelo de email usando `<meta>` , em seguida, use-as quantas vezes desejar em todo o modelo. Como são definidos no modelo, o usuário final poderá modificar seus valores de acordo com suas regras. Observe que você pode definir uma variável como local ou global no escopo. Se você usar uma variável em um &quot;Módulo&quot; (veja abaixo) e um usuário final duplicar esse módulo, as variáveis locais terão valores independentes, enquanto as variáveis globais serão aplicadas a ambos os módulos.

## Sequência de caracteres {#string}

Se você especificar uma variável como uma String, o usuário final poderá inserir texto em uma caixa de texto no editor de email. Você especifica uma variável de string usando `<meta>` com class=&quot;mktoString&quot;

Atributos obrigatórios

* **id:** Como você faz referência à variável no seu modelo de email.
* **mktoName:** Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **allowHTML:** Booleano. Controla se o valor da variável é HTML-escaped. O padrão é Falso se omitido.
* **default**: Valor padrão para a string. Em branco, se omitido.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Lista {#list}

Se você especificar uma variável como uma Lista, o usuário final poderá escolher entre um conjunto de valores que você definir no editor de email. Você especifica uma variável de Lista usando `<meta>` com class=&quot;mktoList&quot;

Atributos obrigatórios

* **id**: Como você faz referência à variável no seu modelo de email.
* **mktoName:** Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **valores:** Lista de valores separada por vírgulas. Deve ter pelo menos uma string.

Atributos opcionais

* **padrão:** Valor padrão da lista suspensa de seleção. Se omitido, o primeiro valor do atributo &quot;values&quot; será usado.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Número {#number}

Se você especificar uma variável como um Número, o usuário final poderá inserir um número no editor de email. Você especifica uma variável Number usando `<meta>` com class=&quot;mktoNumber&quot;

Atributos obrigatórios

* **id**: Como você faz referência à variável no seu modelo de email.
* **mktoName**: Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **padrão:** Valor numérico padrão para a variável .

Atributos opcionais

* **mín:** Valor mínimo aceito.
* **máx.:** Valor máximo aceito.
* **unidades:** Unidades a serem anexadas ao valor do número (por exemplo: px, pt, em etc.) quando exibido no Editor de email, bem como no código resultante.
* **etapa:** Quantas unidades a variável número deve aumentar/diminuir em (0.1, 1, 10, etc.). Se omitido, o padrão será 1.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Cor {#color}

Se você especificar uma variável como uma Cor, o usuário final poderá inserir um valor de cor hexadecimal ou escolher uma cor no seletor de cores no editor de email. Você especifica uma variável de cor usando `<meta>` com class=&quot;mktoColor&quot;

Atributos obrigatórios

* **id**: Como você faz referência à variável no seu modelo de email.
* **mktoName**: Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor padrão para a cor. Código de cor hexadecimal de 6 dígitos. Ex: #ffffff.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Se você especificar uma variável como booleana, o usuário final poderá ativar/desativar a opção no editor de email. Você especifica uma variável booleana usando `<meta>` com class=&quot;mktoBoolean&quot;

Atributos obrigatórios

* **id**: Como você faz referência à variável no seu modelo de email.
* **mktoName**: Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor booleano que determina o estado padrão da alternância de alternância. False, se omitido.
* **false_value:** O valor a ser inserido quando a alternância estiver na posição OFF. False, se omitido.
* **true_value:** O valor a ser inserido quando a alternância estiver na posição ATIVADO. Verdadeiro se omitido.
* **false_value_name:** Interface do usuário exibida no botão de alternância quando em posição OFF. False, se omitido.
* **true_value_name:** Interface do usuário exibida no botão de alternância quando em posição ATIVADA. Verdadeiro se omitido.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloco HTML {#html-block}

Se você especificar uma variável como um Bloco de HTML, o usuário final poderá inserir o HTML verbatim no editor de email. Você especifica uma variável HTML Block usando `<meta>` com class=&quot;mktoHTML&quot;

Atributos obrigatórios

* **id**: Como você faz referência à variável no seu modelo de email.
* **mktoName**: Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor codificado por HTML para servir como conteúdo padrão do bloco.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variável de imagem {#image-variable}

Se você especificar uma variável como uma Imagem, o usuário final poderá escolher uma imagem do seletor de imagens no editor de email. O URL da imagem selecionada será o valor da variável . Você especifica uma variável de imagem usando `<meta>` com class=&quot;mktoImg&quot;

Atributos obrigatórios

* **id**: Como você faz referência à variável no seu modelo de email.
* **mktoName**: Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** URL da imagem padrão do elemento.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é Falso se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Módulos {#modules}

Os módulos são seções personalizadas definidas no nível do modelo que serão exibidas para os usuários finais inserirem no email. Como você pré-criou esses módulos, é possível garantir que eles interajam com o restante do seu conteúdo de email normalmente (de maneira totalmente responsiva). Você só pode colocar um módulo em um contêiner.

>[!IMPORTANT]
>
>Quando um email é gerado a partir de um template de email que contém componentes de módulo definidos, qualquer alteração feita nos módulos do modelo **not** ser encaminhado para o email mencionado.

**Para contêineres do tipo `<table>`, `<tbody>`, `<thead>`ou `<tfoot>`:**

Especificado usando `<tr>` com class=&quot;mktoModule&quot;

**Para contêineres do tipo `<td>`:**

Especificado usando `<table>` com class=&quot;mktoModule&quot;

Atributos obrigatórios

* **id**: Como você faz referência ao módulo no seu modelo de email.
* **mktoName**: Sequência de caracteres. Este é o nome de exibição que será exibido no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoActive:** Determina se esse módulo aparece na lista de módulos no editor de email. O padrão é true. Se falso, o módulo não pode ser adicionado por um usuário final a um email.
* **mktoAddByDefault:** Determina se esse módulo estará na tela de um novo email que usa esse modelo após a criação. O padrão é true (se mktoActive for falso, esse valor será ignorado).

>[!NOTE]
>
>Valores de classe contendo a sintaxe Marketo (ou seja, mktoModule, mktoContainer, mktoText) fazem distinção entre maiúsculas e minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não são.

## Contêineres {#containers}

Um contêiner contém Módulos e define onde eles podem ser colocados. Quando os usuários finais reorganizam e inserem módulos em seu email, o contêiner controla para onde eles podem ir.

**Especificado usando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` ou `<td>` com class=&quot;mktoContainer&quot;**

Atributos obrigatórios

**id**: Como você faz referência ao módulo no seu modelo de email.

>[!CAUTION]
>
>Os contêineres só podem conter módulos; se houver algo mais presente, o contêiner será considerado inválido! Somente um contêiner é permitido por modelo.
