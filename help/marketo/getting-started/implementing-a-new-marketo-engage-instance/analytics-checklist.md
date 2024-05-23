---
description: Configure a seção Analytics para a nova instância do Marketo Engage.
title: Novas práticas recomendadas de instância - Lista de verificação do Analytics
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 46485fb692c0ad9734cbe9cad9df24736002587a
workflow-type: tm+mt
source-wordcount: '1435'
ht-degree: 0%

---

# Novas práticas recomendadas de instância: lista de verificação do Analytics {#new-instance-best-practices-analytics-checklist}

A seção Analytics oferece relatórios globais que analisam o desempenho de seus esforços de marketing. Saiba mais sobre as etapas necessárias para navegá-las.

Lembre-se de [baixar as listas de verificação](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e acompanhe seu progresso.

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
    <td><li>Use uma convenção de nomenclatura de relatório para diferenciar relatórios na guia Relatórios globais.</li>
    <ul>
    <li>Um exemplo de boa prática de convenção de nomenclatura é [Tipo de relatório] [Global vs. Tag específica da BU] [Descrição do relatório] como [Desempenho do email]-[Global]-[Envolvimento de email de 180 dias].</li>
    </ul> 
    <li>Identifique relatórios que devem ser compartilhados com diferentes grupos de usuários em sua organização (por exemplo, equipe de vendas, liderança de marketing) e organize os relatórios por pasta dentro da pasta Relatórios do grupo no Analytics for Global Reports.</li> 
    <li>O arquivamento deve ser limitado à pasta Relatórios globais, pois esses são relatórios sempre ativos.   <ul>
    <li>Limite o arquivamento a alterações organizacionais, como a redução ou a adição de unidades de negócios relevantes, se você estiver emitindo relatórios com base em uma estrutura de unidade de negócios.</li>
    </ul></td>
  </tr>
  <tr>
    <td>Espaços de trabalho (se aplicável)</td>
    <td><li>Replicar os Relatórios globais e a estrutura de pastas nos espaços de trabalho, se você usar o espaço de trabalho, para manter relatórios consistentes para suas equipes. Esses relatórios ficariam contidos na pasta Relatórios do grupo.</li></td>
  </tr>
  <tr>
    <td>Meus relatórios</td>
    <td><li>Identifique e crie os relatórios necessários para uso no <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/creating-reports/understanding-my-reports-and-group-reports">Meus relatórios</a> seção. Use essa seção de relatório privada como sandbox para Relatórios globais. Elas só estão disponíveis para o usuário que está criando o relatório.</li>
    <li>Use a convenção de nomenclatura de sua organização para identificar o relatório e o uso, de modo que você possa reconciliar seus relatórios em Meus relatórios com relatórios em Relatórios de grupo.</li></td>
  </tr>
  <tr>
    <td>Relatórios de grupos</td>
    <td><li>Relatórios de grupo são os Relatórios globais da sua organização e devem relatar a atividade geral da sua organização Marketo Engage.</li>
    <li>Considere criar <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/clone-a-report-to-group-reports" target="_blank">relatórios principais clonáveis</a> você espera que cada unidade de negócios use o máximo para reduzir o tempo necessário para obter o relatório e garantir a exatidão dos dados. Veja os detalhes no <a href="#global-reports">Tabela de relatórios globais abaixo</a>.
    <ul><li>Relatório de desempenho de pessoas (baseado em tempo e horário) - por origem, mês</li>
    <li>Relatório de desempenho do programa (por mês de custo, com base no tempo)</li>
    <li>Relatório de desempenho de email (baseado em tempo)</li></ul>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-activity/report-email-campaign-performance-across-workspaces" target="_blank">Ativar o "Relatório global"</a> na guia Configuração do relatório para incluir os dados de todos os espaços de trabalho nos relatórios Desempenho do email e Desempenho do link de email. Se você tiver mais de um espaço de trabalho, será necessário ativá-lo somente no espaço de trabalho padrão.</li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: Criar o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists" target="_blank">Lista inteligente</a> com os filtros que deseja incluir na maioria dos relatórios na seção 'Banco de dados'. Quando é necessário atualizar os critérios da Smart List, você pode atualizá-la em um local em vez de atualizá-la em todos os Relatórios globais.</td>
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
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: Os emails de assinatura geralmente são enviados durante a noite. Se quiser que as pessoas acessem os dados do relatório em tempo real, será necessário adicioná-las como usuários para que possam verificar o relatório diretamente.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/subscribe-to-a-basic-report">Configurar assinaturas</a> de acordo com a cadência desejada (diária/semanal/mensal) para o monitoramento contínuo de cada equipe. Também é possível <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-subscriptions/manage-report-subscriptions">exibir todas as suas assinaturas</a> em um local na guia Subscriptions no Analytics.</li></td>
  </tr>
</tbody>
</table>

## Relatórios Globais {#global-reports}

Identifique relatórios que devem ser compartilhados com diferentes grupos de usuários em sua organização (por exemplo, equipe de vendas, liderança de marketing). Crie a estrutura de pastas adequada para cada equipe/grupo de usuários/unidade de negócios para organizar os relatórios nos Relatórios do grupo ao clonar os relatórios. Considere a configuração de relatórios globais como:

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
    <td><li>Crie relatórios globais em toda a espaço de trabalho/unidade de negócios com os emails corretos selecionados.</li>
    <li>Crie um relatório de desempenho de email local em todos os modelos de programa clonáveis.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame">Usar um período relevante</a> (por exemplo, YTD, últimos 90 dias etc.) para que o relatório forneça uma visualização precisa das métricas padrão de envolvimento e entrega de email.</li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/email-setup/filtering-email-bot-activity">Ativar a filtragem de "Atividade de bot" em "Admin&gt;Email"</a> para evitar o registro ou identificar se o registro está ativado para as atividades de bot. <a href="https://nation.marketo.com/t5/product-documents/filtering-email-bot-activity-feature-latest-release/ta-p/324860">Inclua o filtro para permitir somente atividades Abertas/Clicadas com a restrição "Atividade de bot Is" definida como "Falso"</a> na Smart List de seus Relatórios globais clonáveis.</td>
  </tr>
  <tr>
    <td>Relatório de Desempenho de Pessoas</td>
    <td><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: é recomendável ter um <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags">estratégia de canal e tag</a> para cada implementação de Marketo Engage antes que você possa rastrear as pessoas adquiridas em cada uma e o ROI de seus investimentos em marketing por canal.
    <p>
    <li>Determine os critérios que você usará para medir o desempenho de seus programas de aquisição de clientes potenciais e crie seus relatórios padrão baseados em tempo (ano atual, últimos 12 meses contínuos ou 180 dias) com base nessas métricas:</li> <ul><li>Programa de aquisição: programa Marketo Engage que é creditado pela aquisição do lead.
    <li>Origem de Pessoa: A categoria de origem de como o registro passou a ser conhecido do banco de dados (com base na lista de valores Origem no seu CRM)
    </li></ul>
    <li>Meça as pessoas criadas por semana ou mês. Este relatório fornecerá uma medida da taxa de crescimento do seu banco de dados e se você está se aproximando ou excederá em breve o limite de tamanho do seu banco de dados.</li>
    <li>Filtrar as métricas nos Relatórios de desempenho de pessoas por <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/editing-reports/add-custom-columns-to-a-person-report">usando suas Smart Lists como colunas personalizadas.</a></li>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: Crie as Smart Lists para as colunas personalizadas que deseja adicionar ao Relatório de desempenho de pessoas em "Banco de dados" em vez de "Atividades de marketing" para que possa ver o nome da Smart List de forma adequada e clara quando for selecionada no relatório.</td>
  </tr>
  <tr>
    <td>Relatório de desempenho do programa</td>
    <td><p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: esse relatório exige que você tenha seus canais, status de progressão e etapas de sucesso definidos na <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/tags/create-a-program-channel">Administração &gt; Área de tags</a>.
    <p>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report">Meça a eficácia das suas táticas de marketing</a> programas seletivos.</li>
    <li>Gerencie a associação ao programa (usando Campanhas inteligentes para atualizar o programa de aquisição, o status, os status de sucesso) de acordo com as práticas recomendadas nas Atividades de marketing.</li>
    <li>Medida com base nos custos do ano atual e dos 12 meses consecutivos.
    <ul><li>Lembre-se de que a manutenção <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/using-period-costs-in-a-program">Custos do Período</a> O é essencial para aproveitar o Relatório de desempenho do programa.</li></ul>
    <p><img src="assets/tip-icon.png" alt="ícone de nota"> DICA: para agregar e exibir qualquer <a href="https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people">listas importadas</a> nos Relatórios de desempenho do programa, certifique-se de que suas equipes selecionem o Programa de aquisição apropriado para marcação. Considere <a href="https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/programs-and-campaigns/default-programs/create-and-measure-default-programs">criação de um programa padrão</a> para ser selecionado como o programa de aquisição quando as listas importadas não se aplicam a nenhum canal. Isso garante que qualquer pessoa importada tenha um programa de aquisição válido relacionado à origem, unidade de negócios, canal, etc. em vez de em branco.</td>
  </tr>
  <tr>
    <td>Relatório de desempenho da landing page</td>
    <td><li>Crie o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">Relatório de desempenho da landing page</a> como um relatório global para que você possa <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/landing-page-actions/filter-a-landing-page-performance-report">filtrar e revisar os números</a> de todas as suas páginas de aterrissagem do Design Studio ou páginas de aterrissagem de atividades de marketing em um único local.</li>
    <li>Para os programas com landing pages, considere <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-performance-report">criação de um relatório local dedicado no modelo de programa</a> para que você possa analisar o desempenho no nível do programa.</li></td>
  </tr>
  <tr>
    <td>Relatório de atividades da página da Web</td>
    <td><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: somente páginas da Web (páginas de aterrissagem externas e do Marketo) que tenham <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website">o JavaScript Munchkin</a> ativado será rastreado neste relatório. Considere a inserção do código JavaScript na plataforma do Tag Management, como <a href="https://developers.marketo.com/blog/integrating-munchkin-with-google-tag-manager/">Gerenciador de tags da Google</a>, para evitar a codificação rígida do código em cada página da Web.
    <p>
    <li>Crie o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/web-page-activity-report">Relatório de atividades da página da Web</a> como um relatório global, para que você possa revisar os números de todas as páginas da Web em um local. Observe que suas atividades externas de página da Web são refletidas somente nos relatórios de Atividades da página da Web.</li></td>
  </tr>
</tbody>
</table>

## Relatórios locais {#local-reports}

Alguns relatórios de Marketo Engage são melhor implantados como ativos locais em programas específicos em &quot;Atividades de marketing&quot;, pois seu melhor uso é em um conjunto mais limitado de programas e ativos. Considere a configuração de relatórios básicos como:

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
    <td><li>Criar <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report" target="_blank">Relatório de desempenho do link de email</a> nos programas que enviam emails e em suas campanhas por gotejamento para fornecer insights sobre os links que as pessoas clicam nos emails enviados.</li></td>
  </tr>
  <tr>
    <td>Relatório de atividades de campanha</td>
    <td><li>Crie o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">Relatório de atividades de campanha</a> e escolha um ponto na pasta operacional em "Atividades de marketing".</li>
    <li>Configurar relatórios para monitorar os acionadores de cada caso de uso e <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/reporting/basic-reporting/report-types/campaign-activity-report" target="_blank">aplicar filtros de campanha</a>, por exemplo, acionadores de Pontuação de comportamento, acionadores de qualificação de ciclo de vida, acionadores de Momentos interessantes.</li></td>
  </tr>
  <tr>
    <td>Relatório de desempenho do fluxo de engajamento (se aplicável)</td>
    <td><li>Criar <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/engagement-stream-performance-report" target="_blank">Relatório de Desempenho de Fluxo de Envolvimento</a> para medir a eficácia do conteúdo e do fluxo implantados em seu programa de engajamento.</li>
    <li>Considere <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/group-email-reports-by-segmentations" target="_blank">uso do filtro "Segmentação" na guia Configuração do relatório</a> e agrupamento dos dados de relatório pelo <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation" target="_blank">segmento</a> (por exemplo, fonte de pessoa, setor) usada em seu programa de envolvimento. Isso ajudará a obter insights mais profundos sobre os padrões de engajamento de cada segmento, orientando você a fazer alterações estratégicas para melhorar o programa de Engajamento (conteúdo, fluxo, cadência de transmissão etc.).</li></td>
  </tr>
</tbody>
</table>
