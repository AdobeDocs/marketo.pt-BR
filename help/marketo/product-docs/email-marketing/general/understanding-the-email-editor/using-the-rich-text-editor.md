---
unique-page-id: 2953419
description: Uso do editor de rich text - Documentação do Marketo - Documentação do produto
title: Uso do Editor de Rich Text
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Uso do Editor de Rich Text {#using-the-rich-text-editor}

O editor de rich text (RTE) é exibido em todo o Marketo e está disponível sempre que você deseja adicionar ou editar conteúdo. Você verá uma versão dele nas landing pages, programas, emails, formulários e trechos. Basta clicar em **[!UICONTROL Editar Rascunho]**, que será exibido para você.

## Configurações do editor {#editor-settings}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento de bloqueio raiz do email usa `<p>` tags. Você tem a opção de alterar isso seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher o elemento de bloco raiz, sempre recomendamos usar as configurações padrão para obter a melhor experiência do usuário.

1. Clique em **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Clique em **[!UICONTROL Editar Configurações do Editor de Texto]**.

   ![](assets/three.png)

1. No menu suspenso **[!UICONTROL Email] / [!UICONTROL Editor de Trechos]**, selecione `<div>` ou [!UICONTROL Nenhum] e clique em **[!UICONTROL Salvar]**. `<div>` é usado neste exemplo.

   ![](assets/four.png)

   Se você tiver `<div class=“mktEditable”></div>` em um Modelo de email, verá o seguinte comportamento do HTML Source ao abrir a seção e digitar &quot;O texto vai aqui&quot; no editor:

<table>
 <tbody>
  <tr>
   <th>&lt;p&gt;</th>
   <th>&lt;div&gt;</th>
   <th>None</th>
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
>Você também pode alterar o elemento de bloco raiz do Editor de página de aterrissagem seguindo as mesmas etapas, mas clicando no menu suspenso **[!UICONTROL Editor de página de aterrissagem]** na Etapa 4 em vez de [!UICONTROL Email] / [!UICONTROL Editor de trechos].

>[!NOTE]
>
>O elemento de bloco raiz é sempre `<p>` para tokens de programa rich text.

## Recursos {#features}

Estes são os recursos que você encontrará em um RTE.

| Ícone | Nome | O que faz |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Família da fonte] | Escolha o seu estilo — temos muito! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Tamanho da Fonte] | Quão grande você quer? 25 opções, de 8px a 90px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL Estilos] | Escolha &#39;Parágrafo&#39; ou seis estilos de cabeçalho (para páginas iniciais). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Espaçamento entre linhas] | Escolha a distância entre as linhas. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Cor do texto] | Preto, vermelho, ou o que quiser. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL Cor do Plano de Fundo] | Destaque para ênfase. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Negrito] | **Mais escuro e mais grosso**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Itálico] | *Angled, para ênfase ou cotação* s. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Sublinhado] | Coloca uma linha abaixo do texto. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Alinhamento] | Use essa lista suspensa para dispor seu texto e imagens. Centralize-os, escolha o alinhamento à esquerda ou à direita ou espalhe-o de borda a borda com a justificação completa. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Lista | Escolha marcadores ou números na lista suspensa. Os marcadores são válidos para listas e números com etapas. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Recuo] | Escolha mais ou menos recuo. Use para parágrafos ou qualquer texto que desejar destacar. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Inserir/Editar Link] | Coloque um link para um site ou outro conteúdo; faça alterações facilmente. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Inserir/Editar Imagem] | Uma imagem vale mais do que mil palavras. Solte um em. Clique no ícone de câmera para navegar no Design Studio. Você pode colocar imagens lado a lado. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Inserir token] | Uma ferramenta eficiente, ideal para personalização de email e rastreamento de dados. Insira um valor padrão. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL Desfazer] | Ih! Vamos voltar uma etapa e tentar novamente. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Refazer] | Se estiver tudo bem, retorne ao original. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Tabela] | Construa o seu, como este aqui. Um menu suspenso permite configurá-lo. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Inserir Âncora] | Solte a âncora! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Linha horizontal] | Muitos usos - Ótimo para dividir seções. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL Editar HTML] | Exibe o Editor Source do HTML para que você possa ajustar seu código. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Subscrito] | Letras baixas (como em O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Sobrescrito] | Você tem o poder! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Tachado] | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Caractere especial] | Quer falar sobre euros? Matemática? Você tem 243 opções. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Localizar e Substituir] | Pesquise e altere as coisas com muito mais rapidez do que procurar cada instância por si mesmo. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Limpar Formatação] | Devolva as coisas ao padrão. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Cancelar] | Pressione o botão para dizer: &quot;Não importa.&quot; |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Salvar] | Pressione o botão para dizer: &quot;OK, eu gostei.&quot; |

>[!TIP]
>
>Você edita seu HTML e texto em telas separadas. Certifique-se de clicar em **[!UICONTROL Copiar do HTML]** na guia **[!UICONTROL Texto]** e em **[!UICONTROL Salvar]** para que o texto corresponda ao seu HTML.

>[!NOTE]
>
>Você não está limitado às fontes no menu suspenso. Você pode usar um não listado acessando o código HTML. Todas as fontes da Web são compatíveis com o Marketo, mas as fontes da Web não funcionam universalmente em todos os clientes de email.

## Páginas de aterrissagem {#landing-pages}

A configuração do elemento de bloco raiz define quais tags vinculam seu conteúdo. Por padrão, o elemento de bloco raiz da página de aterrissagem usa `<div>` tags. Você tem a opção de alterar isso, seguindo as etapas abaixo.

>[!TIP]
>
>Embora você tenha a opção de escolher o elemento de bloco raiz, sempre recomendamos usar as configurações padrão para obter a melhor experiência do usuário.

1. Clique em **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Clique em **[!UICONTROL Editar Configurações do Editor de Texto]**.

   ![](assets/three.png)

1. No menu suspenso **[!UICONTROL Editor de Landing Page]**, selecione `<p>` ou [!UICONTROL Nenhum] e clique em **[!UICONTROL Salvar]**. `<p>` é usado neste exemplo.

   ![](assets/five.png)

   E é isso!
