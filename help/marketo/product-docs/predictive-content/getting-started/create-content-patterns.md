---
unique-page-id: 11385579
description: Criar padrões de conteúdo - Documentação do Marketo - Documentação do produto
title: Criar padrões de conteúdo
exl-id: 963529fb-1b30-486c-b97d-3ff697f91258
feature: Predictive Content
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# Criar padrões de conteúdo {#create-content-patterns}

Quando você define padrões de conteúdo, o conteúdo é descoberto automaticamente quando um visitante da Web clica na página da Web do HTML relevante ao padrão de conteúdo. Ele é usado para adicionar páginas do HTML (publicações de blogs, comunicados de imprensa, artigos de notícias) como partes de conteúdo à página Todo o conteúdo. Quando a descoberta automática se baseia em padrões de conteúdo, ela descobre e rastreia páginas do HTML relacionadas ao padrão de URL definido quando um visitante da Web visualiza ou clica em um link para a página. Essa parte do conteúdo (o URL, o nome da página e os metadados, incluindo o URL da imagem e a descrição) é adicionada à página Todo o conteúdo para preparar conteúdo preditivo. Para a descoberta automática de outro conteúdo, como PDFs e vídeo incorporado, você precisa [habilitar a descoberta de conteúdo](/help/marketo/product-docs/predictive-content/getting-started/enable-content-discovery.md).

1. Vá para **[!UICONTROL Configurações de Conteúdo]**.

   ![](assets/settings-dropdown-hand-2.png)

1. Clique em **[!UICONTROL Padrões de URL]**.

   ![](assets/click-url-patterns-hand.png)

1. Clique em **+** para abrir uma linha onde você pode inserir suas informações.

   ![](assets/content-settings-create-patterns-hand.png)

1. Adicione a extensão de URL do domínio onde a página da Web existe. Selecione a categoria (por exemplo, [!UICONTROL Blog], [!UICONTROL Artigo], [!UICONTROL Data Sheet], [!UICONTROL Press Release]).

   ![](assets/content-settings-create-content-patterns-dm-hands.png)

   >[!NOTE]
   >
   >Os itens na lista suspensa à direita refletem as categorias configuradas quando você [criou categorias](/help/marketo/product-docs/predictive-content/getting-started/set-up-categories.md).

1. Clique em **+** para adicionar outro caminho.

   ![](assets/url-patterns-add2.png)

1. Adicione a extensão e a categoria para o caminho adicional e clique em **[!UICONTROL Salvar]**.

   ![](assets/url-patterns-save.png)

## Regras de padrões de conteúdo {#content-pattern-rules}

* Você pode usar um curinga em qualquer lugar em uma expressão (Exemplo: _domain.com/&#42;_, _domain.com/&#42;blog&#42;_)

* Recomendamos usar /&#42; no final de uma expressão para continuar a descoberta de padrões (Exemplo: _domain.com/blog/&#42;_ descobre todas as postagens na pasta Blog)
* Os padrões de conteúdo não diferenciam maiúsculas de minúsculas (Exemplo: _domain.com/Blog/&#42;_ descobre todas as páginas html em _domain.com/Blog_ e _domain.com/blog_)

* Os parâmetros de URL não são descobertos (isso evita descobrir vários itens com o mesmo URL de conteúdo, mas com parâmetros diferentes)

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
   <td><img alt="—" width="80" src="assets/image2017-3-24-10-3a38-3a46.png" data-linked-resource-id="12976559" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11385579" title="--"></td>
   <td><p>Descobre qualquer URL que contenha a palavra "folhas de dados":</p><p>domain.com/datasheets/5-top-tricks</p><p>domain.com/blog/5-top-datasheets</p></td>
  </tr>
  <tr>
   <td>press-release</td>
   <td><p>Somente uma página HTML com correspondência exata é descoberta:</p><p>domain.com/press-release</p></td>
  </tr>
  <tr>
   <td colspan="1"> </td>
   <td colspan="1"><p>Se a expressão do URL estiver vazia, o padrão de URL descobrirá somente a página inicial:</p><p>domínio.com</p></td>
  </tr>
 </tbody>
</table>
