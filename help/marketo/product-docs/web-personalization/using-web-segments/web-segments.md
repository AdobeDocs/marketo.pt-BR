---
unique-page-id: 4719093
description: Segmentos da Web - Documentos do Marketo - Documentação do produto
title: Segmentos da Web
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '2031'
ht-degree: 6%

---

# Segmentos da Web {#web-segments}

## Exibir segmento {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

A guia Segmentos exibe todos os segmentos personalizados definidos que você configurou com base em vários atributos.  **Um segmento é uma coleção de visitantes que atendem aos critérios especificados, definidos na página &quot;Definir um segmento&quot;.**  Um segmento pode ser visitantes de um setor específico, local ou com base na atividade do visitante no site.

Na Personalização da Web, um visitante pode corresponder a mais de um segmento. Por exemplo, se houver um segmento para visitantes dos EUA e um segmento para empresas financeiras, um visitante da Web do Bank of America corresponderia **both** o segmento para visitante dos EUA e o segmento para empresas financeiras.

**GRÁFICO:**  A página Segmentos exibe um gráfico de barras dos segmentos selecionados de acordo com o número de visitantes do segmento (eixo y) e o nome do segmento (eixo x).

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Nome</th> 
   <th colspan="1" rowspan="1">Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Nome</strong></td> 
   <td colspan="1" rowspan="1">O título do segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>Correspondências</strong></p></td> 
   <td colspan="1" rowspan="1">O número de visitantes que atendem aos critérios personalizados e definidos do segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Definir campanha</strong></td> 
   <td colspan="1" rowspan="1">Permite configurar um CTA de campanha associado ao termo de pesquisa selecionado</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Visitantes</strong></td> 
   <td colspan="1">Uma visualização da tabela de visitantes associada ao termo de pesquisa selecionado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Fluxo de cliques</strong></td> 
   <td colspan="1" rowspan="1">Exibe uma tabela da atividade e do caminho do URL do visitante no site, além do tempo que ele visitou cada página </td> 
  </tr> 
 </tbody> 
</table>

Consulte [como criar e exibir rótulos de segmentos](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segmentos - Painel direito**

![](assets/image2014-11-12-10-3a46-3a32.png)

Selecionar um segmento na tabela revela detalhes adicionais sobre o segmento no painel direito.

Esses detalhes incluem:

* Nome do segmento
* Data de criação do segmento
* As campanhas associadas que mostram as campanhas que operam com o segmento. Clicar no número de reações leva você à página de campanhas exibindo o CTA da campanha (Chamada à ação) para o segmento
* O número de correspondências (quantidade de visitantes que atendeu aos critérios do segmento) para o segmento e o número de visitantes distintos (exclusivos) que corresponderam ao segmento. Clicar no link do visitante único leva você até a página do visitante que exibe os resultados do segmento
* O proprietário/criador de usuário do segmento
* Os sites de domínio associados ao segmento
* Um breve resumo dos critérios selecionados do segmento

## Ativar ou desativar um segmento {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Para ativar ou desativar um segmento, marque a caixa de seleção desse Segmento na tabela e, na caixa suspensa &quot;Escolher ação&quot;, na parte inferior da tabela, selecione a ação &quot;Ativar&quot; ou &quot;Desativar&quot;. Quando um segmento é desativado, a palavra &quot;desativar&quot; é exibida abaixo da coluna Estado.

## Criar segmentos {#create-segments}

O segmento criado atende aos critérios específicos definidos na variável **Definir segmento** página. Você também pode personalizar seus segmentos com base em uma combinação de critérios, direcionando um público-alvo específico em sua campanha.

Para criar um novo segmento

No **Segmentos** página, clique em **Criar novo** sob o gráfico. A tela a seguir é exibida.

![](assets/four.png)

Defina parâmetros gerais para o segmento:

* **Nome:**  Dê um nome ao seu segmento.
* **Descrição:**  Forneça uma explicação mais detalhada dos critérios do segmento.
* **Domínios:**  Selecione os domínios que deseja incluir no segmento.
* **Lógica da regra do segmento:**  Selecione uma lógica E/OU para criar cada atributo de segmentação
* **Tempo:** Defina o nível de engajamento do visitante desejado em sua campanha

   * **Na entrada**: Participe da chegada do visitante ao site
   * **Após 1º a 9º clique**: Envolva o visitante após uma quantidade específica de cliques no site

>[!TIP]
>
>**Lógica da regra do segmento**
>
>Há três opções de filtro:
>
>1. Usar todos os filtros (1 e 2 e 3...)
>1. Usar qualquer filtro (1 ou 2 ou 3...)
>1. Filtros avançados (usando expressões e / ou )

   >
   >    Filtros avançados permitem-lhe controlar a condição do segmento. Insira os números dos filtros separando-os por &quot;e&quot; e &quot;ou&quot;.
   >
   >    * 1 e 2 e 3
   >    * 1 ou 2 ou 3

   >
   >    Se quiser usar &quot;e&quot; e &quot;ou&quot; simultaneamente, use parênteses para esclarecer a intenção lógica. Ex. &quot;1 ou 2 e 3&quot; deve ser escrito de uma das seguintes maneiras:
   >
   >    * 1 e (2 ou 3)
   >    * (1 e 2) ou 3

   >
   >    Caso a lógica seja mais complexa, use parênteses encadeados. Ex.
   >
   >    * (1 e 2) ou (3 e 4)
   >    * 1 e (2 ou (3 e 4))

   >
   >    Confira a lógica depois de inserir, excluir ou reordenar.


Arraste e solte os atributos do segmento da coluna lateral direita no editor de segmentos do lado esquerdo:

![](assets/five.png)

### Perfil da empresa {#firmographics}

**Local**

Arrastar e soltar **Localização** no editor de segmentos.

* Selecione um dos seguintes parâmetros:

   * **Incluir** - Selecione se deseja que a campanha inclua ou exclua um local.
   * **Selecionar país para adicionar** - Na caixa suspensa , selecione o país que deseja incluir no segmento. O nome do país é exibido à direita. Você pode escolher vários países.

Depois que o país for adicionado, você também poderá especificar o estado, a cidade e o código postal do segmento.

* **Selecione Estado ou Província para adicionar** - Na caixa suspensa , selecione o estado dos EUA ou província canadense que deseja incluir. É possível fazer várias seleções.
* **Código Postal** - Insira o CEP que deseja incluir no segmento.
* **Cidades** - Insira a(s) cidade(s) que deseja incluir. Use ponto e vírgula entre cidades.

>[!TIP]
>
>**Quais condições de segmento eu escolho? &quot;AND&quot; ou &quot;OR&quot;?** OU funciona como uma opção adicional em cada campo. As perspectivas precisam atender apenas um critério dos vários critérios selecionados em cada campo para se qualificarem para o segmento. (Por exemplo, os prospetos podem ser dos EUA. *ou* da indústria da defesa). E funciona como um parâmetro obrigatório adicional que deve ser atendido para este segmento. (Por exemplo, os prospetos devem ser dos Estados Unidos e do setor de Defesa). Em cada perfil de segmentação, cada campo separado pode funcionar como ambos, um &quot;AND&quot; ou &quot;OR&quot;, dependendo da Condição de segmento selecionada.

**Setores** Em **Segmentação de perfil** marque a caixa ao lado de **Setor**.

* Selecione um dos seguintes parâmetros:

   * **Inclui** - Selecione se deseja que o segmento inclua ou exclua um setor.
   * **Selecione Indústrias para adicionar** - Selecione o setor que deseja incluir no segmento. O setor aparece abaixo da caixa suspensa. Você pode escolher vários setores.

**Grupo da organização**

Em **Segmentação de perfil** marque a caixa ao lado de **Grupo da Organização.**

* Na caixa suspensa , selecione uma das seguintes opções:

   * Fortune 500 - Inclui apenas 500 empresas Fortune neste segmento
   * Fortune 1000 - Inclui apenas 1000 empresas da Fortune neste segmento
   * Global 2000 - Inclui as 2000 empresas globais neste segmento
   * Empresa - Inclui organizações com mais de 1.000 funcionários e receita superior a US$ 250 milhões
   * SMB - Inclui apenas pequenas e médias empresas neste segmento

**-Contas nomeadas-**

**Organizações**

* **É proveniente dessas empresas (nomes específicos)**

   * Selecione empresa a ser direcionada no menu suspenso &quot;Selecionar empresa para adicionar&quot;.
   * Você pode digitar o nome exato da organização que deseja direcionar. *É _always_ recomendado usar Listas de contas nomeadas em vez de digitar os nomes manualmente para melhores correspondências (veja abaixo).

**Lista de contas nomeadas**

Selecione de um [Lista de contas nomeadas](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) para segmentar as principais contas direcionadas.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>O número entre colchetes ao lado do nome da Lista de contas nomeadas é usado como uma referência de índice para a lista de Personalização da Web [Ler API](https://developers.marketo.com/documentation/websites/rtp-js-api/).

**Excluir provedor de Internet**

Exclui provedores de serviços de Internet (ISPs) do segmento.

### Pessoas conhecidas {#known-people}

**Banco de dados**

A Personalização da Web integra-se ao seu Banco de dados do Marketo, permitindo segmentar e personalizar campanhas por atributos e dados de pessoa conhecidos.

Selecione Banco de dados e selecione um campo de dados de pessoa no menu suspenso. Selecione o **+** para adicionar campos no menu suspenso .

![](assets/seven.png)

Você pode adicionar ou remover campos de dados de pessoas em Configurações da Conta > Banco de Dados

>[!TIP]
>
>Crie seus critérios de Segmento de acordo com todos os campos de dados de pessoa das pessoas do Marketo, como Título do trabalho; Pontuação; Papel; etc...
>
>Ex. &quot;Título de trabalho igual a OCM&quot; e &quot;Pontuação é inferior ou igual a 50&quot;

**Campanha por email do Marketo** Segmente e personalize campanhas por email de referência de um visitante que clica em um email do Marketo e chega ao site. Segmente por nome do programa ou da campanha do Marketo e continue a conversa partindo do e-mail para a Web. Selecione + para adicionar campos no menu suspenso.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Status**

Defina seu segmento de acordo com o status de um prospecto: conhecido ou anônimo.

* Conhecido - Selecione essa opção na caixa suspensa para visitantes conhecidos. Um visitante é conhecido quando ele envia um formulário em seu site e aparece na página Pessoas da personalização da Web .
* Anônimo - Selecione essa opção na caixa suspensa para visitantes anônimos.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportamental {#behavioral}

**Visitas -** Defina seu segmento de acordo com o comportamento do visitante ou identifique.

* Número de visitas - Selecione essa opção na caixa suspensa para especificar o número de visitas para prospetos no site.

   * Selecione Igual, Igual ou Maior que, ou Igual ou Menor que na caixa suspensa.

* Visitas específicas - Selecione essa opção na caixa suspensa para especificar um visitante específico.

   * Na caixa de texto à direita, digite o número de visitante que deseja rastrear. O número de identificação de visitante único da Personalização da Web pode ser encontrado ao clicar em um visitante (na página de visitantes) e em Definir campanha no painel lateral direito. A ID de visitante está localizada na seção Configurações avançadas . A ID de visitante também pode ser encontrada no URL (por exemplo, VISITOR=JZJIFNUI60PZ8Y97BHTY9BL8PKWS).

**Pesquisar termos** - Defina um segmento de acordo com os termos de pesquisa de um prospecto.

* O visitante pesquisou - Na lista suspensa, selecione os termos que deseja rastrear na pesquisa dos visitantes ou adicione seus próprios termos de pesquisa. (Não é necessário &#42; curinga em termos de pesquisa, pois é definido como padrão para incluir frases que contenham o termo de pesquisa).

**Referências** - Adicionar URLs para as quais o visitante foi referenciado.

* Selecione as referências a serem adicionadas - Na lista suspensa, selecione os sites de referência que deseja rastrear ou adicionar sua própria referência. Uma vez selecionadas, as referências serão exibidas na caixa abaixo. (Usando &#42; como um curinga é permitido)

**Incluir páginas** - Rastreie prospetos de páginas específicas visitados em seu site.

* Correspondências de URL - Adicione o URL de páginas da Web específicas que você deseja rastrear. Você pode adicionar vários URLs separando-os com um ponto e vírgula. (Usando &#42; como um curinga é permitido).

**Excluir páginas** - Exclua páginas específicas que você não deseja que correspondam ao segmento. (Usando &#42; como um curinga é permitido).

* URL não corresponde - Adicione o URL de páginas da Web específicas que você deseja excluir do rastreamento. Você pode adicionar vários URLs separando-os com um ponto e vírgula

![](assets/segment-extra.png)

### Dispositivo/Navegador {#device-browser}

**SO móvel**

Arraste e solte o sistema operacional móvel no editor de segmentos

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Tipo de visitante**<br />

   **SO móvel** - Na caixa suspensa , selecione um ou mais SOs móveis listados. O sistema operacional móvel selecionado é exibido abaixo.

   * O visitante está usando qualquer dispositivo móvel
   * O visitante está usando este dispositivo/SO específico
   * O visitante não está usando nenhum dispositivo móvel

* **Dispositivo**  - Na lista suspensa, selecione um ou mais dispositivos (Apple, Samsung, LG, HTC, Nexus, Blackberry etc..). Os dispositivos selecionados aparecem abaixo.

**Navegador**

Visitante do Target que usa tipos e/ou versões específicas do navegador.

* Tipo de navegador - Na caixa suspensa, selecione um ou mais navegadores da Internet . Os navegadores selecionados são exibidos abaixo.
* Versão do navegador - Insira a versão do navegador que você deseja adicionar ao segmento. Você pode selecionar várias versões separando cada uma com uma vírgula. (Usando &#42; como um curinga é permitido).

### API {#api}

**Eventos de dados** - Segmentar visitantes que acionam eventos de dados personalizados específicos

Adicione o valor Event que deseja direcionar. Por exemplo, de fontes de dados de terceiros.

**API do contexto do usuário**

Chamada da API de personalização da Web  [leia mais sobre isso aqui.](https://developers.marketo.com/documentation/websites/rtp-user-context-api/)

>[!TIP]
>
>**Uso de curingas -** Quando você deseja incluir qualquer termo de pesquisa ou URL que contenha algo dentro dele, ou seja, &quot;[google.com](https://google.com)&quot; ou &quot;produto de termo de pesquisa&quot;, chamamos isso de curinga e ele deve ser inserido com um asterisco - esse carinha&#42; - em cada extremidade. Então, qualquer coisa vinda de [google.com](https://google.com) deve ser inserido como &#42; [google.com](https://google.com)&#42;

## Editar segmentos {#edit-segments}

É possível editar um segmento que foi criado.

1. Para editar um segmento, acesse **Segmentos**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. No **Segmentos** , clique no ícone editar ( ![](assets/segment-edit.png)) do segmento que você deseja editar. O **Definir segmento** abre com o segmento selecionado.
1. Aplique as edições ou alterações que deseja fazer no segmento.
1. Clique em **Salvar**.

## Excluir segmentos {#delete-segments}

É possível excluir segmentos criados.

1. No **Segmentos** acima, selecione um segmento.
1. Clique no ícone de exclusão ( ![](assets/segment-delete.png) ) do segmento que deseja excluir.
1. Uma mensagem de confirmação é exibida, confirmando que você está prestes a excluir o **Segmento**.

>[!NOTE]
>
>Não é possível excluir um segmento associado a uma campanha. Primeiro, é necessário excluir a campanha e depois o segmento.

Ótimo! Agora que você entendeu a seção Segmentos , vamos aprender sobre campanhas.

>[!MORELIKETHIS]
>
>* [Criar um segmento básico da Web](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
>* [Criar uma nova campanha Web de diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Criar uma nova campanha na Web na zona](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Criar uma nova campanha Web de widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)

