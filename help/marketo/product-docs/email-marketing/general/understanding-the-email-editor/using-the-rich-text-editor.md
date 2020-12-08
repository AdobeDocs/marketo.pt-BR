---
unique-page-id: 2953419
description: Uso do Editor de Rich Text - Documentos do Marketing - Documentação do produto
title: Uso do Editor de Rich Text
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Uso do Editor de Rich Text {#using-the-rich-text-editor}

O Editor de Rich Text (RTE) é exibido em todo o Marketing e está disponível sempre que você deseja adicionar ou editar conteúdo. Você verá uma versão dele no landing page, programas, emails, formulários e trechos. Basta clicar em **Editar rascunho** e ele aparecerá para servir a você.

## Configurações do editor {#editor-settings}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento do bloco raiz de email utiliza <p> tags. Você tem a opção de alterar isso seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher seu elemento de bloco raiz, recomendamos sempre usar as configurações padrão para a melhor experiência do usuário.

1. Clique em **Admin**.

   ![](assets/one.png)

1. Clique em **Email**.

   ![](assets/two.png)

1. Clique em **Editar configurações** do editor de texto.

   ![](assets/three.png)

1. Na lista suspensa **Email / Editor** de fragmentos, selecione <div> ou Nenhum e clique em **Salvar**. <div> é usada neste exemplo.

   ![](assets/four.png)

   Se você tiver <div class="&ldquo;mktEditable&rdquo;"></div> em um modelo de e-mail, você verá o seguinte comportamento de Origem HTML ao abrir a seção e digitar &quot;O texto vai para aqui&quot; no editor:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Nenhum</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;O texto entra aqui&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;O texto entra aqui&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;O<br>texto entra aqui<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Você também pode alterar o elemento de bloco raiz do Editor de Landings page seguindo as mesmas etapas, mas clicando no menu suspenso Editor **de** Landings page na Etapa 4 em vez de Email / Editor de fragmentos.

>[!NOTE]
>
>O elemento de bloco raiz é sempre <p> para tokens de programa Rich Text.

## Recursos {#features}

Estes são os recursos que você encontrará em um RTE.

| Ícone | Nome | O que ele faz |
|---|---|---|
| ![--](assets/image2015-7-9-10-3a23-3a24.png) | Família de fontes | Escolha o seu estilo - temos muito! |
| ![--](assets/image2015-7-9-10-3a22-3a11.png) | Tamanho da fonte | Quão grande você quer? 25 opções, de 8 px a 90 px. |
| ![--](assets/image2015-7-9-10-3a59-3a4.png) | Estilos | Escolha Parágrafo ou seis estilos de cabeçalho (para landing page). |
| ![--](assets/image2015-7-9-10-3a20-3a1.png) | Espaçamento entre linhas | Escolha sua distância entre as linhas. |
| ![--](assets/image2015-7-9-10-3a25-3a52.png) | Cor do texto | Preto, vermelho, ou o que quiser. |
| ![--](assets/image2015-7-9-10-3a24-3a38.png) | Cor do plano de fundo | Realce para realçar. |
| ![--](assets/image2015-7-9-10-3a28-3a4.png) | Negrito | **Mais escuro e mais espesso**. |
| ![--](assets/image2015-7-9-10-3a29-3a1.png) | Itálico | *Inclinado, para ênfase ou* citações. |
| ![--](assets/image2015-7-9-10-3a30-3a56.png) | Sublinhado | Coloca uma linha sob seu texto. |
| ![--](assets/image2015-7-9-10-3a31-3a57.png) | Alinhamento | Use essa lista suspensa para dispor o texto e as imagens. Centralize-os, escolha o alinhamento à esquerda ou à direita ou expanda-o de borda para borda com justificação completa. |  | ![--](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Escolha marcadores ou números na lista suspensa. Os marcadores são bons com listas e números com etapas. |
| ![--](assets/image2015-7-9-10-3a38-3a0.png) | Recuo | Escolha mais ou menos recuo. Use para parágrafos ou qualquer texto que desejar destacar. |
| ![--](assets/image2015-7-9-10-3a38-3a58.png) | Inserir/Editar link | Colocar um link em um site ou outro conteúdo; faça alterações facilmente. |
| ![--](assets/image2015-7-9-10-3a39-3a42.png) | Inserir/Editar imagem | Uma imagem vale mil palavras. Largue um. Clique no ícone da câmera para navegar pelo Design Studio. Você pode soltar imagens lado a lado. |
| ![--](assets/image2015-7-9-10-3a40-3a36.png) | Inserir token | Uma ferramenta poderosa, excelente para personalização de email e rastreamento de dados. Certifique-se de inserir um valor padrão. |
| ![--](assets/image2015-7-9-10-3a41-3a21.png) | Desfazer | Oops! Vamos voltar um passo e tentar de novo. |
| ![--](assets/image2015-7-9-10-3a42-3a13.png) | Refazer | Se estiver tudo bem, volte ao original. |
| ![--](assets/image2015-7-9-10-3a43-3a29.png) | Tabela | Construa o seu, como este. Um menu suspenso permite configurá-lo. |
| ![--](assets/image2015-7-9-10-3a45-3a1.png) | Inserir âncora | Solte a âncora! |
| ![--](assets/image2015-7-9-10-3a45-3a48.png) | Linha horizontal | Muitos usos - Excelente para dividir seções. |
| ![--](assets/image2015-10-6-12-3a12-3a17.png) | Editar HTML | Exibe o Editor de código-fonte HTML para que você possa ajustar seu código. |
| ![--](assets/image2015-7-9-10-3a47-3a36.png) | Subscrito | Letras de baixo deslocamento (como em O`<sub>2</sub>`). |
| ![--](assets/image2015-7-9-10-3a48-3a35.png) | Sobrescrito | Você tem o poder! (2`<sup>6</sup>`). |
| ![--](assets/image2015-7-9-10-3a49-3a31.png) | Tachado | `<s>Put a line through text, like this</s>`. |
| ![--](assets/image2015-7-9-10-3a50-3a11.png) | Caractere especial | Quer falar de euros? Matemática? Você tem 243 escolhas. |
| ![--](assets/image2015-7-9-10-3a52-3a26.png) | Localizar e substituir | Procure e mude as coisas muito mais rápido do que procurar cada instância. |
| ![--](assets/image2015-7-9-10-3a53-3a37.png) | Limpar formatação | Retorne as coisas ao padrão. |
| ![--](assets/image2015-7-9-10-3a55-3a2.png) | Cancelar | Pressione o botão para dizer, &quot;Esqueça.&quot; |
| ![--](assets/image2015-7-9-10-3a56-3a2.png) | Salvar | Pressione o botão para dizer, &quot;OK, eu gosto.&quot; |

>[!TIP]
>
>Você edita seu HTML e texto em telas separadas. Certifique-se de clicar em **Copiar de HTML** na guia **Texto** e em **Salvar** para que o texto corresponda ao seu HTML.

>[!NOTE]
>
>Você não está limitado às fontes no menu suspenso. Você pode usar uma não listada acessando o código HTML. Todas as fontes da Web são suportadas no Marketo, mas as fontes da Web não funcionam universalmente em todos os clientes de email.

## landings page {#landing-pages}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento do bloco raiz da landing page utiliza <div> tags. Você tem a opção de alterar isso seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher seu elemento de bloco raiz, recomendamos sempre usar as configurações padrão para a melhor experiência do usuário.

1. Clique em **Admin**.

   ![](assets/one.png)

1. Clique em **Email**.

   ![](assets/two.png)

1. Clique em **Editar configurações** do editor de texto.

   ![](assets/three.png)

1. Na lista suspensa Editor **de** Landings page, selecione <p> ou Nenhum e clique em **Salvar**. <p> é usada neste exemplo.

   ![](assets/five.png)

   E é isso!

