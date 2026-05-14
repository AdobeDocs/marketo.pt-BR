---
solution: Marketo Engage
product: marketo
title: Fragmentos personalizáveis
description: Saiba como personalizar fragmentos tornando alguns campos editáveis. Crie fragmentos reutilizáveis flexíveis no Designer de email.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: fdc003d7aed05d85687427d9455bb806eb33d0b2
workflow-type: tm+mt
source-wordcount: 1403
ht-degree: 0%

---

# Fragmentos personalizáveis {#customizable-fragments}

Quando os fragmentos são usados em um email ou modelo de email, eles são bloqueados por padrão devido à herança, o que significa que quaisquer alterações feitas em um fragmento são propagadas automaticamente para todos os ativos onde ele é usado. Com fragmentos personalizáveis, campos específicos em um fragmento podem ser definidos como editáveis quando o fragmento é adicionado a um email ou modelo de email. Por exemplo, se você tiver um fragmento com um banner, algum texto e um botão, poderá designar determinados campos, como a imagem ou o URL de destino do botão, como editáveis.

Os fragmentos personalizáveis permitem gerenciar e personalizar o conteúdo sem criar blocos de conteúdo totalmente novos ou interromper a herança do fragmento. As alterações feitas no nível do fragmento ainda são propagadas, enquanto permitem personalização no nível do email ou do template de email.

Os fragmentos visuais e de expressão podem ser marcados como personalizáveis.

## Adicionar campos editáveis em fragmentos visuais {#visual}

Para tornar partes de um fragmento visual editáveis, siga estas etapas:

>[!NOTE]
>
>Campos editáveis podem ser adicionados aos componentes **imagem**, **texto** e **botão**. Para componentes do **HTML**, os campos editáveis são adicionados usando o editor de personalização, semelhante aos fragmentos de expressão. [Saiba mais sobre campos editáveis em componentes do HTML em fragmentos](#editable-html)

1. Abra a tela de edição de conteúdo do fragmento.

1. Selecione o componente no fragmento onde deseja configurar campos editáveis.

1. O painel de propriedades do componente é aberto no lado direito. Selecione a guia **[!UICONTROL Campos editáveis]** e alterne a opção **[!UICONTROL Habilitar edição]**.

1. Todos os campos que podem ser editados para o componente selecionado são listados no painel. Os campos disponíveis para edição dependem do tipo de componente selecionado.

   No exemplo abaixo, o URL do botão &quot;Clique aqui&quot; está configurado como editável.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Clique em **[!UICONTROL Visão geral]** para verificar todos os campos editáveis e seus valores padrão.

   Neste exemplo, o campo URL do botão é exibido com o valor padrão definido no componente. Os usuários podem personalizar esse valor depois de adicionar o fragmento ao seu conteúdo.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Salve as alterações ao concluir.

Depois de adicionar o fragmento a um email, os usuários podem personalizar todos os campos editáveis configurados no fragmento.

## Componentes editáveis do HTML em fragmentos {#editable-html}

Em um componente do HTML, os seguintes tipos de elementos podem se tornar editáveis:

* Uma parte de **conteúdo de texto** (por exemplo, um título ou um rótulo CTA).
* Uma **URL** completa, usada como um destino de link ou uma fonte de imagem. URLs parciais não são suportados; a variável deve representar todo o valor do URL.
* Um **valor de propriedade CSS** completo (por exemplo, um valor de cor total, um valor de preenchimento completo ou um valor de largura total). Não há suporte para valores parciais de propriedade CSS.

Cada valor de propriedade CSS com parâmetros deve ser exatamente `{{{varName}}}`: sem sufixos, sem texto adicional, sem várias variáveis e sem concatenação em uma única propriedade.

Para parametrizar propriedades de vários lados, como preenchimento:

* declare cada lado como uma propriedade separada _(recomendado)_ ou
* declare uma única variável que contenha o valor abreviado completo.

## Como os campos editáveis funcionam nos componentes do HTML {#components}

Os campos editáveis em um componente do HTML são criados declarando variáveis em linha diretamente dentro do código-fonte do componente. Cada variável tem uma ID exclusiva e um valor padrão. A variável é referenciada sempre que o valor editável deve aparecer na marcação.

Depois que o fragmento é salvo e publicado, cada variável declarada no componente do HTML é automaticamente exibida como um parâmetro editável quando o fragmento é adicionado a um email.

O autor do email pode substituir o valor padrão de qualquer variável do Designer de email (por exemplo, alterar uma cor de fundo, trocar um URL do CTA ou atualizar um título) sem modificar o HTML subjacente.

## Referência de sintaxe {#syntax}

Os campos editáveis são definidos e referenciados usando dois padrões:

### Declaração de uma variável {#declaring}

Use a declaração em linha para definir uma variável com um identificador exclusivo e um valor padrão:

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

Substitua `variableID` por um identificador exclusivo para o campo editável. A ID deve ser exclusiva no componente e não deve conter espaços.

Substitua `default_value` pelo valor que deve ser usado se o autor do email não o substituir.

### Referência a uma variável {#referencing}

Use chaves triplas para fazer referência à variável onde quer que seu valor deva aparecer na marcação:

```handlebars
{{{variableID}}}
```

A mesma ID de variável pode ser referenciada várias vezes na HTML. Todas as referências resolverão para qualquer valor que o autor do email definir (ou para o valor padrão se nenhuma substituição for fornecida).

### Parâmetros opcionais {#optional}

A declaração em linha suporta parâmetros opcionais que alteram como o campo editável é apresentado ou processado:

| Ação | Parâmetro | Exemplo |
|---|---|---|
| Declarar um campo editável com um **valor padrão**. Quando o fragmento é adicionado a um email, esse valor padrão é usado, a menos que o autor o substitua. | Adicione o valor padrão entre as tags em linha. | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| Defina um **rótulo** para o campo editável. Esse rótulo é exibido no Designer de email quando o autor do email edita os campos do fragmento. | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| Declare um campo editável que contenha uma **origem da imagem**. | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| Declarar um campo editável que contenha uma **URL** que precise ser rastreada. | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## Adicionar campos editáveis a um componente do HTML {#adding-editable-fields}

Para tornar editáveis partes de um componente do HTML em um fragmento visual, siga estas etapas:

1. Abra o fragmento visual para edição no Designer de email.
1. Adicione um **componente do HTML** ao fragmento no painel Componentes ou selecione um componente existente do HTML.
1. Com o componente do HTML selecionado, clique em **Mostrar código-fonte** para abrir a exibição do código-fonte do HTML no editor de personalização.
1. No editor de personalização, declare cada variável editável usando a sintaxe de declaração em linha. Coloque todas as declarações de variável na parte superior do componente para facilitar a leitura e atribua uma ID exclusiva a cada variável.
1. Faça referência a cada variável na marcação HTML usando a sintaxe `{{{variableID}}}` sempre que o valor editável for exibido. A mesma variável pode ser referenciada várias vezes no mesmo componente.
1. Salve o componente HTML e, em seguida, salve o fragmento.
1. Publique o fragmento para disponibilizá-lo para uso em emails.

## Uso do fragmento em um email {#using-fragment}

Depois que o fragmento é publicado, todas as variáveis declaradas em seus componentes do HTML são exibidas como parâmetros editáveis no Designer de email.

Para personalizá-los ao usar o fragmento em um email:

1. Abra ou crie um email no Designer de email do Marketo Engage.
1. Adicione o fragmento publicado à tela de email.
1. Selecione o fragmento para abrir o painel de propriedades. A lista de campos editáveis é exibida na seção **Campos editáveis**, com cada campo rotulado por sua ID de variável (ou pelo rótulo amigável especificado por meio do parâmetro `name`).
1. Atualize o valor de qualquer campo editável diretamente do painel de propriedades. A alteração se aplica somente ao email atual; o fragmento publicado e outros emails que fazem referência a ele permanecem inalterados.
1. Salve o email.

O fragmento é renderizado com os valores personalizados, enquanto ainda herda quaisquer atualizações estruturais futuras feitas no fragmento publicado.

### Exemplo: fragmento simples com texto, cor e URL editáveis {#example}

O exemplo a seguir cria um pequeno banner promocional com quatro campos editáveis:

* uma cor de fundo
* um texto de título
* um rótulo do CTA
* um URL do CTA

Depois de publicar o fragmento, um autor de email pode substituir qualquer um desses valores ao adicionar o fragmento a um email.

**Banner editável simples**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

Neste exemplo:

* `bgColor` é referenciado duas vezes: uma para a cor de fundo da tabela e outra para a cor de texto do CTA. Ambas as referências são resolvidas para o mesmo valor, portanto, uma única edição se propaga para ambos os locais.
* `ctaUrl` é declarado com `assetType="url"`, que indica que o valor deve ser processado como uma URL rastreada.

## Práticas recomendadas {#best-practices}

* Inclua unidades (`px`, `em`, `%`) dentro do valor padrão da variável, de modo que a variável represente um valor CSS completo. Isso evita a concatenação, que não é compatível.
* Preferir propriedades CSS longas por lado (`padding-top`, `padding-right`, `padding-bottom`, `padding-left`) em vez de abreviação quando cada lado precisar ser editado independentemente.
* Quando um URL precisar ser rastreado, declare com `assetType="url"`.
* Quando um campo editável transporta uma fonte de imagem, declare com `assetType="image"`.
* Teste o fragmento adicionando-o a um email de rascunho e verificando se todos os campos editáveis aparecem no painel de propriedades e são resolvidos corretamente quando substituídos.

## O que você deve saber {#things-to-know}

* Campos editáveis em componentes do HTML são compatíveis com conteúdo de texto completo, URLs completos e valores de propriedade CSS completos. URLs parciais e valores parciais de propriedade CSS não podem ser parametrizados.
* Um único valor de propriedade CSS não pode combinar uma variável com texto estático adicional ou com outra variável. Cada valor de propriedade parametrizada deve ser exatamente uma referência de variável.
* As IDs de variáveis devem ser exclusivas em um componente do HTML e não devem conter espaços.
* Links do sistema prontos para uso, como o link de cancelamento de inscrição e o URL da mirror page, não podem ser transformados em campos editáveis.

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[Fragmentos](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
