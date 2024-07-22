---
unique-page-id: 4719093
description: Segmentos da Web - Documentação do Marketo - Documentação do produto
title: Segmentos da Web
exl-id: ec62c1ae-579a-4753-9b2d-18c7c2fa1ff5
feature: Web Personalization
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 5%

---

# Segmentos da Web {#web-segments}

## Exibir segmento {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

A guia Segmentos exibe todos os segmentos definidos pelo cliente que você configura com base em vários atributos.  **Um segmento é uma coleção de visitantes que atendem aos critérios especificados na página &#39;Definir um segmento&#39;.** Um segmento pode ser de visitantes de um setor, local ou com base na atividade do visitante no site.

No Web Personalization, um visitante pode corresponder a mais de um segmento. Por exemplo, se houver um segmento para visitantes dos EUA e um segmento para empresas financeiras, um visitante do Bank of America corresponderá **tanto** o segmento para visitante dos EUA quanto o segmento para empresas financeiras.

**GRÁFICO:** a página Segmentos exibe um gráfico de barras dos segmentos selecionados de acordo com o número de visitantes do segmento (eixo y) e o nome do segmento (eixo x).

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
   <td colspan="1" rowspan="1">Permite configurar um CTA do Campaign associado ao termo de pesquisa selecionado</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Visitantes</strong></td> 
   <td colspan="1">Uma visualização da tabela de visitantes associada ao termo de pesquisa selecionado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Fluxo de cliques</strong></td> 
   <td colspan="1" rowspan="1">Exibe uma tabela da atividade do visitante e o caminho do URL no site, e quanto tempo eles visitaram cada página </td> 
  </tr> 
 </tbody> 
</table>

Consulte [como criar e exibir rótulos de segmento](/help/marketo/product-docs/web-personalization/using-web-segments/label-your-segment.md)

**Segmentos - Painel direito**

![](assets/image2014-11-12-10-3a46-3a32.png)

A seleção de um segmento na tabela revela detalhes adicionais sobre o segmento no painel direito.

Esses detalhes incluem:

* Nome do segmento
* Data de criação do segmento
* As campanhas associadas que mostram as campanhas que operam com o segmento. Ao clicar no número de reações, você é levado para a página de campanhas que exibe o CTA (Call to Action) da campanha para o segmento
* O número de correspondências (quantidade de visitantes que atenderam aos critérios do segmento) para o segmento e o número de visitantes distintos (únicos) que corresponderam ao segmento. Ao clicar no link de visitante único, você é levado à página do visitante que exibe os resultados do segmento
* O criador do segmento/usuário
* Os sites do domínio associados ao segmento
* Um breve resumo dos critérios selecionados do segmento

## Ativar ou desativar um segmento {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Para ativar ou desativar um segmento, marque a caixa de seleção desse Segmento na tabela e, na caixa suspensa &quot;Escolher ação&quot; na parte inferior da tabela, selecione a ação &quot;Ativar&quot; ou &quot;Desativar&quot;. Quando um segmento é desativado, a palavra &quot;desativar&quot; é exibida abaixo da coluna Estado.

## Criar segmentos {#create-segments}

O segmento criado atende a qualquer critério específico definido na página **Definir segmento**. Você também pode personalizar seus segmentos com base em uma combinação de critérios, direcionando um público-alvo específico na sua campanha.

Para criar um novo segmento

Na página **Segmentos**, clique em **Criar novo** no gráfico. A tela a seguir é exibida.

![](assets/four.png)

Defina parâmetros gerais para o seu segmento:

* **Nome:** Nomeie seu segmento.
* **Descrição:** forneça uma explicação mais detalhada dos critérios do segmento.
* **Domínios:** selecione os domínios que deseja incluir no segmento.
* **Lógica da regra de segmento:** selecione uma lógica AND/OR para criar cada atributo de segmentação
* **Horário:** defina o nível de envolvimento do visitante que você deseja em sua campanha

   * **Na Entrada**: participação do visitante que chega ao site
   * **Após o primeiro - o nono clique**: envolver o visitante após uma quantidade específica de cliques no site

>[!TIP]
>
>**Lógica da regra de segmento**
>
>Há três opções de filtro:
>
>1. Usar todos os filtros (1, 2 e 3...)
>1. Use quaisquer filtros (1, 2 ou 3...)
>1. Filtros avançados (usando expressões and/or)
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

Arraste e solte os atributos de segmento da coluna do lado direito no editor de segmentos do lado esquerdo:

![](assets/five.png)

### Perfil da empresa {#firmographics}

**Local**

Arraste e solte **Local** no editor de segmentos.

* Selecione entre os seguintes parâmetros:

   * **Incluir** - Selecione se deseja que a campanha inclua ou exclua uma localização.
   * **Selecione o país a ser adicionado** - Na caixa suspensa, selecione o país que deseja incluir no segmento. O nome do país é exibido à direita. Você pode escolher vários países.

Depois que o país for adicionado, também será possível especificar o estado, a cidade e o CEP do segmento.

* **Selecione Estado ou Província para adicionar** - Na caixa suspensa, selecione o estado dos EUA ou Província Canadense que deseja incluir. É possível fazer várias seleções.
* **CEP** - Digite o CEP que você deseja incluir no seu segmento.
* **Cidades** - Insira a cidade ou cidades que deseja incluir. Use um ponto e vírgula entre as cidades.

>[!TIP]
>
>**Quais condições de segmento eu escolho? &quot;AND&quot; ou &quot;OR&quot;?** OR funciona como uma opção adicional em cada campo. Os clientes potenciais precisam atender apenas a um critério dos vários critérios selecionados em cada campo para se qualificarem para o segmento. (Por exemplo, clientes potenciais podem ser dos EUA *ou* do setor de defesa). AND funciona como um parâmetro obrigatório adicional que deve ser atendido para esse segmento. (Por exemplo, os clientes potenciais devem ser tanto dos EUA quanto da indústria de defesa). Em cada perfil de segmentação, cada campo separado pode funcionar como ambos, &quot;E&quot; ou &quot;OU&quot;, dependendo da Condição de segmento selecionada.

**Setores** Na seção **Segmentação de Perfil**, marque a caixa ao lado de **Setor**.

* Selecione entre os seguintes parâmetros:

   * **Inclui** - Selecione se você deseja que o segmento inclua ou exclua um setor.
   * **Selecione os setores a serem adicionados** - Selecione o setor que deseja incluir no segmento. O setor aparece abaixo da caixa suspensa. Você pode escolher vários setores.

**Grupo de Organizações**

Na seção **Segmentação de Perfil**, marque a caixa ao lado de **Grupo de Organizações.**

* Na caixa suspensa, selecione uma das seguintes opções:

   * Fortune 500 - inclui neste segmento somente empresas da Fortune 500
   * Fortune 1000 - inclui neste segmento apenas empresas da Fortune 1000
   * Global 2000 - inclui as empresas Global 2000 neste segmento
   * Empresa - inclui organizações com mais de 1.000 funcionários e receita superior a US$ 250 milhões
   * SMB - Inclui somente empresas de pequeno e médio porte neste segmento

**Contas Nomeadas-**

**Organizações**

* **É destas empresas (nomes específicos)**

   * Selecione a empresa a ser direcionada no menu suspenso &#39;Selecionar empresa para adicionar&#39;.
   * Você pode digitar o nome exato da organização que deseja direcionar. *É _sempre_ recomendável usar Listas de Contas Nomeadas em vez de digitar os nomes manualmente para obter melhores correspondências (veja abaixo).

**Lista de Contas Nomeadas**

Selecione de uma [Lista de contas nomeadas](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) para segmentar as principais contas direcionadas.

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>O número entre colchetes ao lado do nome da Lista de Contas Nomeadas é usado como uma referência de índice para a lista da [API de Leitura](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization) do Web Personalization.

**Excluir ISP**

Exclui provedores de serviço de internet (ISPs) do segmento.

### Pessoas conhecidas {#known-people}

**Banco de dados**

O Web Personalization integra-se ao banco de dados do Marketo, permitindo segmentar e personalizar campanhas por atributos e dados de pessoas conhecidas.

Selecione Banco de Dados e selecione um campo de dados da pessoa no menu suspenso. Selecione o **+** para adicionar campos do menu suspenso.

![](assets/seven.png)

Você pode adicionar ou remover campos de dados da pessoa em Configurações da conta > Banco de dados

>[!TIP]
>
>Crie os critérios do seu Segmento de acordo com todos os campos de dados de pessoas da Marketo, como Título do cargo, Pontuação, Função, etc...
>
>Ex. &quot;O título do trabalho é igual a CMO&quot; e &quot;A pontuação é menor ou igual a 50&quot;

**Campanha de email do Marketo** Segmente e personalize campanhas por referência de email de um visitante clicando em um email do Marketo e chegando ao site. Segmente por Nome de programa ou Nome de campanha da Marketo e continue a conversa do email para a Web. Selecione o + para adicionar campos no menu suspenso.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Status**

Defina seu segmento de acordo com o status de um cliente potencial: conhecido ou anônimo.

* Conhecido - Selecione essa opção na caixa suspensa para visitantes conhecidos. Um visitante é conhecido quando envia um formulário em seu site e aparece na página Pessoas do Web Personalization.
* Anônimo - Selecione essa opção na caixa suspensa para visitantes anônimos.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportamental {#behavioral}

**Visitas -** Defina seu segmento de acordo com o comportamento do visitante ou identifique-o.

* Número de visitas - Selecione essa opção na caixa suspensa para especificar o número de visitas para prospetos no site.

   * Selecione Igual, Igual ou Maior que, ou Igual ou Menor que na caixa suspensa.

* Visitas específicas - Selecione essa opção na caixa suspensa para especificar um visitante específico.

   * Na caixa de texto à direita, digite o número do visitante que deseja rastrear. O número exclusivo de identificação do visitante do Web Personalization pode ser encontrado ao clicar em um visitante (na página de visitantes) e no botão Definir campanha no painel direito. A ID do visitante está localizada na seção Configurações avançadas. A ID de visitante também pode ser encontrada no URL (por exemplo, VISITOR=JZZJIFJNUI60PZ8Y97BHTY9BL8PKWS).

**Termos de Pesquisa** - Defina um segmento de acordo com os termos de pesquisa de um cliente potencial.

* O visitante pesquisou - Na lista suspensa, selecione os termos que deseja rastrear na pesquisa de visitantes ou adicione seus próprios termos de pesquisa. (Não há necessidade do curinga &#42; nos termos de pesquisa, pois ele é definido como padrão para incluir frases que contêm o termo de pesquisa).

**Referências** - Adicione as URLs pelas quais o visitante foi referenciado.

* Selecionar referências a serem adicionadas - Na lista suspensa, selecione os sites de referência que deseja rastrear ou adicione sua própria referência. Depois de selecionadas, as referências aparecerão na caixa abaixo. (O uso de &#42; como curinga é permitido)

**Incluir páginas** - Rastreie os clientes potenciais de páginas específicas visitados em seu site.

* Correspondências de URL - Adicione o URL de páginas da Web específicas que você deseja rastrear. Você pode adicionar vários URLs separando-os com um ponto e vírgula. (O uso de &#42; como curinga é permitido).

**Excluir páginas** - Exclua páginas específicas que não deseja corresponder no segmento. (O uso de &#42; como curinga é permitido).

* O URL não corresponde: adicione o URL de páginas da Web específicas que você deseja excluir do rastreamento. Você pode adicionar vários URLs separando-os com um ponto e vírgula

![](assets/segment-extra.png)

### Dispositivo/Navegador {#device-browser}

**SO móvel**

Arraste e solte o SO móvel no editor de segmentos

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Tipo de visitante**<br />
  **SO móvel** - Na caixa suspensa, selecione um ou mais SOs móveis listados. O SO móvel selecionado é exibido abaixo.

   * O visitante está usando qualquer dispositivo móvel
   * O visitante está usando este dispositivo/SO específico
   * O visitante não está usando nenhum dispositivo móvel

* **Dispositivo** - Na lista suspensa, selecione um ou mais dispositivos (Apple, Samsung, LG, HTC, Nexus, Blackberry etc...). Os dispositivos selecionados são exibidos abaixo.

**Navegador**

Visitantes do Target que usam tipos e/ou versões específicas do navegador.

* Tipo de navegador - Na caixa suspensa, selecione um ou mais navegadores da Internet . Os navegadores selecionados aparecem abaixo de.
* Versão do navegador - Insira a versão do navegador que deseja adicionar ao segmento. Você pode selecionar várias versões separando cada uma com uma vírgula. (O uso de &#42; como curinga é permitido).

### API {#api}

**Eventos de dados** - Segmente visitantes que acionam eventos de dados personalizados específicos

Adicione o valor de Evento que deseja direcionar. Por exemplo, de fontes de dados de terceiros.

**API de Contexto de Usuário**

Chamada de API do Web Personalization [leia mais sobre isso aqui.](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/web-personalization)

>[!TIP]
>
>**Usando Curingas -** Quando você deseja incluir qualquer termo de pesquisa ou URL que contenha algo dentro dele, por exemplo, &quot;[google.com](https://google.com)&quot; ou &quot;produto de termo de pesquisa&quot;, chamamos isso de curinga e ele deve ser inserido com um asterisco - este carinha&#42; - em cada extremidade. Portanto, qualquer item vindo de [google.com](https://google.com) deve ser inserido como &#42; [google.com](https://google.com)&#42;

## Editar segmentos {#edit-segments}

Você pode editar um segmento que foi criado.

1. Para editar um segmento, vá para **Segmentos**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Na tabela **Segmentos**, clique no ícone de edição ( ![](assets/segment-edit.png)) do segmento que deseja editar. A página **Definir segmento** é aberta com o segmento selecionado.
1. Aplique todas as edições ou alterações que deseja fazer no segmento.
1. Clique em **Salvar**.

## Excluir segmentos {#delete-segments}

É possível excluir segmentos criados.

1. Na página **Segmentos** acima, selecione um segmento.
1. Clique no ícone de exclusão ( ![](assets/segment-delete.png) ) do segmento que deseja excluir.
1. Uma mensagem de confirmação é exibida confirmando que você está prestes a excluir o **Segmento**.

>[!NOTE]
>
Não é possível excluir um segmento associado a uma campanha. Primeiro, é necessário excluir a campanha e, em seguida, o segmento.

Ótimo! Agora que você entende a seção Segmentos, vamos aprender sobre campanhas.

>[!MORELIKETHIS]
>
* [Criar um segmento básico da Web](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)
* [Criar uma Nova Campanha da Web de Caixa de Diálogo](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Criar uma nova Campanha da Web na Zona](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Criar uma Nova Campanha Web do Widget](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
