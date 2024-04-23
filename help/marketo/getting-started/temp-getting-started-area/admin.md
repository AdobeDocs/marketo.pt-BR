---
description: NOVA ÁREA - Documentação do Marketo - Documentação do produto
title: NOVA ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: a9d902bf40e6193838a931ecb96a080bae098d68
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 5%

---

# NOVA ÁREA: Lista de verificação do administrador {#new-area-admin-checklist}

Texto de introdução.

## Funções {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Funções</td>
    <td><li>Revise as funções pré-criadas e confirme quais permissões/acesso cada função tem.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Criar uma nova função</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">editar as funções</a> com base nas necessidades da sua organização.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">Atribuir usuários às funções apropriadas</a>. Os usuários devem ser adicionados à assinatura no Adobe Admin Console antes de conceder suas funções nas Funções. Consulte a seção "Usuários" na lista de verificação "Configuração inicial" [LINK].</li>
    <li>Depois de atribuir as funções para usuários, analise o número de usuários por função.</li>
    <li>Implemente uma função exclusiva para cada usuário da API para facilitar a solução de problemas.</li></td>
  </tr>
  <tr>
    <td>Documentação</td>
    <td><li>Defina usuários e funções para sua organização.</li>
    <li>Defina seu processo para adicionar um novo usuário/administrador.</li></td>
  </tr>
  <tr>
    <td>Sandbox (se aplicável)</td>
    <td><li>Revise as categorias acima para seu <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md">sandbox</a>.</li></td>
  </tr>
</tbody>
</table>

## Áreas de trabalho e partições {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaços de trabalho e partições (se aplicável)</td>
    <td><li>Determine o número de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> espaços de trabalho</a> e/ou partições que sua organização precisa ter e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">quantos usuários têm acesso a cada espaço de trabalho.</a></li>
    <li>Defina o objetivo principal de cada espaço de trabalho e partição.</li>
    <li>Defina o relacionamento entre seus espaços de trabalho e partições.</li></td>
  </tr>
  <tr>
    <td>Documentação</td>
    <td><li>Documente como os espaços de trabalho são definidos e como eles se relacionam com as partições de banco de dados (por exemplo, um espaço de trabalho Global que mostra todos vs. setores de negócios).</li>
    <li>Importar novos registros para a partição apropriada.</li>
    <li>Defina o valor no CRM que coloca os usuários na partição apropriada.</li></td>
  </tr>
</tbody>
</table>

## Configurações da campanha inteligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Configurações da campanha inteligente</td>
    <td><li>Adicionar um <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">restrição no tamanho da Campanha inteligente</a>, evitando o envio por email de todo o banco de dados.</li></td>
  </tr>
</tbody>
</table>

## Configurações de e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Padrões de email</td>
    <td><li>Em Domínio de marca, selecione seu domínio e adicione seu CNAME de email. Isso deve estar no formato: [EmailTrackingCNAME].[Domínio da empresa].com.</li>
    <li><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Entre em contato com o Suporte da Marketo</a> para protegê-la com uma provisão de Certificado SSL. Esse processo pode levar até 3 dias úteis para ser concluído.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Configurar SPF e DKIM</a> para capacidade de entrega de email.</li></td>
  </tr>
</tbody>
</table>

## Limites de comunicação {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de comunicação</td>
    <td><li>Iniciar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">limites de comunicação</a>.</li>
    <li>Determine se sua empresa requer uma política de limites de comunicação.</li></td>
  </tr>
</tbody>
</table>

## Tags {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canais</td>
    <td><li>Definir como usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank">canais</a>.</li></td>
  </tr>
  <tr>
    <td>Tags</td>
    <td><li>Definir como usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Calendário (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank">Emitir vagas do Calendário de marketing</a> a quem precisa de acesso.</li>
    <li>Configurar o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank">Calendário</a>.</li></td>
  </tr>
</tbody>
</table>

## Gerenciamento de bancos de dados {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gerenciamento de campos</td>
    <td><li>Implementar uma convenção de nomenclatura para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">campos personalizados</a> (por exemplo, começando com "MKTO").</li>
    <li>Seja seletivo quanto aos campos sincronizados. Quanto mais campos você sincronizar, mais lento será o ciclo de sincronização.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Bloquear atualizações de campos</a> você deseja gravar em uma única vez (por exemplo, fonte de lead original, detalhes da fonte de lead original, campos de UTM de primeiro contato etc.).</li></td>
  </tr>
  <tr>
    <td>Atividades personalizadas</td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Atividades personalizadas</a> que são específicos para a sua empresa.</li></td>
  </tr>
  <tr>
    <td>Objetos personalizados</td>
    <td><li>Analise quantas <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Objetos personalizados</a> você precisa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Sincronizar esses Objetos Personalizados com seu CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## Integrações {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>Iniciar Sincronização do CRM. Escolha uma das opções a seguir, dependendo do CRM que sua empresa usa: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>.</li>
    <li>Identifique o tipo de acesso necessário para acessar seu CRM.</li>
    <li>Identifique o administrador do CRM para solucionar problemas.</li></td>
  </tr>
  <tr>
    <td>Páginas de aterrissagem</td>
    <td>OBSERVAÇÃO: você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial. <br>Configure seu domínio de landing page com um <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">CNAME</a> e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">inserir informações de domínio e página</a>. Deve estar no formato: [LandingPageCNAME].[DomínioDaEmpresa].com <br>Escolha um CNAME para suas landing pages. Alguns exemplos: <br>* **ir**.[DomínioDaEmpresa].com <br>* **www2**.[DomínioDaEmpresa].com <br>* **lp**.[DomínioDaEmpresa].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">Entre em contato com o Suporte da Marketo</a> para iniciar o processo de provisionamento de um Certificado SSL. Esse processo pode levar até 3 dias úteis para ser concluído. <br>DICA: Mantenha curto! URLs mais curtos são mais fáceis de lembrar. Sugerimos "go" como o domínio. <br>Adicione o código de rastreamento de análise (por exemplo, Google Analytics ou Adobe Analytics) aos modelos de página de aterrissagem. </td>
  </tr>
  <tr>
    <td>Munchkin</td>
    <td>OBSERVAÇÃO: se você for um cliente do Launch Pack, ignore esta etapa. Seu consultor fornecerá a você instruções do código Munchkin em seu documento de instruções de configuração de TI.
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html">Adicionar código de rastreamento do Munchkin</a> ao seu site. O código do Munchkin pode ser <a href="https://developers.marketo.com/javascript-api/lead-tracking/">codificado</a> ou implantado pelo Google Tag Manager.</li></td>
  </tr>
  <tr>
    <td>Serviços da Web</td>
    <td><li>Determine os usuários/aplicativos que podem fazer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">Chamadas de API</a> em sua instância.</li>
    <li>Revise todos os aplicativos que farão chamadas de API e determine se é necessário aumentar ou diminuir as chamadas de API.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configurar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> serviços para sua empresa. Cada LaunchPoint deve ser combinado com um usuário único da API para ajudar na solução de problemas.</li></td>
  </tr>
  <tr>
    <td>Webinars interativos (se aplicável)</td>
    <td>OBSERVAÇÃO: os webinários interativos são provisionados somente para instâncias de Produção.
    <li>Para criar Webinars interativos, o recurso de webinário integrado, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">adicionar usuários à seção "Usuário"</a> na guia Webinar interativo.</li></td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (se aplicável)</td>
    <td>Para usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html">Dynamic Chat</a>, o canal nativo de automação de conversas no Marketo Engage, prossiga com a configuração de permissões do usuário, seguindo as etapas abaixo no <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador de sistema da organização Adobe. Contato <a href="https://helpx.adobe.com/contact.html">Atendimento ao cliente Adobe</a> para descobrir quem na sua organização tem privilégios de administrador no console. <br>Aceitar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">o convite 'Dynamic Chat Product Admin'</a>. A variável <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">email de boas-vindas</a> é enviado quando o Dynamic Chat está ativado na sua instância Marketo Engage e você é designado como um Administrador do sistema.  <br>Atribua todos os usuários apropriados a um Perfil de produto do Dynamic Chat no Adobe Admin Console. <br>Se um usuário indesejável for adicionado a vários perfis de produto, você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Dynamic Chat. <br>Você pode <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">editar perfis de produto no Dynamic Chat</a> e criar um perfil personalizado com um conjunto personalizado de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">permissões disponíveis em sua assinatura</a>. <br>Atribuir usuários a <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Funções de "Dynamic Chat de acesso"</a> em Marketo Engage/Admin/Usuários e funções. </td>
  </tr>
  <tr>
    <td>Sales Insight (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Configurar Ação de Insight de Vendas</a> em Sales Insight &gt; Actions Config.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Emitir vagas para os usuários apropriados</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Configurar a API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Personalizar as pontuações dos clientes potenciais</a>.</li></td>
  </tr>
  <tr>
    <td>Conexão de vendas (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Convide os administradores de Marketo Engage apropriados para a instância do Sales Connect</a>.</li>
    <li>Conclua o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">configuração adicional do administrador do Sales Connect</a> no Sales Connect e no Salesforce.</li></td>
  </tr>
</tbody>
</table>

## Baú do tesouro {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Baú do tesouro </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Ativar o Treasure Chest</a> para experimentar os recursos do piloto.</li>
    <li>Determine os recursos que deseja ativar ou desativar.</li></td>
  </tr>
  <tr>
    <td>Inspetor de campanhas </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Ativar o Inspetor de campanha</a> para exibir todas as suas Campanhas inteligentes de uma só vez.</li></td>
  </tr>
</tbody>
</table>
