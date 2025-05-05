---
description: Configure a seção Analytics para a nova instância do Marketo Engage.
title: Novas práticas recomendadas de instância - Lista de verificação do Analytics
feature: Getting Started
exl-id: ddbb9bc7-d06a-4a2e-a560-9d308630ae3f
source-git-commit: 7a847ece020ea0c0001241abf8e49b9eadf8edce
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 1%

---

# Novas práticas recomendadas de instância: lista de verificação do Analytics {#new-instance-best-practices-analytics-checklist}

A seção Analytics oferece relatórios globais que analisam o desempenho de seus esforços de marketing. Saiba mais sobre as etapas necessárias para navegá-las.

Lembre-se de [baixar as listas de verificação](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e acompanhar seu progresso.

## Árvore {#tree}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
    <th></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Organização: nomeação, pastas e arquivamento</td>
    <td><li>Use uma convenção de nomenclatura de relatório para diferenciar relatórios na guia Relatórios globais.
    <ul><li>Um exemplo de boa prática de convenção de nomenclatura é [Tipo de relatório] [Global vs. Tag específica da BU] [Descrição do relatório] como [Desempenho do email]-[Global]-[Envolvimento de email de 180 dias].</li></ul><br>
    <li>Identifique relatórios que devem ser compartilhados com diferentes grupos de usuários em sua organização (por exemplo, equipe de vendas, liderança de marketing) e organize os relatórios por pasta dentro da pasta Relatórios do grupo no Analytics for Global Reports.</li> 
    <li>O arquivamento deve ser limitado à pasta Relatórios globais, pois esses são relatórios sempre ativos.   <ul><li>Limite o arquivamento a alterações organizacionais, como a redução ou a adição de unidades de negócios relevantes, se você estiver emitindo relatórios com base em uma estrutura de unidade de negócios.</li></ul>
    </td>
  </tr>
  <tr>
    <td>Espaços de trabalho (se aplicável)</td>
    <td><li>Replique os Relatórios globais e a estrutura de pastas nos espaços de trabalho para manter a consistência dos relatórios para suas equipes. Esses relatórios estariam na pasta Relatórios do grupo.</li></td>
  </tr>
  <tr>
    <td>Meus relatórios</td>
    <td><li>Identifique e crie os relatórios necessários para uso na seção <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Meus Relatórios</a>. Use essa seção de relatório privada como sandbox para Relatórios globais. Elas só estão disponíveis para o usuário que está criando o relatório.</li>
    <li>Use a convenção de nomenclatura de sua organização para identificar o relatório e o uso para que você possa reconciliar relatórios em Meus Relatórios com relatórios em Relatórios de Grupo.</li></td>
  </tr>
  <tr>
    <td>Relatórios de grupos</td>
    <td><li>Relatórios de grupo são os Relatórios globais da sua organização e devem relatar as atividades gerais da sua organização.</li>
    <li>Considere criar <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">relatórios principais clonáveis</a> que cada unidade de negócios usará com mais frequência para reduzir o tempo necessário para obter o relatório e garantir a exatidão dos dados. Veja os detalhes na <a href="#global-reports">tabela Relatórios Globais abaixo</a>.
    <ul><li>Relatório de desempenho de pessoas (com base em tempo e horário) por origem, mês</li>
    <li>Relatório de desempenho do programa (por mês de custo, com base no tempo)</li>
    <li>Relatório de desempenho de email (baseado em tempo)</li></ul>
    <li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Ative a opção "Relatório Global"</a> na guia Configuração do relatório para incluir os dados de todos os espaços de trabalho nos relatórios Desempenho do Email e Desempenho do Link de Email. Se houver mais de um espaço de trabalho, você só precisará ativá-lo no espaço de trabalho padrão.</li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: Crie a <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Smart List</a> com os filtros que deseja incluir na maioria dos relatórios na seção Banco de Dados. Quando é necessário atualizar os critérios da Smart List, você pode atualizá-la em um local em vez de atualizá-la em todos os Relatórios globais.</td>
  </tr>
</tbody>
</table>

## Assinaturas {#subscriptions}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Assinaturas</td>
    <td><li>Alinhe com seu líder de marketing em relação às pessoas que devem revisar os resultados do relatório e sua cadência durante a implementação.</li> <li>Use assinaturas para distribuir dados a pessoas que precisam de informações na sua organização sem esgotar uma licença de usuário nomeada.</li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: se você quiser que as pessoas acessem os dados de relatório em tempo real, será necessário adicioná-los como usuários para que eles possam exibir o relatório.
    <p>
    <li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Configure as assinaturas</a> na cadência desejada (diariamente/semanalmente/mensalmente) para o monitoramento contínuo de cada equipe. Você também pode <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">exibir todas as suas assinaturas</a> em um local na guia Assinaturas do Analytics.</li></td>
  </tr>
</tbody>
</table>

## Relatórios Globais {#global-reports}

Identifique relatórios que devem ser compartilhados com diferentes grupos de usuários em sua organização (por exemplo, equipe de vendas, liderança de marketing). Crie a estrutura de pastas adequada para cada equipe/grupo de usuários/unidade de negócios para organizar os relatórios clonados nos Relatórios do grupo. Considere a configuração de relatórios globais, como:

<table>
<thead>
  <tr>
    <th style="width:20%">Tipo de relatório</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Relatório de desempenho de email</td>
    <td><li>Crie relatórios globais em toda a unidade de Workspace/negócios com os emails corretos selecionados.</li>
    <li>Crie um Relatório de desempenho de email local em todos os modelos de programa clonáveis.</li>
    <li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Usar um período relevante</a> (por exemplo, YTD, últimos 90 dias etc.) para que o relatório forneça uma visualização precisa das métricas padrão de envolvimento e capacidade de entrega de email.</li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Ative a filtragem 'Atividade de bot' em <strong>Admin &gt; Email</strong></a> para evitar o registro em log ou identificar se o registro em log está habilitado para atividades de bot. Inclua o filtro para permitir somente <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">atividades Abertas/Clicadas com a restrição "Atividade de bot Is" definida como "Falsa"</a> na Smart List de seus Relatórios Globais clonáveis.</td>
  </tr>
  <tr>
    <td>Relatório de Desempenho de Pessoas</td>
    <td><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: é recomendável ter uma <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">estratégia de canal e tag</a> adequada para cada implementação de Marketo Engage para que você possa rastrear as pessoas adquiridas e o ROI de seus investimentos em marketing por canal.
    <p>
    <li>Determine os critérios que você usará para medir o desempenho de seus programas de aquisição de clientes potenciais e crie seus relatórios padrão baseados em tempo (ano atual, últimos 12 meses contínuos ou 180 dias) com base nessas métricas: <ul><li>Programa de aquisição: programa de Marketo Engage que é creditado pela aquisição da pessoa.</li>
    <li>Source de pessoa: a categoria de origem de como o registro ficou conhecido para o banco de dados (com base na lista de origem de valores no CRM)
    </li></ul>
    <li>Meça as pessoas criadas por semana ou mês. Este relatório fornecerá uma medida da taxa de crescimento do Banco de Dados e se você está se aproximando do limite de tamanho do Banco de Dados.</li>
    <li>Filtre as métricas nos Relatórios de Desempenho de Pessoas <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">usando suas Smart Lists como colunas personalizadas.</a></li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: crie Smart Lists para as colunas personalizadas que deseja adicionar ao Relatório de desempenho de pessoas no banco de dados em vez de Atividades de marketing para que você possa ver o nome da Smart List de forma adequada e clara quando ela estiver selecionada no relatório.</td>
  </tr>
  <tr>
    <td>Relatório de desempenho do programa</td>
    <td><p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: este relatório requer que você tenha seus canais, status de progressão e etapas de sucesso definidos em <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/tags/create-a-program-channel"><strong>Administrador</strong> &gt; <strong>Marcas</strong></a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Meça a eficácia de suas táticas de marketing</a> em programas seletivos.</li>
    <li>Gerencie a associação ao programa (usando Campanhas inteligentes para atualizar o programa de aquisição, o status, os status de sucesso) de acordo com as práticas recomendadas nas Atividades de marketing.</li>
    <li>Medida com base nos custos do ano atual e nos 12 meses consecutivos.
    <ul><li>Lembre-se de que manter <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Custos do Período</a> é essencial para aproveitar o Relatório de Desempenho do Programa.</li></ul></li>
    <p>
    <img src="assets/tip-icon.png" alt="ícone de nota"> DICA: para agregar e visualizar quaisquer <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">listas importadas</a> nos Relatórios de desempenho do programa, certifique-se de que suas equipes selecionem o Programa de aquisição apropriado para marcação. Considere <a href="https://experienceleague.adobe.com/pt-br/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">criar um programa padrão</a> a ser selecionado como o programa de Aquisição quando as listas importadas não se aplicarem a nenhum canal. Isso garante que qualquer pessoa importada tenha um programa de aquisição válido relacionado à origem, unidade de negócios, canal, etc., em vez de um valor em branco.</td>
  </tr>
  <tr>
    <td>Relatório de desempenho da landing page</td>
    <td><li>Crie o <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Relatório de desempenho da página de aterrissagem</a> como um relatório global para que você possa <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrar e revisar os números</a> de todas as suas Páginas de aterrissagem do Design Studio/Atividades de marketing em um local.</li>
    <li>Para programas com Página(s) de Aterrissagem, considere <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">criar um relatório local dedicado dentro do modelo de programa</a> para que você possa analisar o desempenho no nível do programa.</li></td>
  </tr>
  <tr>
    <td>Relatório de atividades da página da Web</td>
    <td><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: somente as páginas da Web (páginas de aterrissagem externas e do Marketo) que têm <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">o Munchkin JavaScript</a> habilitado serão rastreadas neste relatório. Considere colocar o código do JavaScript na Plataforma Tag Management, como o <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Google Tag Manager</a>, para evitar a codificação rígida do código em cada página da Web.
    <p>
    <li>Crie o <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Relatório de Atividades da Página da Web</a> como um relatório global para que você possa examinar os números de todas as páginas da Web em um local. Observe que suas atividades externas de página da Web são refletidas somente nos relatórios de Atividades da página da Web.</li></td>
  </tr>
</tbody>
</table>

## Relatórios locais {#local-reports}

Alguns relatórios de Marketo Engage são melhor implantados como ativos locais em programas específicos em Atividades de marketing, pois seu uso típico é em um conjunto mais limitado de programas e ativos. Considere a configuração de relatórios básicos, como:

<table>
<thead>
  <tr>
    <th style="width:20%">Tipo de relatório</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Relatório de desempenho do link de email</td>
    <td><li>Crie um <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Relatório de Desempenho do Link de Email</a> em programas que enviam emails e em suas campanhas drip para fornecer insights sobre os links que as pessoas clicam em seus emails enviados.</li></td>
  </tr>
  <tr>
    <td>Relatório de atividades de campanha</td>
    <td><li>Crie o <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Relatório de atividades de campanha</a> e escolha um período em sua pasta operacional em Atividades de marketing.</li>
    <li>Configure relatórios para monitorar os acionadores de cada caso de uso e <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/filter-a-campaign-activity-report" target="_blank">aplique filtros de campanha</a> (por exemplo, acionadores de Pontuação de comportamento, acionadores de qualificação de ciclo de vida, acionadores de Momentos interessantes).</li></td>
  </tr>
  <tr>
    <td>Relatório de desempenho do fluxo de engajamento (se aplicável)</td>
    <td><li>Crie um <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Relatório de Desempenho de Fluxo de Envolvimento</a> para medir a eficácia do conteúdo e do fluxo implantados em seu Programa de Envolvimento.</li>
    <li>Considere usar o filtro <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">"Segmentação" na guia Configuração do relatório</a> e agrupar os dados de relatório pelo <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segmento</a> (por exemplo, fonte de pessoa, setor) usado em seu Programa de Envolvimento. Isso ajudará a obter insights mais profundos sobre os padrões de engajamento de cada segmento, orientando você a fazer alterações estratégicas para melhorar o programa de Engajamento (conteúdo, fluxo, cadência de transmissão etc.).</li></td>
  </tr>
</tbody>
</table>
