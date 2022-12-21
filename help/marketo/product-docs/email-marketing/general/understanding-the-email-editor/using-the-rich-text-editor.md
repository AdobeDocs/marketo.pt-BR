---
unique-page-id: 2953419
description: Uso do Editor de Rich Text - Documentos do Marketo - Documentação do produto
title: Uso do Editor de Rich Text
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 5%

---

# Uso do Editor de Rich Text {#using-the-rich-text-editor}

O Editor de Rich Text (RTE) é exibido em todo o Marketo e está disponível sempre que você deseja adicionar ou editar conteúdo. Você verá uma versão dela em landing pages, programas, emails, formulários e trechos. Basta clicar em **Editar rascunho** E vai aparecer para te servir.

## Configurações do editor {#editor-settings}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento de bloco raiz de email usa `<p>` tags. Você tem a opção de alterar isso seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher seu elemento de bloco raiz, sempre recomendamos usar as configurações padrão para a melhor experiência do usuário.

1. Clique em **Administrador**.

   ![](assets/one.png)

1. Clique em **Email**.

   ![](assets/two.png)

1. Clique em **Editar configurações do editor de texto**.

   ![](assets/three.png)

1. No **Editor de email/trecho** , selecione `<div>` ou Nenhum e clique em **Salvar**. `<div>` é usada neste exemplo.

   ![](assets/four.png)

   Se tiver `<div class=“mktEditable”></div>` em um modelo de email, você verá o seguinte comportamento de HTML Source ao abrir a seção e digitar &quot;Text Goes Here&quot; no editor:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Nenhum</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;O texto fica aqui&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;O texto fica aqui&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>O texto fica aqui<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Você também pode alterar o elemento de bloco raiz do Editor de página inicial seguindo as mesmas etapas, mas clicando no botão **Editor de página de aterrissagem** na Etapa 4, em vez do Editor de email/trecho.

>[!NOTE]
>
>O elemento de bloco raiz é sempre `<p>` para tokens de programa rich text.

## Recursos {#features}

Estes são os recursos que você encontrará em um RTE.

| Ícone | Nome | O que ele faz |
|---|---|---|
| ![--](assets/image2015-7-9-10-3a23-3a24.png) | Família de fontes | Escolha o seu estilo, temos muito! |
| ![--](assets/image2015-7-9-10-3a22-3a11.png) | Tamanho da fonte | Quão grande você quer? 25 opções, de 8px a 90px. |
| ![--](assets/image2015-7-9-10-3a59-3a4.png) | Estilos | Escolha os estilos Parágrafo ou Seis Cabeçalhos (para landing pages). |
| ![--](assets/image2015-7-9-10-3a20-3a1.png) | Espaçamento entre linhas | Escolha a distância entre as linhas. |
| ![--](assets/image2015-7-9-10-3a25-3a52.png) | Cor do texto | Preto, vermelho, ou o que quiser. |
| ![--](assets/image2015-7-9-10-3a24-3a38.png) | Cor de fundo | Destaque para ênfase. |
| ![--](assets/image2015-7-9-10-3a28-3a4.png) | Negrito | **Mais escuro e espesso**. |
| ![--](assets/image2015-7-9-10-3a29-3a1.png) | Itálico | *Angular, para ênfase ou cotação* s. |
| ![--](assets/image2015-7-9-10-3a30-3a56.png) | Sublinhado | Coloca uma linha sob o texto. |
| ![--](assets/image2015-7-9-10-3a31-3a57.png) | Alinhamento | Use essa lista suspensa para dispor o texto e as imagens. Centralize-os, escolha o alinhamento à esquerda ou à direita ou expanda-o de ponta a ponta com justificação completa. |  | ![--](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Escolha marcadores ou números na lista suspensa. Os marcadores são bons com listas e números com etapas. |
| ![--](assets/image2015-7-9-10-3a38-3a0.png) | Recuar | Escolha mais ou menos recuo. Use para parágrafos ou qualquer texto que desejar destacar. |
| ![--](assets/image2015-7-9-10-3a38-3a58.png) | Inserir/editar link | Colocar um link em um site ou outro conteúdo; faça alterações facilmente nele. |
| ![--](assets/image2015-7-9-10-3a39-3a42.png) | Inserir/editar imagem | Uma imagem vale mil palavras. Solte um. Clique no ícone da câmera para navegar pelo Design Studio. Você pode soltar imagens lado a lado. |
| ![--](assets/image2015-7-9-10-3a40-3a36.png) | Inserir token | Uma ferramenta poderosa, excelente para personalização de email e rastreamento de dados. Certifique-se de inserir um valor padrão. |
| ![--](assets/image2015-7-9-10-3a41-3a21.png) | Desfazer | Ih! Vamos voltar um passo e tentar de novo. |
| ![--](assets/image2015-7-9-10-3a42-3a13.png) | Refazer | Se estiver muito bem como está, volte ao original. |
| ![--](assets/image2015-7-9-10-3a43-3a29.png) | Tabela | Construa o seu, como este. Um menu suspenso permite configurá-lo. |
| ![--](assets/image2015-7-9-10-3a45-3a1.png) | Inserir âncora | Solte a âncora! |
| ![--](assets/image2015-7-9-10-3a45-3a48.png) | Linha horizontal | Muitos usos - Excelente para divisão de seções. |
| ![--](assets/image2015-10-6-12-3a12-3a17.png) | Editar HTML | Aperte o Editor de fonte HTML para ajustar o código. |
| ![--](assets/image2015-7-9-10-3a47-3a36.png) | Subscrito | Letras com baixo deslocamento (como em O`<sub>2</sub>`). |
| ![--](assets/image2015-7-9-10-3a48-3a35.png) | Sobrescrito | Você tem o poder! (2`<sup>6</sup>`). |
| ![--](assets/image2015-7-9-10-3a49-3a31.png) | Tachado | `<s>Put a line through text, like this</s>`. |
| ![--](assets/image2015-7-9-10-3a50-3a11.png) | Caractere especial | Quer falar de euros? Matemática? Você tem 243 escolhas. |
| ![--](assets/image2015-7-9-10-3a52-3a26.png) | Localizar e substituir | Procure e altere as coisas muito mais rápido do que procurar cada instância por conta própria. |
| ![--](assets/image2015-7-9-10-3a53-3a37.png) | Limpar Formatação | Retorne as coisas para o padrão. |
| ![--](assets/image2015-7-9-10-3a55-3a2.png) | Cancelar | Pressione o botão para dizer, &quot;Esqueça.&quot; |
| ![--](assets/image2015-7-9-10-3a56-3a2.png) | Salvar | Pressione o botão para dizer, &quot;OK, eu gosto.&quot; |

>[!TIP]
>
>Você edita o HTML e o texto em telas separadas. Certifique-se de clicar em **Copiar do HTML** no **Texto** e depois **Salvar** assim, seu texto corresponde ao HTML.

>[!NOTE]
>
>Você não está limitado às fontes no menu suspenso . Você pode usar um não listado acessando o código HTML. Todas as fontes da Web são compatíveis com o Marketo, mas as fontes da Web não funcionam universalmente em todos os clientes de email.

## Páginas {#landing-pages}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento de bloco raiz da página de aterrissagem usa `<div>` tags. Você tem a opção de alterar isso seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher seu elemento de bloco raiz, sempre recomendamos usar as configurações padrão para a melhor experiência do usuário.

1. Clique em **Administrador**.

   ![](assets/one.png)

1. Clique em **Email**.

   ![](assets/two.png)

1. Clique em **Editar configurações do editor de texto**.

   ![](assets/three.png)

1. No **Editor de página de aterrissagem** , selecione `<p>` ou Nenhum e clique em **Salvar**. `<p>` é usada neste exemplo.

   ![](assets/five.png)

   E é isso!
