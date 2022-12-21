---
unique-page-id: 11385579
description: Criar padrões de conteúdo - Documentos do Marketo - Documentação do produto
title: Criar padrões de conteúdo
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 2%

---

# Criar padrões de conteúdo {#create-content-patterns}

Quando você define padrões de conteúdo, o conteúdo é descoberto automaticamente quando um visitante da Web clica na página da Web do HTML relevante para o padrão de conteúdo. É usado para adicionar HTML pages (posts de blogues, comunicados de imprensa, artigos de notícias) como partes de conteúdo à página Todo o conteúdo . Quando a descoberta automática é baseada em padrões de conteúdo, ela descobre e rastreia HTML páginas relacionadas ao padrão de URL definido quando um visitante da Web exibe ou clica em um link para a página. Esse conteúdo (o URL, o nome da página e os metadados, incluindo o URL da imagem e a descrição) é adicionado à página Todo o conteúdo para preparar o conteúdo preditivo. Para descobrir automaticamente outro conteúdo, como PDF e vídeo incorporado, é necessário [ativar a descoberta de conteúdo](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Ir para **Configurações de conteúdo**.

   ![](assets/settings-dropdown-hand-2.png)

1. Clique em **Padrões de URL**.

   ![](assets/click-url-patterns-hand.png)

1. Clique no botão **+** para abrir uma linha onde você pode inserir suas informações.

   ![](assets/content-settings-create-patterns-hand.png)

1. Adicione a extensão de URL do domínio em que a página da Web existe. Selecione a categoria (por exemplo, Blog, Artigo, Data Sheet, Comunicado de imprensa).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Os itens na lista suspensa à direita refletem as categorias que você configurou ao [categorias criadas](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Clique em **+** para adicionar outro caminho.

   ![](assets/url-patterns-add2.png)

1. Adicione a extensão e a categoria do caminho adicional e clique em **Salvar**.

   ![](assets/url-patterns-save.png)

## Regras de padrão de conteúdo {#content-pattern-rules}

* Você pode usar um curinga em qualquer lugar em uma expressão (Exemplo: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Recomendamos usar /&#42; no final de uma expressão para continuar a descoberta de padrões (Exemplo: _domain.com/blog/&#42;_ descobre todas as publicações na pasta Blog)
* Os padrões de conteúdo não fazem distinção entre maiúsculas e minúsculas (Exemplo: _domain.com/Blog/&#42;_ descobre todas as páginas html em _domain.com/Blog_ e _domain.com/blog_)

* Os parâmetros de URL não são descobertos (isso evita descobrir vários itens com o mesmo URL de conteúdo, mas diferentes parâmetros)

## Exemplos {#examples}

Para _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>Padrão do URL</th> 
   <th>Resultado</th> 
  </tr> 
  <tr> 
   <td>blog/*</td> 
   <td><p>Descobre todo o conteúdo que corresponde ao padrão domain.com/blog/:</p><p>domain.com/blog/5-top-tricks</p><p>domain.com/blog/2017/new-year-solutions</p><p>domain.com/Blog/3-best-recipes</p></td> 
  </tr> 
  <tr> 
   <td>artigo/2017/*</td> 
   <td><p>Descobre todo o conteúdo que corresponde ao padrão domain.com/article/2017/:</p><p>domain.com/article/2017/5-top-tricks</p></td> 
  </tr> 
  <tr> 
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td> 
   <td><p>Descobre qualquer URL que contenha a palavra "fichas técnicas":</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>comunicado de imprensa</td> 
   <td><p>Apenas uma página de HTML de correspondência exata é descoberta:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Se a expressão do URL estiver vazia, o padrão do URL descobrirá somente a página inicial:</p><p>domínio.com</p></td> 
  </tr> 
 </tbody> 
</table>
