---
unique-page-id: 2953419
description: Uso do editor de rich text - Documentação do Marketo - Documentação do produto
title: Uso do Editor de Rich Text
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 5%

---

# Uso do Editor de Rich Text {#using-the-rich-text-editor}

O editor de rich text (RTE) é exibido em todo o Marketo e está disponível sempre que você deseja adicionar ou editar conteúdo. Você verá uma versão dele nas landing pages, programas, emails, formulários e trechos. Basta clicar em **Editar Rascunho**, que será exibido para você.

## Configurações do editor {#editor-settings}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento de bloqueio raiz do email usa `<p>` tags. Você tem a opção de alterar isso seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher o elemento de bloco raiz, sempre recomendamos usar as configurações padrão para obter a melhor experiência do usuário.

1. Clique em **Administrador**.

   ![](assets/one.png)

1. Clique em **Email**.

   ![](assets/two.png)

1. Clique em **Editar Configurações do Editor de Texto**.

   ![](assets/three.png)

1. No menu suspenso **Email / Editor de trecho**, selecione `<div>` ou Nenhum e clique em **Salvar**. `<div>` é usado neste exemplo.

   ![](assets/four.png)

   Se você tiver `<div class=“mktEditable”></div>` em um Modelo de email, verá o seguinte comportamento do HTML Source ao abrir a seção e digitar &quot;O texto é inserido aqui&quot; no editor:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Nenhum</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;O texto é inserido aqui&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;O texto é inserido aqui&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="mktEditable"&gt;<br>O texto é inserido aqui<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Você também pode alterar o elemento de bloco raiz do Editor de páginas iniciais seguindo as mesmas etapas, mas clicando no menu suspenso **Editor de páginas iniciais** na Etapa 4 em vez de Email/Editor de trechos.

>[!NOTE]
>
>O elemento de bloco raiz é sempre `<p>` para tokens de programa rich text.

## Recursos {#features}

Estes são os recursos que você encontrará em um RTE.

| Ícone | Nome | O que faz |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Família de fontes | Escolha o seu estilo — temos muito! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Tamanho da fonte | Quão grande você quer? 25 opções, de 8px a 90px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Estilos | Escolha &#39;Parágrafo&#39; ou seis estilos de cabeçalho (para páginas iniciais). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Espaçamento entre linhas | Escolha a distância entre as linhas. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Cor do texto | Preto, vermelho, ou o que quiser. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Cor de fundo | Destaque para ênfase. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Negrito | **Mais escuro e mais grosso**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Itálico | *Angled, para ênfase ou cotação* s. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Sublinhado | Coloca uma linha abaixo do texto. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Alinhamento | Use essa lista suspensa para dispor seu texto e imagens. Centralize-os, escolha o alinhamento à esquerda ou à direita ou espalhe-o de borda a borda com a justificação completa. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Escolha marcadores ou números na lista suspensa. Os marcadores são válidos para listas e números com etapas. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Recuar | Escolha mais ou menos recuo. Use para parágrafos ou qualquer texto que desejar destacar. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Inserir/editar link | Coloque um link para um site ou outro conteúdo; faça alterações facilmente. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Inserir/editar imagem | Uma imagem vale mais do que mil palavras. Solte um em. Clique no ícone de câmera para navegar no Design Studio. Você pode colocar imagens lado a lado. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Inserir token | Uma ferramenta eficiente, ideal para personalização de email e rastreamento de dados. Insira um valor padrão. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Desfazer | Ih! Vamos voltar uma etapa e tentar novamente. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Refazer | Se estiver tudo bem, retorne ao original. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Tabela | Construa o seu, como este aqui. Um menu suspenso permite configurá-lo. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Inserir Âncora | Solte a âncora! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Linha horizontal | Muitos usos - Ótimo para dividir seções. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | Editar HTML | Exibe o Editor de Source do HTML para que você possa ajustar seu código. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Subscrito | Letras baixas (como em O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Sobrescrito | Você tem o poder! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Tachado | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Caractere especial | Quer falar sobre euros? Matemática? Você tem 243 opções. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Localizar e substituir | Pesquise e altere as coisas com muito mais rapidez do que procurar cada instância por si mesmo. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Limpar Formatação | Devolva as coisas ao padrão. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Cancelar | Pressione o botão para dizer: &quot;Não importa.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Salvar | Pressione o botão para dizer: &quot;OK, eu gostei.&quot; |

>[!TIP]
>
>Você edita seu HTML e texto em telas separadas. Certifique-se de clicar em **Copiar do HTML** na guia **Texto** e em **Salvar** para que o texto corresponda ao HTML.

>[!NOTE]
>
>Você não está limitado às fontes no menu suspenso. Você pode usar um não listado acessando o código HTML. Todas as fontes da Web são compatíveis com o Marketo, mas as fontes da Web não funcionam universalmente em todos os clientes de email.

## Páginas de aterrissagem {#landing-pages}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento de bloco raiz da página de aterrissagem usa `<div>` tags. Você tem a opção de alterar isso, seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher o elemento de bloco raiz, sempre recomendamos usar as configurações padrão para obter a melhor experiência do usuário.

1. Clique em **Administrador**.

   ![](assets/one.png)

1. Clique em **Email**.

   ![](assets/two.png)

1. Clique em **Editar Configurações do Editor de Texto**.

   ![](assets/three.png)

1. No menu suspenso **Editor de Landing Page**, selecione `<p>` ou Nenhum e clique em **Salvar**. `<p>` é usado neste exemplo.

   ![](assets/five.png)

   E é isso!
