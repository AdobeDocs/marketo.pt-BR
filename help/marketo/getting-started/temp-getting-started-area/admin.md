---
description: NOVA ÁREA - Documentação do Marketo - Documentação do produto
title: NOVA ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 6%

---

# NOVA ÁREA: Lista de verificação do administrador {#new-area-admin-checklist}

Texto de introdução.

## Funções {#roles}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Funções</td>
    <td><li>Revise as funções pré-criadas e confirme quais permissões/acesso cada função tem.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Criar uma nova função</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">editar as funções</a> com base nas necessidades de sua organização e na frequência com que os usuários fazem logon.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Atribuir usuários às funções apropriadas</a>.</li>
    <li>Depois de atribuir as funções para usuários, revise o número de usuários por função.</li>  <li>Implemente uma função exclusiva para cada usuário da API para facilitar a solução de problemas.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentação</td>
    <td>Defina usuários e funções para sua organização. <br>Defina seu processo para adicionar um novo usuário/administrador.</td>
    <td></td>
  </tr>
  <tr>
    <td>Sandbox (se aplicável)</td>
    <td>Revise as categorias acima para sua sandbox, se você tiver uma.</td>
    <td></td>
  </tr>
</tbody>
</table>

## Espaços de trabalho e partições {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaços de trabalho e partições </td>
    <td><li>Determine o número de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> espaços de trabalho</a> e/ou partições que sua organização precisa ter e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">quantos usuários têm acesso a cada espaço de trabalho.</a></li>
    <li>Defina o objetivo principal de cada espaço de trabalho e partição.</li>
    <li>Defina o relacionamento entre seus espaços de trabalho e partições.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentação</td>
    <td><li>Documente como os espaços de trabalho são definidos e como eles se relacionam com as partições de banco de dados (ou seja, um espaço de trabalho global que vê todos, em comparação aos setores de negócios).</li>
    <li>Importar novos registros para a partição apropriada.</li>
    <li>Defina o valor no CRM que coloca os usuários na partição apropriada.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Configurações da campanha inteligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Configurações da campanha inteligente </td>
    <td><li>Adicionar um <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restrição no tamanho da Campanha inteligente</a>, evitando o envio acidental por email de todo o banco de dados.</li>
    <li>Ativar restrições de pessoa para Campanhas inteligentes</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Configurações de e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Padrões de email</td>
    <td><li>Em Domínio de marca, selecione seu domínio e adicione seu CNAME de email. Isso deve estar no formato: [EmailTrackingCNAME].[Domínio da empresa].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configurar SPF e DKIM</a> para capacidade de entrega de email.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Limites de comunicação {#communication-limits}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de comunicação</td>
    <td><li>Local <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Limites de comunicação</a>.</li>
    <li>Determine se sua empresa requer uma política de limites de comunicação.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Tags {#tags}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canais</td>
    <td><li>Definir como usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">canais</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Tags </td>
    <td><li>Definir como usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tags</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Calendário (se aplicável) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Emitir vagas do Calendário de marketing</a> a quem precisa de acesso.</li> 
    <li>Configurar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendário</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Gerenciamento de bancos de dados {#database-management}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gerenciamento de campos</td>
    <td><li>Implementar a convenção de nomenclatura para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">campos personalizados.</a> Por exemplo, comece com "MKTO".</li>
    <li>Seja seletivo quanto aos campos sincronizados. Quanto mais campos você sincronizar, mais lento será o ciclo de sincronização.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Bloquear atualizações de campos</a> você deseja gravar no uma vez (ou seja, fonte de lead original, detalhes da fonte de lead original, campos de UTM de primeiro contato etc.).</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Atividades personalizadas </td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Atividades personalizadas</a> que são específicos para a sua empresa.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Objetos personalizados </td>
    <td><li>Analise quantas <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Objetos personalizados</a> você precisa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Sincronizar esses Objetos Personalizados com seu CRM</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Integrações {#integrations}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Iniciar Sincronização do CRM. Escolha uma das opções a seguir, dependendo do CRM que sua empresa usa: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>Identifique o tipo de acesso necessário para acessar seu CRM.</li>
    <li>Identifique o administrador do CRM para solucionar problemas.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Sales Insight (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Configurar o Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Emita vagas para os usuários apropriados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Configurar a API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Personalizar as pontuações dos clientes potenciais.</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>Páginas de aterrissagem </td>
    <td>OBSERVAÇÃO: você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial. <br>Configure seu domínio de landing page com um <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">inserir informações de domínio e página</a>. Deve estar no formato: [LandingPageCNAME].[DomínioDaEmpresa].com <br>Escolha um CNAME para suas landing pages. Alguns exemplos: <br>* **ir**.[DomínioDaEmpresa].com <br>* **www2**.[DomínioDaEmpresa].com <br>* **lp**.[DomínioDaEmpresa].com <br>DICA: Mantenha curto! URLs mais curtos são mais fáceis de lembrar. Sugerimos "go" como o domínio. <br>Adicione o código de rastreamento de análise (por exemplo, Google Analytics ou Adobe Analytics) aos modelos de página de aterrissagem. </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">Editar configurações da página de aterrissagem</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">OBSERVAÇÃO: se você for um cliente do Launch Pack, ignore esta etapa. Seu consultor fornecerá a você instruções do código Munchkin em seu documento de instruções de configuração de TI. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Adicionar código de rastreamento do Munchkin</a> ao seu site. O código do Munchkin pode ser <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">codificado</a> ou implantado pelo Google Tag Manager.</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Adicionar Munchkin Track Code para o seu site</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">Rastreamento de leads</a> </td>
  </tr>
  <tr>
    <td>Serviços da Web </td>
    <td>Ativar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">as restrições de IP</a> se aplicável. <br>Determine os usuários/aplicativos que podem fazer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">Chamadas de API</a> em sua instância. <br>Revise todos os aplicativos que farão chamadas de API e determine se um aumento ou um corte é necessário para as chamadas de API.</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">Criar uma Inclui na lista de permissões para Acesso à API com base em IP </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (se aplicável) </td>
    <td>Para usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>, o canal nativo de engajamento conversacional no Marketo Engage, você continuará com a configuração de permissão do usuário seguindo as etapas abaixo em <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador de sistema da organização Adobe. Contato <a href="https://helpx.adobe.com/contact.html" target="_blank">Atendimento ao cliente Adobe</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> para descobrir quem na sua organização tem privilégios de administrador no console. <br>Aceitar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">o convite 'Dynamic Chat Product Admin'</a>. A variável <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">email de boas-vindas</a> é enviado quando o Dynamic Chat está ativado na sua instância Marketo Engage e você é designado como um Administrador do sistema.  <br>Atribua todos os usuários apropriados ao perfil de produto Marketo Engage no Adobe Admin Console. <br>Não é possível atribuir funções de usuários no Marketo Engage/Admin/Usuários e funções antes de adicioná-los a um Perfil de produto.  <br>Se um usuário indesejável for adicionado a vários perfis de produto, você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Dynamic Chat. </td>
    <td> </td>
  </tr>
  <tr>
    <td>Ponto de lançamento (se aplicável) </td>
    <td>Configure os obrigatórios <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> serviços para sua empresa.  <br>OBSERVAÇÃO: os webinários interativos são um recurso de webinário integrado com integração nativa ao Adobe Connect. Não é necessária nenhuma integração adicional, mas sua instância precisará <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">sincronizar com o Adobe Connect as a LaunchPoint Service.</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">Integrações adicionais</a> </td>
  </tr>
  <tr>
    <td>Webhooks (se aplicável)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Criar todos os webhooks necessários</a> para sua empresa.  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Criar um Webhook</a> </td>
  </tr>
</tbody>
</table>

## Baú do tesouro {#treasure-chest}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Item de Ação</th>
    <th>Prioridade</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Baú do tesouro</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Ativar o Treasure Chest</a> para experimentar os recursos do piloto.  <br>Determine os recursos que deseja ativar ou desativar.</td>
    <td>Texto</td>
  </tr>
  <tr>
    <td>Inspetor de campanhas </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Ativar o Inspetor de campanha</a> para exibir todas as suas Campanhas inteligentes de uma só vez.</td>
    <td>Texto</td>
  </tr>
</tbody>
</table>
