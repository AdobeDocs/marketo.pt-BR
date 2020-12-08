---
unique-page-id: 11371040
description: Sintaxe do modelo de email - Documentos do marketing - Documentação do produto
title: Sintaxe do modelo de email
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---


# Sintaxe do modelo de email {#email-template-syntax}

Na nova experiência do Marketo com e-mail 2.0, os modelos de e-mail são compostos de qualquer combinação de Elementos, Variáveis, Módulos ou Container. Cada uma é definida adicionando sintaxe específica de marketing ao seu HTML. Modelos de email antigos (v1.0) são suportados no Editor de email 2.0; no entanto, eles não incluirão todos os recursos do novo Editor.

A sintaxe de e-mail de marketing só funciona em modelos e e-mails individuais; ele **não** funciona se incorporado a fragmentos ou tokens Rich Text.

>[!NOTE]
>
>O suporte de marketing não está configurado para auxiliar com CSS/HTML. Se você não estiver familiarizado com CSS/HTML, consulte seu desenvolvedor.

>[!CAUTION]
>
>Os valores de classe que contêm a sintaxe Marketo (ou seja, mktoModule, mktoContainer, mktoText) fazem distinção entre maiúsculas e minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não são.

## Elementos {#elements}

Os elementos são regiões de conteúdo que você define como editável no seu modelo de email. A experiência de edição de um elemento é exclusiva ao seu tipo e oferta uma maneira simples de trabalhar com conteúdo. Os possíveis elementos que podem ser incluídos em um modelo de email são:

* Rich Text
* Imagens
* Trechos
* Vídeos

## Rich Text {#rich-text}

Se você definir uma região como Rich Text, os usuários poderão editar seu conteúdo [usando o Editor](../../../../product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)de Rich Text do Marketo. Há duas maneiras de definir um elemento Rich Text dentro de um modelo de email: mktEditable e mktoText. Lembre-se de que um elemento Rich Text sempre pode ser convertido em um fragmento no editor de email.

### Opção 1 - mktEditable {#option-mkteditable}

Como o Editor de e-mail 2.0 é compatível com versões anteriores, alguns modelos de e-mail antigos podem especificar elementos Rich Text adicionando class=&quot;mktEditable&quot; em qualquer elemento HTML. Isso ainda é suportado e a ID do elemento é o que será usado como o nome de exibição no editor de email.

Atributos necessários

* **classe**: &quot;mktEditable&quot;.
* **id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.

Atributos opcionais

* **mktoName** : String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo no elemento HTML (se fornecido) com class=&quot;mktEditable&quot; será usado como o valor padrão do elemento Rich Text.

Exemplo:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opção 2 - mktoText {#option-mktotext}

É recomendável especificar elementos Rich Text usando a sintaxe class=&quot;mktoText&quot;. Isso garante que sempre haja um nome de exibição adequado para o elemento.

Atributos necessários

* **classe**: &quot;mktoText&quot;
* **id**: Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName** : String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão

O conteúdo dentro do elemento HTML (se fornecido) com class=&quot;mktoText&quot; será usado como o valor padrão para o elemento Rich Text.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Imagens {#images}

Você tem duas opções para definir elementos de Imagem editáveis. Você pode usar um `<div>`, que especifica um container no qual o `<img>` será inserido, ou uma `<img>` tag. Se você pretende que o usuário final simplesmente escolha uma imagem que retorne o URL da imagem (em vez do DOM), consulte &quot;variáveis de imagem&quot; na seção abaixo. As duas opções a seguir inserirão um `<img>` elemento HTML.

### Opção 1 - Use um \&lt;div\> {#option-use-a-div}

Atributos necessários

* **classe:** &quot;mktoImg&quot;.
* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName :** String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** String. O valor aqui será adicionado ao atributo class do `<img>` elemento dentro de div.
* **mktoImgSrc:** A ser usado como valor padrão para a imagem que é colocada dentro desta div. Um espaço reservado é usado se for omitido.
* **mktoImgLink:** Indique que o `<img>` deve estar rodeado por uma `<a>` tag com este URL de destino. O usuário pode alterar isso no Editor de email.
* **mktoImgLinkTarget:** Indique se a `<a>` tag do atributo mktoImgLink deve usar esse público alvo. Não tem efeito se mktoImgLink também não for usado.
* **mktoImgWidth:** Usada como a largura no delimitado `<img>`.
* **mktoImgHeight:** Usada como a altura no delimitado `<img>`.
* **mktoLockImgSize:** Usado para desbloquear a propriedade de altura e largura do `<img>` elemento para que o usuário final possa modificar (o padrão é verdadeiro se omitido).
* **mktoLockImgStyle:** Usado para bloquear a propriedade style do `<img>` elemento (o padrão é false).

Valor padrão (opcional)

**`<img>`**: A ser usado como o `<img>` elemento no qual a imagem será colocada. Útil se você quiser adicionar estilos em linha à imagem. Lembre-se de incluir `<a> </a>` as tags adjacentes. Portanto, se o usuário adicionar um link, seu estilo não será removido!

Exemplo:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="http://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opção 2 - Use um \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Essa opção não permite que os usuários finais adicionem um link à imagem. Use a Opção 1 se isso for importante para o seu modelo.

Atributos necessários

* **classe:** &quot;mktoImg&quot;.
* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName:** String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.  Valor padrão (opcional)
* **src:** A ser usado como valor padrão para a imagem. Um espaço reservado é usado se for omitido.
* **mktoLockImgSize:** Usado para desbloquear a propriedade de altura e largura do `<img>` elemento para que o usuário final possa modificar (o padrão é verdadeiro se omitido).
* **mktoLockImgStyle:** Usado para bloquear a propriedade style do `<img>` elemento (o padrão é false).

Exemplo:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Trechos {#snippets}

Se você definir uma região como um Snippet, os usuários finais poderão escolher qual [](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)Snippet aprovado eles gostariam de inserir nesta região. Embora os elementos Rich Text possam ser convertidos em Snippets no editor de email, quando você define uma região especificamente como um Snippet, ele não pode ser convertido em Rich Text. Você pode especificar uma região Snippet usando um `<div>` com class=&quot;mktoSnippet&quot;

Atributos necessários

* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName:** String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Valor padrão (opcional)

**mktoDefaultSnippetId**: A ID numérica do trecho de marketing que deve aparecer por padrão (só funcionará se existir um trecho com essa ID e for aprovado nesse espaço de trabalho).

Exemplo:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Vídeo {#video}

Se você definir uma região como um Vídeo, os usuários finais poderão inserir um URL do YouTube ou do Vimeo que será exibido como uma imagem em miniatura (com o botão &quot;play&quot;) dentro do email. Você pode especificar uma região de Vídeo usando um `<div>` com class=&quot;mktoVideo&quot;

Atributos necessários

* **id:** Sequência de ID. Contém apenas letras, números, traço &quot;-&quot; e sublinhado &quot;_&quot;. Não são permitidos espaços. Deve ser único.
* **mktoName:** String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoImgClass:** String. O valor aqui será adicionado ao atributo class da miniatura de vídeo `<img>` dentro da div.

Exemplo:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variáveis {#variables}

As variáveis são como tokens. Primeiro, você os define na seção `<head>` do modelo de e-mail usando `<meta>` tags e, em seguida, os usa quantas vezes desejar em todo o modelo. Como estão definidos no modelo, o usuário final poderá modificar seus valores de acordo com suas regras. Observe que é possível definir uma variável como local ou global no escopo. Se você usar uma variável dentro de um &quot;Módulo&quot; (veja abaixo) e um usuário final duplicados desse módulo, as variáveis locais terão valores independentes, enquanto as variáveis globais se aplicarão a ambos os módulos.

## String {#string}

Se você especificar uma variável como uma string, o usuário final poderá digitar texto em uma caixa de texto no editor de email. Você especifica uma variável String usando `<meta>` com class=&quot;mktoString&quot;

Atributos necessários

* **id:** Como você faz referência à variável em seu modelo de email.
* **mktoName:** String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **allowHTML:** Booleano. Controla se o valor da variável é de escape HTML. O padrão é False, se omitido.
* **padrão**: Valor padrão para a string. Em branco se omitido.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Lista {#list}

Se você especificar uma variável como uma Lista, o usuário final poderá escolher entre um conjunto de valores que você definir no editor de email. Você especifica uma variável de Lista usando `<meta>` com class=&quot;mktoList&quot;

Atributos necessários

* **id**: Como você faz referência à variável em seu modelo de email.
* **mktoName:** String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **valores:** Lista de valores separada por vírgulas. Deve ter pelo menos uma string.

Atributos opcionais

* **padrão:** Valor padrão da lista suspensa selecionada. Se omitido, o primeiro valor do atributo &quot;values&quot; é usado.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Número {#number}

Se você especificar uma variável como um Número, o usuário final poderá inserir um número no editor de email. Você especifica uma variável Number usando `<meta>` com class=&quot;mktoNumber&quot;

Atributos necessários

* **id**: Como você faz referência à variável em seu modelo de email.
* **mktoName**: String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.
* **padrão:** Valor numérico padrão para a variável.

Atributos opcionais

* **min:** Valor mínimo aceito.
* **máx.:** Valor máximo aceito.
* **unidades:** Unidades a acrescentar ao valor numérico (por exemplo: px, pt, em etc.) quando exibido no Editor de email, bem como no código resultante.
* **etapa:** Quantas unidades a variável de número deve aumentar/diminuir em (0,1, 1, 10 etc.). Se omitido, o padrão é 1.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Cor {#color}

Se você especificar uma variável como uma Cor, o usuário final poderá inserir um valor de cor hexadecimal ou escolher uma cor no seletor de cores no editor de e-mail. Você especifica uma variável Color usando `<meta>` com class=&quot;mktoColor&quot;

Atributos necessários

* **id**: Como você faz referência à variável em seu modelo de email.
* **mktoName**: String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor padrão para a cor. Código de cor hexadecimal de 6 dígitos. Ex: #ffffff.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Se você especificar uma variável como booleana, o usuário final poderá ativar/desativar a opção no editor de email. Você especifica uma variável Booleana usando `<meta>` com class=&quot;mktoBoolean&quot;

Atributos necessários

* **id**: Como você faz referência à variável em seu modelo de email.
* **mktoName**: String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor booliano que determina o estado padrão do switch de alternância. Falso se omitido.
* **false_value:** O valor a ser inserido quando a alternância estiver na posição OFF. Falso se omitido.
* **true_value:** Valor a ser inserido quando a alternância estiver na posição ON. Verdadeiro se omitido.
* **false_value_name:** Interface do usuário exibida na alternância quando na posição OFF. Falso se omitido.
* **true_value_name:** IU mostrada na alternância quando em posição ON. Verdadeiro se omitido.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Bloco HTML {#html-block}

Se você especificar uma variável como um Bloco HTML, o usuário final poderá inserir um HTML textual no editor de email. Você especifica uma variável de Bloco HTML usando `<meta>` com class=&quot;mktoHTML&quot;

Atributos necessários

* **id**: Como você faz referência à variável em seu modelo de email.
* **mktoName**: String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** Valor codificado em HTML para servir como conteúdo padrão do bloco.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variável de imagem {#image-variable}

Se você especificar uma variável como uma Imagem, o usuário final poderá escolher uma imagem do seletor de imagem no editor de email. O URL da imagem selecionada será o valor da variável. Você especifica uma variável de Imagem usando `<meta>` com class=&quot;mktoImg&quot;

Atributos necessários

* **id**: Como você faz referência à variável em seu modelo de email.
* **mktoName**: String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **padrão:** URL da imagem padrão para o elemento.
* **mktoModuleScope**: Booleano. Controla se a variável é local (true) ou global (false) quando usada em um módulo. O padrão é False, se omitido.

Exemplo de declaração:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="http://www.company.com/image.jpg"></pre>`

Exemplo de uso:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Módulos {#modules}

Os módulos são seções templatizadas definidas no nível do modelo que serão exibidas para que os usuários finais sejam inseridos em seus emails. Como você pré-criou esses módulos, é possível garantir que eles interajam com o restante do seu conteúdo de email de forma graciosa (de maneira totalmente responsiva). Você só pode colocar um módulo em um container.

**Para container do tipo `<table>`, `<tbody>`, `<thead>`ou `<tfoot>`:**

Especificado usando `<tr>` com class=&quot;mktoModule&quot;

**Para container do tipo `<td>`:**

Especificado usando `<table>` com class=&quot;mktoModule&quot;

Atributos necessários

* **id**: Como você consulta o módulo em seu modelo de email.
* **mktoName**: String. Esse é o nome para exibição que será mostrado no Editor de email 2.0. A prática recomendada é usar um nome descritivo.

Atributos opcionais

* **mktoActive:** Determina se este módulo aparece na lista de módulos no editor de e-mail. O padrão é true. Se falso, o módulo não pode ser adicionado por um usuário final a um email.
* **mktoAddByDefault:** Determina se este módulo estará na tela de um novo e-mail que usa este modelo após a criação. O padrão é true (se mktoActive for false, esse valor será ignorado).

>[!NOTE]
>
>**Lembrete**
>
>Os valores de classe que contêm a sintaxe Marketo (ou seja, mktoModule, mktoContainer, mktoText) fazem distinção entre maiúsculas e minúsculas. Os nomes de atributos personalizados (ou seja, mktoimgwidth, mktoname) não são.

## Container {#containers}

Um container contém Módulos e define onde eles podem ser colocados. Quando os usuários finais estão reorganizando e inserindo módulos em seus emails, o container controla para onde eles podem ir.

**Especificado usando `<table>`, `<tbody>`, `<thead>``<tfoot>` ou `<td>` com class=&quot;mktoContainer&quot;**

Atributos necessários

**id**: Como você consulta o módulo em seu modelo de email.

>[!CAUTION]
>
>Os container só podem conter Módulos - se houver mais alguma coisa presente, o Container é considerado inválido! Somente um container é permitido por modelo.
