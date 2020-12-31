---
unique-page-id: 4719093
description: Segmentos da Web - Documentos do Marketing - Documentação do produto
title: Segmentos da Web
translation-type: tm+mt
source-git-commit: 44e4fd230bb1e997700f6b31290d224899561f9a
workflow-type: tm+mt
source-wordcount: '2031'
ht-degree: 0%

---


# Segmentos da Web {#web-segments}

## Segmento de visualização {#view-segment}

![](assets/image2014-11-11-20-3a24-3a5.png)

A guia Segmentos exibe todos os segmentos personalizados definidos que você configurou com base em vários atributos.  **Um segmento é uma coleção de visitantes que atendem aos critérios especificados definidos na página &quot;Definir um segmento&quot;.**  Um segmento pode ser visitantes de um setor específico, local ou com base na atividade no local do visitante.

Na Personalização da Web, um visitante pode corresponder a mais de um segmento. Por exemplo, se houver um segmento para visitantes dos EUA e um segmento para empresas financeiras, um visitante da Web do Bank of America corresponderia **ambos** ao segmento para visitantes dos EUA e ao segmento para empresas financeiras.

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
   <td colspan="1" rowspan="1"><p><strong>Corresponde</strong></p></td> 
   <td colspan="1" rowspan="1">O número de visitantes que atendem aos critérios personalizados e definidos do segmento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Definir Campanha</strong></td> 
   <td colspan="1" rowspan="1">Permite configurar um CTA de Campanha associado ao termo de pesquisa selecionado</td> 
  </tr> 
  <tr> 
   <td colspan="1"><strong>Visitantes</strong></td> 
   <td colspan="1">Uma pré-visualização da tabela visitantes associada ao termo de pesquisa selecionado</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Clickstream</strong></td> 
   <td colspan="1" rowspan="1">Exibe uma tabela da atividade do visitante e o caminho do URL no site e quanto tempo eles visitaram cada página </td> 
  </tr> 
 </tbody> 
</table>

Consulte [como criar e visualização rótulos de segmentos](label-your-segment.md)

**Segmentos - Painel direito**

![](assets/image2014-11-12-10-3a46-3a32.png)

Selecionar um segmento na tabela mostra detalhes adicionais sobre o segmento no painel direito.

Esses detalhes incluem:

* Nome do segmento
* Data de criação do segmento
* As campanhas associadas mostrando as campanhas que operam com o segmento. Clicar no número de reações leva você para a página de campanhas que exibe o CTA da Campanha (Chamada para Ação) do segmento
* O número de correspondências (quantidade de visitantes que atenderam aos critérios do segmento) para o segmento e o número de visitantes distintos (exclusivos) que corresponderam ao segmento. Clicar no link de visitante único leva você até a página do visitante que exibe os resultados do segmento
* O proprietário/criador de usuário do segmento
* Os sites de domínio associados ao segmento
* Um breve resumo dos critérios selecionados do segmento

## Ativar ou desativar um segmento {#enable-or-disable-a-segment}

![](assets/image2014-11-12-10-3a48-3a9.png)

Para ativar ou desativar um segmento, marque a caixa de seleção desse Segmento na tabela e, na caixa suspensa &quot;Escolher ação&quot;, na parte inferior da tabela, selecione a ação &quot;Ativar&quot; ou &quot;Desativar&quot;. Quando um segmento é desativado, a palavra &quot;desativar&quot; é exibida abaixo da coluna Estado.

## Criar segmentos {#create-segments}

O segmento criado atende aos critérios específicos definidos na página **Definir segmento**. Você também pode personalizar seus segmentos com base em uma combinação de critérios, direcionando uma audiência específica em sua campanha.

Para criar um novo segmento

Na página **Segmentos**, clique em **Criar novo** no gráfico. A tela a seguir é exibida.

![](assets/four.png)

Defina parâmetros gerais para o seu segmento:

* **Nome:**  nomeie seu segmento.
* **Descrição:**  forneça uma explicação mais detalhada dos critérios de segmento.
* **Domínios:**  selecione os domínios que deseja incluir no segmento.
* **Lógica da regra de segmento:**  selecione uma lógica E/OU para criar cada atributo de segmentação
* **Tempo:** Defina o nível de envolvimento do visitante desejado em sua campanha

   * **Na Entrada**: Participe da chegada do visitante ao site
   * **Após o 1º a 9º clique**: Envolva o visitante após uma quantidade específica de cliques no site

>[!TIP]
>
>**Lógica da regra de segmento**
>
>Há três opções de filtro:
>
>1. Usar todos os Filtros (1 e 2 e 3...)
>1. Usar quaisquer Filtros (1 ou 2 ou 3...)
>1. Filtros avançados (usando e/ou expressão)

   >
   >    
   Filtros avançados permitem controlar a condição do segmento. Insira os números de filtro separados por &quot;e&quot; e &quot;ou&quot;.
   >
   >    
   * 1 e 2 e 3
   >    * 1 ou 2 ou 3

   >
   Misturar &quot;e&quot; e &quot;ou&quot; requer parênteses para esclarecer a intenção lógica. por exemplo, &quot;1 ou 2 e 3&quot; deve ser escrito como uma das seguintes menções:

   * 1 e (2 ou 3)
   * (1 e 2) ou 3

   Os parênteses aninhados são aceitos para uma lógica mais complicada, por exemplo.

   * (1 e 2) ou (3 e 4)
   * 1 e 2 ou 3 e 4)

   Verifique sua lógica após qualquer inserção, exclusão ou reordenação.






Arraste e solte os atributos do segmento da coluna do lado direito no editor de segmentos do lado esquerdo:

![](assets/five.png)

### Firmográficos {#firmographics}

**Localização**

Arraste e solte **Location** no editor de segmentos.

* Selecione um dos seguintes parâmetros:

   * **Incluir**  - Selecione se deseja que a campanha inclua ou exclua um local.
   * **Selecione o país a ser adicionado**  - Na caixa suspensa, selecione o país que deseja incluir no segmento. O nome do país é exibido à direita. Você pode escolher vários países.

Depois que o país é adicionado, você também pode especificar o estado, a cidade e o CEP do segmento.

* **Selecione Estado ou província para adicionar**  - Na caixa suspensa, selecione o estado dos EUA ou província canadense que deseja incluir. É possível fazer várias seleções.
* **CEP**  - insira o CEP que deseja incluir no seu segmento.
* **Cidades**  - Entre na cidade ou cidades que deseja incluir. Use ponto-e-vírgula entre cidades.

>[!TIP]
>
>**Quais condições de segmento eu escolho? &quot;AND&quot; ou &quot;OR&quot;?** OU funciona como uma opção adicional em cada campo. Os prospectos precisam apenas atender a um critério dos vários critérios selecionados em cada campo para se qualificarem para o segmento. (Por exemplo, prospectos podem ser dos EUA. *ou* do setor de Defesa). E funciona como um parâmetro obrigatório adicional que deve ser atendido para este segmento. (Por exemplo, os prospectos devem ser dos EUA e da indústria de Defesa). Em cada perfil de segmentação, cada campo separado pode funcionar como ambos, seja &quot;E&quot; ou &quot;OU&quot;, dependendo da Condição do segmento selecionada.

**** IndústriasNa seção  **Segmentação** do Perfil, marque a caixa ao lado da  **Indústria**.

* Selecione um dos seguintes parâmetros:

   * **Inclui**  - Selecione se deseja que o segmento inclua ou exclua um setor.
   * **Selecione Indústrias para adicionar**  - Selecione o setor que deseja incluir no segmento. O setor é exibido abaixo da caixa suspensa. Você pode escolher vários setores.

**Grupo de organizações**

Na seção **Segmentação do Perfil**, marque a caixa ao lado de **Grupo da Organização.**

* Na caixa suspensa, selecione uma das seguintes opções:

   * Fortune 500 - Inclui apenas empresas do Fortune 500 neste segmento
   * Fortune 1000 - Inclui apenas empresas do Fortune 1000 neste segmento
   * Global 2000 - Inclui as empresas globais 2000 neste segmento
   * Empresa - Inclui organizações com mais de 1.000 funcionários e receita superior a US$ 250 milhões
   * SMB - Inclui apenas pequenas e médias empresas neste segmento

**Contas nomeadas**

**Organizações**

* **É dessas empresas (nomes específicos)**

   * Selecione empresa a público alvo no menu suspenso &#39;Selecionar empresa para adicionar&#39;.
   * Você pode digitar o nome exato da organização que deseja público alvo. *É recomendável que *sempre *use Listas de Conta Nomeada em vez de digitar os nomes manualmente para melhores correspondências (consulte abaixo).*

**Lista de conta nomeada**

Selecione de uma [Lista Conta nomeada](../../../product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md) para segmentar as principais contas direcionadas

![](assets/image2015-5-27-17-3a14-3a8.png)

>[!NOTE]
>
>O número entre colchetes ao lado do nome da Lista Conta nomeada é usado como uma referência de índice para a lista de Personalização da Web [Ler API](http://developers.marketo.com/documentation/websites/rtp-js-api/).

**Excluir ISP**

Exclui Provedores de serviço da Internet (ISPs) do segmento.

### Pessoas conhecidas {#known-people}

**Banco de dados**

A Personalização da Web se integra ao seu Banco de Dados de Marketing, permitindo que você segmente e personalize campanhas por atributos e dados de pessoas conhecidas.

Selecione Banco de dados e selecione um campo de dados de pessoa no menu suspenso. Selecione a variável   **+** para adicionar campos do menu suspenso.

![](assets/seven.png)

Você pode adicionar ou remover campos de dados de pessoa de Configurações da conta > Banco de dados

>[!TIP]
>
>Crie seus critérios de segmento de acordo com todos os campos de dados pessoais de Marketo para pessoas como Título do trabalho; Pontuação; Papel; etc...
>
>Eg. &quot;Cargo igual a COM&quot; e &quot;A pontuação é menor que ou igual a 50&quot;

**Marketo Email** CampaignSegmente e personalize campanhas por email de referência de um visitante clicando em um email de marketing e chegando ao site. Segmentar por Nome do Programa ou Nome da Campanha do Marketing e continuar a conversa de email para Web. Selecione + para adicionar campos no menu suspenso.

![](assets/image2015-5-27-17-3a20-3a34.png)

**Status**

Defina seu segmento de acordo com o status de um prospecto: conhecido ou anônimo.

* Known - Selecione essa opção na caixa suspensa para visitantes conhecidos. Um visitante é conhecido quando ele envia um formulário para o seu site e aparece na página Pessoas da personalização da Web.
* Anônimo - Selecione essa opção na caixa suspensa para visitantes anônimos.

![](assets/image2015-5-27-17-3a23-3a2.png)

### Comportamento {#behavioral}

**Visitas -** Defina seu segmento de acordo com o comportamento ou a identificação do visitante.

* Número de visitas - Selecione essa opção na caixa suspensa para especificar o número de visitas para prospectos no site.

   * Selecione Igual, Igual ou Maior que, ou Igual ou Menor que na caixa suspensa.

* Visitas específicas - Selecione essa opção na caixa suspensa para especificar um visitante específico.

   * Na caixa de texto à direita, digite o número do visitante que deseja rastrear. O número exclusivo de identificação do visitante de personalização da Web pode ser encontrado ao clicar em um visitante (na página visitantes) e em Definir Campanha no painel direito. A ID do Visitante está localizada na seção Configurações avançadas. A ID do visitante também pode ser encontrada no URL (por exemplo, VISITANTE=JZJIFNUI60PZ8Y97BHTY9BL8PKWS).

**Termos**  de pesquisa - Defina um segmento de acordo com os termos de pesquisa de um prospecto.

* O visitante pesquisado - Na lista suspensa, selecione os termos que deseja rastrear na pesquisa de visitantes ou adicione seus próprios termos de pesquisa. (Não há necessidade do * curinga em termos de pesquisa, pois ele é definido como padrão para incluir frases que contêm o termo de pesquisa).

**Referências**  - Adicione URLs pelas quais o visitante foi referenciado.

* Selecione as referências a serem adicionadas - na lista suspensa, selecione os sites de referência que deseja rastrear ou adicione sua própria referência. Uma vez selecionadas, as referências aparecerão na caixa abaixo. (É permitido usar * como curinga)

**Incluir páginas**  - rastreie prospectos de páginas específicas visitados em seu site.

* Correspondências de URL - adicione o URL de páginas da Web específicas que você deseja rastrear. É possível adicionar vários URLs separando-os com um ponto e vírgula. (É permitido usar * como curinga).

**Excluir páginas**  - exclua páginas específicas que não deseja corresponder no segmento. (É permitido usar * como curinga).

* URL não corresponde - Adicione o URL de páginas da Web específicas que você deseja excluir do rastreamento. É possível adicionar vários URLs separando-os com um ponto e vírgula

![](assets/segment-extra.png)

### Dispositivo / Navegador {#device-browser}

**SO móvel**

Arraste e solte o Mobile OS no editor de segmentos

![](assets/image2015-5-27-17-3a45-3a3.png)

* **Tipo de visitante**

   **Sistema operacional**  móvel - Na caixa suspensa, selecione um ou mais sistemas operacionais móveis listados. O SO móvel selecionado é exibido abaixo.

   * O visitante está usando qualquer dispositivo móvel
   * O visitante está usando este dispositivo/SO específico
   * O visitante não está usando nenhum dispositivo móvel

* **Dispositivo**   - Na lista suspensa, selecione um ou mais dispositivos (Apple, Samsung, LG, HTC, Nexus, Blackberry etc..). Os dispositivos selecionados são exibidos abaixo.

**Navegador**

Visitante de público alvo que usa tipos e/ou versões de navegadores específicos.

* Tipo de navegador - Na caixa suspensa, selecione um ou mais navegadores da Internet . Os navegadores selecionados são exibidos abaixo.
* Versão do navegador - insira a versão do navegador que deseja adicionar ao segmento. É possível selecionar várias versões separando cada uma com uma vírgula. (É permitido usar * como curinga).

### API {#api}

**Eventos**  de dados - visitantes de segmentos que acionam Eventos de dados personalizados específicos

Adicione o valor do Evento que você deseja público alvo. Por exemplo, de fontes de dados de terceiros.

**API de contexto do usuário**

Chamada da API de personalização da Web [leia mais sobre ela aqui.](http://developers.marketo.com/documentation/websites/rtp-user-context-api/)

>[!TIP]
>
>**Uso de curingas -** quando você deseja incluir qualquer termo de pesquisa ou URL que contenha algo dentro dele, ou seja, &quot;[google.com](http://google.com)&quot; ou &quot;produto de termo de pesquisa&quot;, chamamos isso de curinga e ele deve ser digitado com um asterisco - esse carinha* - em cada extremidade. Portanto, qualquer item vindo de [google.com](http://google.com) deve ser inserido como * [google.com](http://google.com)*

## Editar segmentos {#edit-segments}

É possível editar um segmento que foi criado.

1. Para editar um segmento, vá para **Segmentos**.

   ![](assets/image2014-11-12-11-3a38-3a22.png)

1. Na tabela **Segmentos**, clique no ícone de edição ( ![](assets/segment-edit.png)) do segmento que deseja editar. A página **Definir segmento** é aberta com o segmento selecionado.
1. Aplique todas as edições ou alterações que desejar fazer no segmento.
1. Clique em **Salvar**.

## Excluir segmentos {#delete-segments}

É possível excluir segmentos criados.

1. Na página **Segmentos** acima, selecione um segmento.
1. Clique no ícone de exclusão ( ![](assets/segment-delete.png) ) do segmento que deseja excluir.
1. Uma mensagem de confirmação é exibida, confirmando que você está prestes a excluir o **Segmento**.

>[!NOTE]
Não é possível excluir um segmento associado a uma campanha. Primeiro, é necessário excluir a campanha e, em seguida, o segmento.

Ótimo! Agora que você entende a seção Segmentos, vamos aprender sobre campanhas.

>[!MORELIKETHIS]
* [Criar um segmento básico da Web](create-a-basic-web-segment.md)
* [Criar uma nova Campanha da Web de diálogo](../../../product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Criar uma nova Campanha da Web na zona](../../../product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Criar uma nova Campanha Web de widget](../../../product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)

