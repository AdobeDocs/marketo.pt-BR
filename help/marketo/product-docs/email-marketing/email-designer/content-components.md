---
solution: Marketo Engage
product: marketo
title: Componentes do conteúdo
description: DESCRIÇÃO.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: ca8644c43cfbdbaf7be9f21c5e440949b796cfdb
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# Componentes do conteúdo {#content-components}

Ao criar seu conteúdo de email, os **[!UICONTROL Componentes de conteúdo]** permitem personalizar ainda mais seu email com componentes brutos que podem ser editados depois de colocados no email.

É possível adicionar quantos componentes de conteúdo forem necessários dentro de um ou mais componentes de estrutura, que definem o layout do seu email.

## Adicionar componentes de conteúdo {#add-content-components}

Para adicionar componentes de conteúdo ao seu email e ajustá-los às suas necessidades, siga as etapas abaixo.

1. No Designer de email, use um conteúdo existente ou arraste e solte **[!UICONTROL Componentes da estrutura]** no seu conteúdo vazio para definir o layout do seu email. `[Learn how](content-from-scratch.md)`

1. Para acessar a seção **[!UICONTROL Componentes de conteúdo]**, selecione o botão correspondente no painel esquerdo do Designer de email.

   CAPTURA DE TELA

1. Arraste e solte os componentes de conteúdo de sua escolha dentro dos componentes de estrutura relevantes.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >É possível adicionar vários componentes em um único componente de estrutura e em cada coluna de um componente de estrutura.

1. Ajuste os atributos e o estilo de cada componente usando as guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilo]** à direita. Por exemplo, é possível alterar o estilo do texto, o preenchimento ou a margem de cada componente. `[Learn more about alignment and padding](alignment-and-padding.md)`

   CAPTURA DE TELA

1. No menu avançado do seu **[!UICONTROL Componente de conteúdo]**, você pode excluir ou duplicar facilmente qualquer componente de conteúdo, conforme necessário.

   CAPTURA DE TELA

## Container {#container}

Para aplicar um estilo específico a um grupo de componentes de conteúdo, você pode adicionar um componente **[!UICONTROL Contêiner]** e depois adicionar o(s) componente(s) de conteúdo desejado(s) dentro dele. Isso permite aplicar um estilo distinto ao contêiner, que será diferente do estilo aplicado aos componentes de conteúdo dentro dele.

Por exemplo, adicione um componente **[!UICONTROL Contêiner]** e adicione um componente [Botão](#button) dentro desse contêiner. Você pode usar um plano de fundo específico para o contêiner e outro para o botão.

CAPTURA DE TELA

## Botão {#button}

Use o componente **[!UICONTROL Botão]** para inserir um ou vários botões no email e redirecionar o público-alvo de email para outra página.

1. Em **[!UICONTROL Componentes do conteúdo]**, arraste e solte o componente **[!UICONTROL Botão]** em um **[!UICONTROL componente de Estrutura]**.

1. Clique no botão recém-adicionado para personalizar o texto e ter acesso às guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilos]** no painel direito do Email Designer.

   CAPTURA DE TELA

1. No menu **[!UICONTROL Link]**, adicione a URL para a qual você deseja redirecionar ao clicar no botão.

1. Escolha como o público será redirecionado com a lista suspensa **[!UICONTROL Target]**:

   * **[!UICONTROL Nenhum]**: abre o link no mesmo quadro em que foi clicado (padrão).
   * **[!UICONTROL Em branco]**: abre o link em uma nova janela ou guia.
   * **[!UICONTROL Self]**: abre o link no mesmo quadro em que foi clicado.
   * **[!UICONTROL Pai]**: abre o link no quadro pai.
   * **[!UICONTROL Superior]**: abre o link no corpo inteiro da janela.

   CAPTURA DE TELA

1. Você pode personalizar ainda mais seu botão alterando atributos de estilo como **[!UICONTROL Borda]**, **[!UICONTROL Tamanho]**, **[!UICONTROL Margem]**, etc. do painel **[!UICONTROL Configurações de componente]**.

## Texto {#text}

Use o componente **[!UICONTROL Texto]** para inserir texto no email e ajustar o estilo (borda, tamanho, preenchimento etc.) usando a guia **[!UICONTROL Estilos]**.

CAPTURA DE TELA

1. Em **[!UICONTROL Componentes do conteúdo]**, arraste e solte o componente **[!UICONTROL Texto]** em um **[!UICONTROL componente de Estrutura]**.

1. Clique no componente recém-adicionado para personalizar o texto e ter acesso às guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilos]** no painel direito do Designer de email.

1. Altere o texto com as seguintes opções disponíveis na barra de ferramentas:

   CAPTURA DE TELA

   * **[!UICONTROL Alterar estilo do texto]**: aplique negrito, itálico, sublinhado ou tachado ao texto.
   * **Alterar alinhamento**: escolha entre alinhamento à esquerda, à direita, centralizado ou justificado para o texto.
   * **[!UICONTROL Criar lista]**: adicionar lista de marcadores ou números ao texto.
   * **[!UICONTROL Definir cabeçalho]**: adicione até seis níveis de cabeçalho ao texto.
   * **Tamanho da fonte**: selecione o tamanho da fonte do texto em pixels.
   * **[!UICONTROL Alterar cor da fonte]**: escolha a cor da fonte.
   * **[!UICONTROL Inserir link]**: adicione qualquer tipo de link ao seu conteúdo.
   * **[!UICONTROL Editar imagem]**: adicione uma imagem ou um ativo ao seu componente de texto. `[Learn more about asset management](../integrations/assets.md)`
   * **[!UICONTROL Alterar cor da fonte]**: escolha a cor da fonte.
   * **[!UICONTROL Adicionar personalização]**: adicione campos de personalização para personalizar o conteúdo dos dados de seus perfis. `[Learn more about content personalization](../personalization/personalize.md)`
   * **[!UICONTROL Mostrar o código-fonte]**: exibir o código-fonte do texto. Ele não pode ser modificado.
   * **[!UICONTROL Habilitar conteúdo condicional]**: adicione conteúdo condicional para adaptar o conteúdo do componente aos perfis direcionados. `[Learn more about dynamic content](../personalization/get-started-dynamic-content.md)`
   * **[!UICONTROL Duplicar]**: adicione uma cópia do componente de texto.
   * **[!UICONTROL Excluir]**: exclui o componente de texto selecionado do seu email.

1. Ajuste os outros atributos de estilo, como cor do texto, família da fonte, borda, preenchimento, margem, etc. na guia **[!UICONTROL Estilos]**.

   CAPTURA DE TELA

## Divisor {#divider}

Use o componente **[!UICONTROL Divider]** para inserir uma linha divisória para organizar o layout e o conteúdo do seu email.

É possível ajustar atributos de estilo, como cor, estilo e altura da linha, nas guias **[!UICONTROL Configurações]** e **[!UICONTROL Estilos]**.

CAPTURA DE TELA

## HTML {#HTML}

Use o componente **[!UICONTROL HTML]** para copiar e colar as diferentes partes do HTML existente. Isso permite criar componentes modulares gratuitos do HTML para reutilizar algum conteúdo externo.

1. Em **[!UICONTROL Componentes do Conteúdo]**, arraste e solte o componente **[!UICONTROL HTML]** em um **[!UICONTROL componente de Estrutura]**.

1. Clique no componente recém-adicionado e selecione **[!UICONTROL Mostrar o código-fonte]** na barra de ferramentas contextual para adicionar seu HTML.

   CAPTURA DE TELA

1. Copie e cole o código HTML que deseja adicionar ao seu email e clique em **[!UICONTROL Salvar]**.

   CAPTURA DE TELA

>[!NOTE]
>
>Para simplesmente tornar um conteúdo externo compatível com o Email Designer, a Adobe recomenda criar uma mensagem do zero e copiar o conteúdo do seu email existente para os componentes.

## Imagem {#image}

Use o componente **[!UICONTROL Imagem]** para inserir um arquivo de imagem do seu computador no conteúdo de email.

1. Em **[!UICONTROL Componentes do conteúdo]**, arraste e solte o componente **[!UICONTROL Imagem]** em um **[!UICONTROL componente de Estrutura]**.

   CAPTURA DE TELA

1. Na guia **[!UICONTROL Configurações]**, clique em **[!UICONTROL Procurar]** para escolher um arquivo de imagem de seus ativos ou em **[!UICONTROL Importar mídia]** para carregar um ativo para a Adobe Experience Manager Assets.

   Para saber mais sobre [!DNL Adobe Experience Manager Assets], consulte a [documentação do Adobe Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-assets-essentials/help/introduction.html){target="_blank"}.

   >[!NOTE]
   >
   > Para garantir que seus links permaneçam ativos e evitar problemas de expiração, recomendamos usar o Adobe Assets em vez de depender de um URL de origem para suas imagens.

1. Você também pode pesquisar diretamente no Adobe Stock com a opção **[!UICONTROL Localizar fotos do Adobe Stock]**.

1. Clique no componente recém-adicionado e configure as propriedades da imagem:

   * **[!UICONTROL O título da imagem]** permite definir um título para a imagem.
   * **[!UICONTROL O texto alternativo]** permite definir a legenda vinculada à sua imagem. Isso corresponde ao atributo alt HTML.

   CAPTURA DE TELA

1. Você também pode optar por **[!UICONTROL Localizar fotos semelhantes do Stock]**. `[Learn more](../integrations/stock.md)`

1. Na guia **[!UICONTROL Estilos]**, ajuste os outros atributos de estilo, como margem, borda etc. ou adicionando um link para redirecionar o público-alvo para outro conteúdo do painel **[!UICONTROL Configurações de componente]**.

## Redes sociais {#social}

Use o componente **[!UICONTROL Social]** para inserir links para páginas de redes sociais no seu conteúdo de email.

1. Em **[!UICONTROL Componentes do Conteúdo]**, arraste e solte o componente **[!UICONTROL Social]** em um **[!UICONTROL componente de Estrutura]**.

1. Selecione o componente recém-adicionado.

1. No campo **[!UICONTROL Social]** da guia **[!UICONTROL Configurações]**, escolha a mídia social que deseja adicionar ou remover.

   CAPTURA DE TELA

1. Escolha o tamanho dos ícones por meio do campo dedicado.

1. Clique em cada um dos ícones da rede social para configurar a **[!UICONTROL URL]** para a qual o público-alvo será redirecionado.

   CAPTURA DE TELA

1. Você também pode alterar os ícones de cada uma das mídias sociais, se necessário, no Assets.

1. Ajuste os outros atributos de estilo, como estilo, margem, borda etc. na guia **[!UICONTROL Estilos]**.

## Decisão de oferta {#offer-decision}

Use o componente **[!UICONTROL Offer decision]** para inserir ofertas em suas mensagens. O mecanismo do `[decision management](../offers/get-started/starting-offer-decisioning.md)` escolherá a melhor oferta para entregar aos seus clientes.

1. Em **[!UICONTROL Componentes do Conteúdo]**, arraste e solte o componente **[!UICONTROL Decisão de oferta]** em um **[!UICONTROL componente de Estrutura]**.

1. Clique em **[!UICONTROL Adicionar]** para selecionar sua **[!UICONTROL Decisão de oferta]**.

   CAPTURA DE TELA

1. Na lista suspensa, selecione seus **[!UICONTROL Posicionamentos]**.  Em seguida, selecione a **[!UICONTROL Decisão de oferta]** que deseja adicionar ao seu conteúdo e clique em **[!UICONTROL Adicionar]**.

   CAPTURA DE TELA

1. Na guia **[!UICONTROL Offer decision]**, você pode visualizar ou alterar a Oferta inserida.

Saiba como adicionar ofertas personalizadas a um email no `[this section](add-offers-email.md)`.

>[!IMPORTANT]
>
>Se forem feitas alterações em uma decisão de oferta em uso na mensagem de uma jornada, será necessário desfazer a publicação da jornada e republicá-la.  Isso garantirá que as alterações sejam incorporadas à mensagem da jornada e que ela seja consistente com as atualizações mais recentes.

