---
description: Recursos da GenAI - Documentação do Marketo - Documentação do produto
title: Recursos da GenAI
feature: Interactive Webinars
exl-id: 3e0a41b0-7ff3-4676-bafc-4e7a0725a737
source-git-commit: 6350137c2abfb46a0a8451772a8dc08391f3e4b5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Recursos da GenAI {#gen-ai-features}

Gere capítulos e resumos automaticamente para os webinars gravados, tornando-os mais acessíveis e fáceis de navegar para o público-alvo.

* **Geração automática de capítulo**: a tecnologia habilitada por IA cria capítulos para o conteúdo do webinário.

* **Resumo gerado por IA**: obtenha um resumo automatizado do texto de seu webinário.

* **Geração de blog com base em IA**: permite gerar automaticamente conteúdo de blog sobre a marca a partir de seus webinários.

* **Conteúdo editável**: modifique capítulos e resumos gerados, se desejar, usando funcionalidades de edição manuais e alimentadas por IA.

* **Fácil integração**: adicione facilmente capítulos e resumos às suas Páginas de Aterrissagem copiando o código do HTML para o editor de páginas da Web de sua escolha.

## Ativar GenAI {#enable-genai}

>[!PREREQUISITES]
>
>Antes de usar esses recursos, primeiro você deve aceitar os termos e condições da GenAI da Adobe. Caso ainda não o tenha feito, entre em contato com a Equipe de conta da Adobe (seu Gerente de conta) para obter detalhes.

Depois de aceitar os termos e condições da GenAI da Adobe, o próximo passo é habilitá-la para usuários individuais. Para fazer isso, vá para **[!UICONTROL Admin]** > **[!UICONTROL Webinars interativos]** e selecione quais usuários devem ter acesso à GenAI.

![](assets/gen-ai-features-1.png){width="800" zoomable="yes"}

## Como acessar o {#how-to-access}

1. Navegue até a página de visão geral do webinário em Webinários interativos do Marketo Engage.

1. Depois de conduzir o webinário sob demanda, aguarde de 30 a 60 minutos para que a IA processe sua gravação. O botão Gerar se tornará clicável quando estiver disponível.

1. Clique em **[!UICONTROL Exibir Conteúdo GenAI]**.

   ![](assets/gen-ai-features-2.png){width="800" zoomable="yes"}

1. Uma nova guia é aberta, exibindo capítulos gerados por IA e um resumo de texto.

## Editar conteúdo gerado {#edit-generated-content}

1. Revise os capítulos e o resumo gerados.

1. Se forem necessárias alterações, clique no botão **[!UICONTROL Editar]**.

   Fazendo modificações:

   * Editar texto no resumo e/ou nos títulos do capítulo.

   * Ajuste os carimbos de data e hora, se necessário, editando os valores nos campos de carimbo de data e hora.

   * Exclua capítulos indesejados selecionando-os e clicando em **[!UICONTROL Excluir]**.

   * Mescle dois capítulos consecutivos selecionando-os e clicando em **[!UICONTROL Mesclar]**.

      * A IA gera um capítulo composto composto pelos dois capítulos selecionados

      * Para mesclar vários capítulos, é necessário fazer dois de cada vez

     ![](assets/gen-ai-features-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* Se desejar, você pode classificar a qualidade do resumo/capítulos gerados com os ícones _miniatura_ ![Miniatura](assets/icon-thumbs-up.png) ou _miniatura_ ![Miniatura para baixo](assets/icon-thumbs-down.png). Você também pode sinalizar qualquer conteúdo problemático clicando no ícone de sinalizador ![Ícone de sinalizador](assets/icon-flag.png).
   >
   >* Se você não estiver satisfeito com o resumo inicial, clique no botão **[!UICONTROL Gerar resumo novamente]** e outra versão será gerada.

1. Salve as alterações clicando no botão **[!UICONTROL Salvar]** na parte superior direita da tela.

## Usar conteúdo gerado {#use-generated-content}

Depois de copiar o conteúdo que deseja usar, cole-o no editor de sua escolha (por exemplo, editor de página de destino do Marketo Engage) e faça os ajustes desejados.

### Resumo {#summary}

**Copiar HTML** - Clique no botão **[!UICONTROL Copiar HTML]** para obter todo o texto, completo com o código HTML formatando-o dentro de uma tabela.

**Somente texto** - Se desejar apenas o texto, basta realçá-lo e selecionar Ctrl/Cmd+C (ou clicar com o botão direito do mouse) para copiar.

### Capítulos {#chapters}

**Copiar HTML** - Clique no botão **[!UICONTROL Copiar HTML]** para que todas as gravações e seus capítulos sejam formatados em um player de vídeo.

## Direcionar seu público

Aproveite os filtros e/ou acionadores de Campanha/Lista inteligente para ver o que cada visualizador assistiu, quantas vezes etc., permitindo acompanhamentos personalizados.

![](assets/gen-ai-features-4.png){width="800" zoomable="yes"}

* **Acionadores**: _Link de Cliques na Página da Web_, _Página da Web de Visitas_

* **Filtros**: _Link Clicado na Página da Web_, _Página da Web Visitada_

O &quot;link&quot; é o nome do capítulo e a &quot;página da Web&quot; é a página que hospeda o webinário sob demanda.

>[!TIP]
>
>Use [restrições](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} para refinar ainda mais seu público-alvo.

## Itens a serem observados {#things-to-note}

* Excluir ou mesclar capítulos afeta apenas a pilha do capítulo, não o conteúdo de vídeo em si. Essas ações são permanentes.

* Os recursos da GenAI são flexíveis e podem ser usados com vários editores de página da Web, não apenas os do Marketo Engage.

* Somente sessões realizadas em salas de seminários estarão disponíveis para a geração de blogues. As salas de seminários estão disponíveis somente em contas com um Módulo de evento ou uma licença de Seminário (Sala compartilhada/Eventos).

* Sempre visualize as alterações para garantir a funcionalidade e a aparência desejadas.

* A exclusão do webinário também exclui o conteúdo GenAI.

* Se quiser excluir o conteúdo GenAI sem excluir o webinário, entre em contato com a Equipe de Conta da Adobe (seu Gerente de Conta) ou envie uma solicitação de exclusão de dados para: `marketo-webinar-genai-alerts@adobe.com`.
