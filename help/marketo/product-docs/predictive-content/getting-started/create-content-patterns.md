---
unique-page-id: 11385579
description: Criar padrões de conteúdo - Documentos do marketing - Documentação do produto
title: Criar padrões de conteúdo
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---


# Criar padrões de conteúdo {#create-content-patterns}

Quando você define padrões de conteúdo, o conteúdo é detectado automaticamente quando um visitante da Web clica na página da Web HTML relevante para o padrão de conteúdo. É usado para adicionar páginas HTML (publicações em blog, comunicados à imprensa, artigos de notícias) como partes de conteúdo à página Todo conteúdo. Quando a descoberta automática é baseada em padrões de conteúdo, ela descobre e rastreia páginas HTML que estão relacionadas ao padrão de URL definido quando um visitante da Web visualização ou clica em um link para a página. Esse conteúdo (o URL, o nome da página e os metadados - incluindo o URL da imagem e a descrição) é adicionado à página Todo o conteúdo para preparar o conteúdo preditivo. Para descobrir automaticamente outro conteúdo, como PDFs e vídeo incorporado, é necessário [ativar a descoberta de conteúdo](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vá para **Configurações de conteúdo**.

   ![](assets/settings-dropdown-hand-2.png)

1. Clique em **Padrões de URL**.

   ![](assets/click-url-patterns-hand.png)

1. Clique em **+** para abrir uma linha na qual você pode inserir suas informações.

   ![](assets/content-settings-create-patterns-hand.png)

1. Adicione a extensão de URL do domínio em que a página da Web existe. Selecione a categoria (por exemplo, Blog, Artigo, Data Sheet, Comunicado à imprensa).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Os itens na lista suspensa à direita refletem as categorias que você configurou ao [criar categoria](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Clique em **+** para adicionar outro caminho.

   ![](assets/url-patterns-add2.png)

1. Adicione a extensão e a categoria do caminho adicional e clique em **Salvar**.

   ![](assets/url-patterns-save.png)

## Regras de padrão de conteúdo {#content-pattern-rules}

* Você pode usar um curinga em qualquer lugar em uma expressão (exemplo: _domain.com/*_, _domain.com/*blog*_)

* Recomendamos usar /* no final de uma expressão para continuar a descoberta de padrões (Exemplo: _domain.com/blog/*_ descobre todas as publicações na pasta Blog)
* Os padrões de conteúdo não distinguem maiúsculas de minúsculas (exemplo: _domain.com/Blog/*_ descobre todas as páginas html em _domain.com/Blog_ e _domain.com/blog_)

* Parâmetros de URL não são detectados (isso evita descobrir vários itens com o mesmo URL de conteúdo, mas parâmetros diferentes)

## Exemplos {#examples}

Para _domain.com_:

<table> 
 <tbody> 
  <tr> 
   <th>Padrão de URL</th> 
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
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="—"></td> 
   <td><p>Descobre qualquer URL que contenha a palavra "fichas técnicas:"</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td> 
  </tr> 
  <tr> 
   <td>comunicado de imprensa</td> 
   <td><p>Apenas uma página HTML de correspondência exata é descoberta:</p><p>domain.com/press-release</p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> </td> 
   <td colspan="1"><p>Se a expressão de URL estiver vazia, o padrão de URL detectará apenas o home page:</p><p>domain.com</p></td> 
  </tr> 
 </tbody> 
</table>
