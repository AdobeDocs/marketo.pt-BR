---
title: Criar conteúdo acessível
description: Saiba como criar conteúdo acessível para seus emails no Adobe Marketo Engage.
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: email, design, acessibilidade
source-git-commit: 5adfebfd8f9f0cdaebb1eb86a68c136d46298446
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 0%

---

# Criar conteúdo acessível {#accessible-content}

A [Lei Europeia da Acessibilidade](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882){target="_blank"} é uma diretiva destinada a reforçar o mercado interno de produtos e serviços acessíveis, eliminando os obstáculos causados pelas diferentes regras nacionais entre os Estados-Membros.

Esse regulamento estabelece que todas as comunicações digitais, incluindo emails, boletins informativos, PDFs e conteúdo para download, devem estar acessíveis. Ao criar conteúdo para seus destinatários, você deve seguir diretrizes específicas, como o uso de fontes acessíveis e formatos legíveis e o fornecimento de texto alternativo para imagens.

O Marketo Engage Email Designer permite cumprir facilmente esta diretiva, com base nas Web Content Accessibility Guidelines (WCAG) 2.1, nível AA. As práticas recomendadas para criar conteúdo acessível com o Marketo Engage estão listadas abaixo.

>[!NOTE]
>
>Esta página trata de tornar o conteúdo acessível a todos os recipients, para que as pessoas com deficiência possam ler, entender e interagir com seus emails criados no Marketo Engage.

## Garantir a legibilidade do texto {#text-readability}

Use a guia **[!UICONTROL Estilos]** do componente **[!UICONTROL Texto]** para garantir que o texto seja legível, por exemplo, usando contraste de cores adequado e fontes simples.

<!--![](assets/accessible-text-styles.png){width="80%"}-->

Para fontes e texto, siga estas diretrizes:

**Seleção de fonte**

* Use fontes sans-serif como Arial, Verdana, Tahoma, Helvetica ou Open Sans.
* Evite fontes serif, cursivas ou decorativas no conteúdo do corpo.
* Use um conjunto de fontes limitado para fins de consistência e fallback (por exemplo: `font-family: Arial, Helvetica, sans-serif;`).

**Dimensionamento de fonte**

* Verifique um tamanho de fonte mínimo de 16px para o corpo de texto.
* Use hierarquia adequada para cabeçalhos.

**Contraste de cores**

* Mantenha uma taxa de contraste de pelo menos 4,5:1 entre o texto e o plano de fundo.
* Para textos grandes (≥ 24px ou bold 18px), verifique se há pelo menos um contraste de 3:1.
* Evite texto cinza-claro ou pastel em planos de fundo brancos.
* Não confie apenas na cor para transmitir significado. Use sublinhados, ícones, etc.

**Acessibilidade de texto**

* Evite texto em imagens.
* Não use todas as letras maiúsculas no corpo de texto.
* Garanta que o texto possa ser ampliado até 200% sem quebrar o layout.

## Garantir acessibilidade visual {#visual-accessibility}

* Evite usar indicadores somente de cores para informações importantes.
* Use rótulos de texto ou ícones para maior clareza.
* Otimize seu design para layouts móveis e responsivos, garantindo que os botões sejam grandes e espaçados corretamente.
* Teste regularmente entre dispositivos e tamanhos de tela para manter a acessibilidade.

No Marketo Engage, o tamanho e o espaçamento dos diferentes elementos no seu conteúdo podem ser refinados usando os parâmetros de estilo e atributos do painel **[!UICONTROL Estilos]** do Email Designer.

Por exemplo, você pode atualizar o plano de fundo ou alterar as margens, o preenchimento e o alinhamento para melhorar a acessibilidade visual.

<!--![](assets/accessible-styles.png){width="80%"}-->

O Marketo Engage Email Designer permite pré-visualizar e otimizar o design para diferentes dispositivos e tamanhos de tela. A qualquer momento, você pode **[!UICONTROL Alternar para o modo de exibição ativo]** para verificar como o conteúdo pode ser renderizado em vários tamanhos de dispositivo.

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>A visualização em tempo real é uma visualização genérica criada para comparar como o conteúdo pode ser renderizado em vários tamanhos de dispositivo. A renderização final pode variar de acordo com o cliente de email do recipient.

## Usar texto alternativo para imagens {#alt-text}

Use o componente **[!UICONTROL Imagem]** para fornecer texto alternativo para imagens.

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* Descreva a finalidade da imagem de forma concisa e contextual.
* Evite frases redundantes como &quot;Imagem de...&quot; e use texto alternativo vazio para imagens decorativas.
* Para ícones com significado, forneça rótulos significativos e para imagens complexas, use um breve texto alternativo mais uma descrição mais longa em outro lugar.

## Usar formato legível {#readable-format}

Use a estrutura relevante do Email Designer e os componentes do conteúdo, bem como as opções no painel **[!UICONTROL Estilos]**, para organizar o conteúdo de forma clara, lógica e concisa, acessível a todos.

<!--![](assets/accessible-components.png){width="100%"}-->

* Use HTML estruturado e semântico com cabeçalhos, parágrafos, listas e tabelas adequados.
* Garantir que o conteúdo siga um fluxo lógico da esquerda para a direita, de cima para baixo.
* Use uma linguagem clara e concisa.
* Fornecer formatos alternativos para PDFs e infográficos.
* Permita o redimensionamento e o refluxo do texto e verifique se a tipografia é legível com contraste de cor adequado em todos os formatos.

## Garantir a legibilidade do conteúdo {#readability}

Para ser legível, seu conteúdo deve ser claro, bem estruturado e utilizável por todos, incluindo pessoas com dificuldades visuais, cognitivas ou de leitura e aquelas que usam tecnologias assistivas. Alguns pontos a serem considerados ao criar conteúdo acessível incluem:

* Mantenha as sentenças em torno de 20 palavras ou menos.
* Edite sua cópia para que seja direta e concisa.
* Use a voz ativa para manter a estrutura da frase mais simples.
* Evite gírias, jargões ou palavras regionais com as quais algumas pessoas possam não estar familiarizadas.

Para avaliar sua legibilidade de email, você pode usar o popular [Teste de Facilidade de Leitura Flesch](https://support.microsoft.com/en-us/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"}, que pode ser encontrado no Microsoft Word e calcula como é fácil ler seu conteúdo em uma escala de 0 a 100.

## Testar seu conteúdo {#test}

Para verificar a acessibilidade do conteúdo, você pode usar os recursos de teste fornecidos pelo Marketo Engage. Eles não foram projetados especificamente para verificar se o conteúdo está totalmente acessível, mas podem fornecer um primeiro nível de verificação.

* Pré-visualize o conteúdo usando perfis de teste.

* Use a opção [Renderização de email](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"} que usa o Litmus para simular seus designs nos principais clientes de email (Apple Mail, Gmail, Outlook) e ver se o texto, as cores e as imagens tornam seu conteúdo acessível. <!--Litmus includes accessibility testing-->

* Envie provas para testar a renderização do seu conteúdo antes de enviá-lo para o seu público real.

<!--![](assets/accessible-simulate.png){width="90%"}-->

Para verificar de maneira mais consistente se o conteúdo está acessível de maneira confiável, procure por ferramentas externas específicas, como:

* O [verificador de contraste do WebAim](https://webaim.org/resources/contrastchecker/){target="_blank"} e a [ferramenta de avaliação de acessibilidade da Web do WAVE](https://wave.webaim.org/){target="_blank"} para avaliar o contraste e a conformidade;

* Tecnologias assistivas, como leitores de tela (por exemplo: [NVDA](https://www.nvaccess.org/download/){target="_blank"} ou [VoiceOver](https://support.apple.com/en-ie/guide/iphone/iph3e2e415f/ios){target="_blank"} no iPhone), para experimentar emails da perspectiva de usuários com deficiências visuais.

## Usar modo escuro {#dark-mode}

O [modo escuro](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"} aprimora a acessibilidade visual para usuários com sensibilidade à luz ou deficiências visuais, melhorando a experiência de visualização.

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

Algumas práticas recomendadas para criar conteúdo no modo escuro incluem:

* Uso de PNGs ou SVGs transparentes
* Definição de metatags e CSS apropriados
* Fornecer estilo de fallback acessível se o modo escuro não for suportado.

Verifique se os emails são renderizados corretamente no modo escuro, testando todo o conteúdo de email e os elementos da interface do usuário nos modos claro e escuro.

## Usar atributos específicos para acessibilidade {#attributes}

### Atributos de idioma {#language}

Ao criar designs, inclua os atributos `lang` (idioma) e `dir` (direção de texto) no corpo do conteúdo. Esses atributos ajudam as tecnologias assistivas (como leitores de tela) a interpretar e apresentar seu conteúdo de maneira apropriada.

* O atributo `lang` indica o idioma do email para tecnologias assistivas, garantindo que as palavras sejam pronunciadas corretamente.

  +++Exemplos

  Exemplo para inglês:

  ```
  <body lang="en">
  ```

  Exemplo para francês:

  ```
  <body lang="fr">
  ```

  +++

* O atributo `dir` especifica a direção do texto. A maioria dos idiomas, incluindo inglês e francês, são lidos da esquerda para a direita (ltr), enquanto idiomas como árabe e hebraico são lidos da direita para a esquerda (rtl).

  +++Exemplos

  Exemplo para inglês (da esquerda para a direita):

  ```html
  <body lang="en" dir="ltr">
  ```

  Exemplo para árabe (da direita para a esquerda):

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

Os leitores de tela dependem do atributo `lang` para aplicar as regras de pronúncia corretas, enquanto a direção do texto garante o fluxo do conteúdo naturalmente para idiomas da esquerda para a direita ou da direita para a esquerda. Sem esses atributos, os usuários podem enfrentar ordem de leitura confusa ou pronúncia incorreta. Sempre envolva seu corpo de email com os atributos `lang` e `dir` apropriados.

>[!TIP]
>
>Se o email contiver vários idiomas, atribua os atributos de idioma apropriados a seções específicas (como blocos `<table>` ou `<td>`) para garantir que cada parte seja lida corretamente.

### Tabelas {#tables}

No conteúdo do HTML, as tabelas são frequentemente usadas para layout. Por padrão, os leitores de tela tratam cada `<table>` como uma tabela de dados, anunciando linhas, colunas e estrutura. Isso pode ser confuso se a tabela for usada apenas para formatação.

Adicione `role="presentation"` (ou `role="none"`) às tabelas de layout para garantir que as tecnologias assistivas ignore sua estrutura e se concentre apenas no conteúdo real.

+++Exemplo - Tabela de layout (com `role="presentation"`)

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

Os leitores de tela leem:
&quot;Olá, Mundo. Bem-vindo ao nosso informativo.&quot; _(Nenhuma menção de linhas, colunas ou tabela)_

+++

+++Exemplo - Tabela de dados (sem `role="presentation"`)

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

Os leitores de tela leem:
&quot;Tabela com 2 colunas e 3 linhas.&quot;

&quot;Nome, Peter. Pontuação, 19.&quot;

&quot;Nome, Parker. Pontuação, 62.&quot;

+++

>[!TIP]
>
>Use `role="presentation"` exclusivamente para tabelas de layout. Para tabelas de dados, mantenha a estrutura semântica `<table>` para que os leitores de tela possam anunciar corretamente cabeçalhos e relações.

### Texto para links {#links}

Os leitores de tela leem os links usando o texto. Se um link for rotulado apenas como &quot;Clique aqui&quot; ou &quot;Leia mais&quot;, os usuários de tecnologias assistivas não saberão o destino. Para garantir a acessibilidade, eles precisam de um texto descritivo que indique claramente o target ou a ação.

Use o Designer de email para adicionar um link ao seu conteúdo e editar o rótulo para torná-lo visível (visível) e descritivo (claro sobre o propósito). Evite rótulos vagos como &quot;aqui&quot; ou &quot;mais&quot;.

<!--![](assets/accessible-link.png){width="70%"}-->

+++Exemplo - bom link (descritivo): 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

Os leitores de tela leem:
&quot;Link, notas de versão de agosto.&quot;

+++

+++Exemplo - Link inválido (não descritivo)

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

Os leitores de tela leem:
&quot;Link, clique aqui.&quot; *(Não fornece contexto fora da ordem de leitura)*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->
