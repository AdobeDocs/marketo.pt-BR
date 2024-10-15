---
description: Modelos de email - Documentação do Marketo - Documentação do produto
title: Modelos de e-mail
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 28bc524ac651a2a9516888b11acb226725689869
workflow-type: tm+mt
source-wordcount: '1411'
ht-degree: 1%

---

# Modelos de e-mail {#email-templates}

Texto de introdução aqui.

>[!IMPORTANT]
>
>Este artigo é destinado apenas aos membros do New Marketo Engage Email Editor beta. Por favor, não difunda.

>[!NOTE]
>
>Os modelos de email no novo editor de email só podem ser usados para criar emails no novo editor de email. Eles não podem ser referenciados no editor de email antigo.

## Criar um modelo de email {#create-an-email-template}

1. Faça logon no Marketo Engage por meio da [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. Em Meu Marketo, selecione **Design Studio**.

   ![](assets/create-an-email-template-1.png)

1. Na árvore, selecione **Modelos de email (Novo editor)**.

   ![](assets/create-an-email-template-2.png)

1. Clique no botão **Criar modelo**.

   ![](assets/create-an-email-template-3.png)

1. Insira um nome de template e uma descrição opcional. Clique em **Criar**.

   ![](assets/create-an-email-template-4.png)

## Criar seu modelo {#design-your-template}

Na página _Criar seu modelo_, você pode escolher entre algumas opções. [Criar do zero](#design-from-scratch), [importar seu próprio HTML](#import-html) ou [selecionar um modelo existente](#choose-a-template) (uma de nossas amostras ou uma que você já salvou).

### Criar do zero {#design-from-scratch}

Defina o conteúdo adicionando e movendo elementos estruturais com ações simples de arrastar e soltar.

1. Na página _Criar seu modelo_, selecione **Criar do zero**.

   CAPTURA DE TELA

1. Adicionar [estrutura e conteúdo](#add-structure-and-content).

### Importar seu HTML {#import-your-html}

Você pode importar conteúdo de HTML existente para criar seus modelos de email. O conteúdo pode ser:

* Um arquivo HTML com uma folha de estilos incorporada

* Um arquivo .zip que inclui um arquivo HTML, a folha de estilos (.css) e as imagens

>[!NOTE]
>
>Não há restrições na estrutura do arquivo .zip. No entanto, as referências devem ser relativas e se encaixar na estrutura de árvore da pasta .zip.

1. Na página _Criar seu modelo_, selecione **Importar HTML**.

   CAPTURA DE TELA

1. Arraste e solte o arquivo de HTML ou .zip desejado e clique em **Importar**.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >Quando o conteúdo em HTML for carregado, o conteúdo estará no modo Compatibilidade. Nesse modo, você só pode personalizar seu texto, adicionar links ou adicionar ativos ao seu conteúdo.

1. Para aproveitar os componentes de conteúdo do Email Designer, clique na guia **HTML converter** e clique em **Converter**.

   CAPTURA DE TELA

   >[!CAUTION]
   >
   >Usar uma marca `<table>` como a primeira camada em um arquivo de HTML pode causar perda de estilo, incluindo configurações de plano de fundo e largura na marca de camada superior.

Agora você pode personalizar o arquivo importado, conforme necessário, com o editor visual de email.

### Escolher um modelo {#choose-a-template}

Há dois tipos de modelos para escolher.

* Modelos de exemplo: o Marketo Engage oferece quatro modelos de email prontos para uso.

* Modelos salvos: são modelos criados do zero usando o menu Modelos ou um email que você criou e optou por salvar como modelo.

>[!BEGINTABS]

>[!TAB Modelos de exemplo]

Escolha um dos quatro modelos prontos para uso para um head start no design do modelo de email.

1. Selecione Modelos de amostra.

   CAPTURA DE TELA

1. Texto.

   CAPTURA DE TELA

>[!TAB Modelos salvos]

1. Selecione Modelos salvos.

   CAPTURA DE TELA

1. Texto.

   CAPTURA DE TELA

>[!ENDTABS]

## Adicionar estrutura e conteúdo {#add-structure-and-content}

1. Para começar a criar ou modificar conteúdo, arraste e solte um item de Estruturas na tela. Edite suas configurações no painel à direita.

   >[!TIP]
   >
   >Selecione o componente de coluna n:n para definir o número de colunas de sua escolha (entre três e 10). Você também pode definir a largura de cada coluna movendo as setas abaixo dela.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >Cada tamanho de coluna não pode ser menor que 10% da largura total do componente de estrutura. Somente colunas vazias podem ser removidas.

1. Na seção Conteúdo, arraste sobre os itens desejados e solte-os em um ou mais componentes da estrutura.

   CAPTURA DE TELA

1. Cada componente pode ser personalizado por meio das guias Configurações ou Estilo. Altere a fonte, o estilo do texto, a margem e muito mais.

CAPTURA DE TELA

### Adicionar o Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY?
```

1. Para acessar suas imagens, clique no ícone Seletor de ativos.

   CAPTURA DE TELA

1. Arraste e solte a imagem desejada em um componente de estrutura.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >Para substituir uma imagem existente, selecione-a e clique em **Selecionar um ativo** na guia Configurações à direita.

Clique em Ativar conteúdo de condição para adicionar conteúdo dinâmico e adaptar o conteúdo aos perfis direcionados com base em regras condicionais.



Se necessário, você pode personalizar ainda mais seu email clicando em Alternar para o editor de código no menu avançado. Isso permite editar o código fonte do email, por exemplo, para adicionar tags de rastreamento ou HTML personalizadas.

CUIDADO
Você não pode reverter para o designer visual neste email depois de alternar para o editor de código.

Quando o conteúdo estiver pronto, clique no botão Simular conteúdo para verificar a renderização. Você pode escolher a visualização de desktop ou móvel.

Quando estiver pronto, clique em Salvar

### Camadas, configurações e estilos {#layers-settings-styles}

```
ARE THEY CALLED LAYERS OR COMPONENTS
```

Abra a árvore de navegação para acessar estruturas específicas e suas colunas/componentes para uma edição mais granular.

1. Para acessar o, clique no ícone da Árvore de navegação.

CAPTURA DE TELA




### Personalizar conteúdo {#personalize-content}

Os tokens funcionam no novo editor da mesma forma que no antigo, mas o ícone é diferente.

1. Selecione o componente de texto e clique no ícone **Adicionar personalização**.

   CAPTURA DE TELA

1. Clique no [tipo de token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} desejado.

   CAPTURA DE TELA

1. Clique em + ou ... para adicionar um token ao espaço em branco.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >&quot;Texto de fallback&quot; é o novo termo do editor para o valor padrão. Exemplo: ``{{lead.First Name:default=Friend}}``

1. Clique em **Salvar** quando terminar.

### Editar rastreamento de URL {#edit-url-tracking}

Às vezes, você não quer ativar o URL de rastreamento do Marketo em um link em um email. Isso é útil quando a página de destino não suporta parâmetros de URL e pode resultar em um link quebrado.

1. Clique no ícone Links para exibir todos os URLs do email.

   CAPTURA DE TELA

1. Clique no ícone de lápis para editar o rastreamento dos links desejados.

   CAPTURA DE TELA

   ```
   LABEL?
   
   TAGS?
   ```

   <table><tbody>
     <tr>
       <td><b>Rastrear sem mkt_tok</b></td>
       <td>definição</td>
     </tr>
     <tr>
       <td><b>Rastrear com mkt_tok</b></td>
       <td>definição</td>
     </tr>
     <tr>
       <td><b>Não rastrear</b></td>
       <td>definição</td>
     </tr>
   </tbody>
   </table>

1. Clique em **Salvar** quando terminar.

### Exibir opções {#view-options}

Aproveite as opções de exibição e validação de conteúdo disponíveis no editor visual de email.

* Aumente/diminua o zoom do conteúdo usando as opções de zoom predefinidas.

* Visualizar o conteúdo na área de trabalho, dispositivo móvel ou somente texto/texto simples.

   * Clique no ícone de exibição em tempo real (olho) para pré-visualização de conteúdo em todos os dispositivos.

   * Selecione um dos dispositivos prontos para uso ou insira dimensões personalizadas para visualizar seu conteúdo.

### Mais opções {#more-options}

Nas opções **Mais** do editor de conteúdo, você pode realizar as seguintes ações:

CAPTURA DE TELA

* **Redefinir modelo**: selecione essa opção para limpar a tela do designer de email visual em branco e reiniciar a criação de conteúdo.

* **Alterar seu design**: volte para a página _Criar seu modelo_. Aqui, você pode executar qualquer ação descrita na seção [Criar seu modelo](#design-your-template).

* **Exportar HTML**: baixe o conteúdo na tela visual para o sistema local no formato HTML empacotado como um arquivo zip.

## Exibir detalhes do modelo {#view-template-details}

Na página de listagem _Modelos de email_, clique no nome de um modelo de email para exibir seus detalhes.

CAPTURA DE TELA

Detalhes básicos como nome e descrição podem ser editados. Clique fora do campo que você editou para salvar suas alterações.

Clique em **Mais** para excluir ou duplicar rapidamente seu modelo.

Se houver alertas ativos (erros/avisos para o modelo de email), clique em Alertas para exibir as informações.

>[!NOTE]
>
>Embora esses alertas não proíbam o uso do modelo de email para criação de email, as informações fornecem visibilidade sobre o que pode não funcionar e as atualizações necessárias antes que o email possa ser usado para a entrega.

## Exibir modelo de email usado por referências {#email-template-used-by-references}

No resumo do modelo de email, clique na guia **Usado por** para exibir detalhes sobre onde esse modelo de email foi usado no Marketo Engage.

CAPTURA DE TELA

## Editar modelos de email {#edit-email-templates}

Esta ação pode ser tomada a partir de:

* Na guia de detalhes - Clique em **Editar modelo de email**.

* Página de listagem _Modelos de email_ - Clique no ícone Mais ações (três pontos) do modelo de email desejado e escolha Editar.

```
THE SECOND ONE DOESN'T WORK IN MARKETO?? JUST LISTS DUPE AND DELETE
```

Esta ação direciona você à página _Criar modelo_ ou à página do editor de conteúdo visual com base no último status salvo do modelo de email. Aqui, você pode editar o conteúdo do seu modelo de email conforme necessário. Consulte Criar modelos de email para obter informações sobre as opções de edição.

## Modelos de email duplicados {#duplicate-email-templates}

Há duas maneiras de duplicar um template de email:

* Nos detalhes do modelo de email à direita, clique em **Mais** e selecione **Duplicar**.

CAPTURA DE TELA

* Na página de listagem _Modelos de email_, clique no ícone Mais ações (três pontos) do modelo de email desejado e escolha **Duplicar**.

Na caixa de diálogo, digite um nome exclusivo e uma descrição opcional. Clique em **Duplicar** quando terminar.

O modelo de email duplicado aparece na página de listagem _Modelos de email_.

## Excluir modelos de email {#delete-email-templates}

Há duas maneiras de excluir um template de email.

>[!CAUTION]
>
>A exclusão de um modelo de email não pode ser desfeita.

* Nos detalhes do modelo de email à direita, clique em **Mais** e selecione **Excluir**.

CAPTURA DE TELA

* Na página de listagem _Modelos de email_, clique no ícone Mais ações (três pontos) do modelo de email desejado e escolha **Excluir**.

## Ações em massa {#bulk-actions}

Na página de listagem _Modelos de email_, selecione vários modelos marcando as caixas de seleção à esquerda. Um banner é exibido na parte inferior.

**Excluir**: é possível excluir no máximo 20 modelos de cada vez. Uma caixa de diálogo de confirmação permite suspender a ação ou confirmar a exclusão.

>[!MORELIKETHIS]
>
>[Criação de email](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-authoring.md){target="_blank"}: saiba como criar, projetar e fazer referência a um email no novo editor.
