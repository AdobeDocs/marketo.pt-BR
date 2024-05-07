---
description: Configure a seção Admin para sua nova instância do Marketo Engage.
title: Novas Práticas Recomendadas Da Instância - Lista De Verificação Da Seção Do Administrador
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 6%

---

# Novas Práticas Recomendadas Da Instância: Lista De Verificação Da Seção Admin {#new-instance-best-practices-admin-section-checklist}

Como novo administrador navegando em uma nova instância do Marketo Engage, aplique a lista de verificação abaixo para ajudar a orientá-lo pelo processo de implementação. Como em todos esses guias, você também pode [baixar as listas de verificação](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e acompanhe seu progresso.

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
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Atribuir usuários às funções apropriadas</a>. Os usuários devem ser adicionados à assinatura no Adobe Admin Console antes de conceder suas funções em "Funções". Consulte a seção Usuários no <a href="/help/marketo/getting-started/initial-setup/user-setup.md">Lista de verificação de configuração inicial</a>.</li>
    <li>Depois de atribuir as funções para usuários, analise o número de usuários por função.</li>
    <li>Implemente uma função exclusiva para cada usuário da API para facilitar a solução de problemas.</li></td>
  </tr>
  <tr>
    <td>Sandbox (se aplicável)</td>
    <td><li>Revise as categorias acima para seu <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandbox</a>.</li></td>
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
    <td><li>Implementar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank">limites de comunicação</a>.</li>
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
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Atividades personalizadas</a> que são específicos para a sua empresa.</li></td>
  </tr>
  <tr>
    <td>Objetos personalizados</td>
    <td><li>Analise quantas <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Objetos personalizados</a> você precisa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Sincronizar esses objetos personalizados</a> ao seu CRM.</li></td>
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
    <td><li>Identifique as permissões necessárias para acessar seu CRM.</li>
    <li>Identifique o administrador do CRM para solucionar problemas.</li></td>
  </tr>
  <tr>
    <td>Serviços da Web</td>
    <td><li>Determine os usuários/aplicativos que podem fazer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">Chamadas de API</a> em sua instância.</li>
    <li>Revise todos os aplicativos que farão chamadas de API e determine se é necessário aumentar ou diminuir as chamadas de API.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configurar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> serviços para sua empresa. Cada LaunchPoint deve ser combinado com um usuário único da API para ajudar na solução de problemas.</li></td>
  </tr>
  <tr>
    <td>Webinars interativos (se aplicável)</td>
    <td><li>Para criar Webinars interativos, o recurso de webinário integrado Marketo Engage, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">adicionar usuários à seção "Usuário"</a> na guia Webinar interativo.</li>
    <p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: os webinários interativos são provisionados somente para instâncias de Produção.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (se aplicável)</td>
    <td><li>Atribuir usuários a <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank">Funções de "Dynamic Chat de acesso"</a> em Marketo Engage &gt; Administrador &gt; Usuários e funções.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Configurar Ação de Insight de Vendas</a> em Sales Insight &gt; Actions Config.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Emitir vaga</a> aos usuários apropriados.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Configurar a API</a>.</li>
    <li>Personalize o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">pontuações de lead</a>.</li></td>
  </tr>
  <tr>
    <td>Conexão de vendas (se aplicável)</td>
    <td><li>Convide os administradores de Marketo Engage apropriados para o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">Instância do Sales Connect</a>.</li>
    <li>Conclua o <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">configuração adicional do administrador do Sales Connect</a> no Sales Connect e no Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhooks (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Criar todos os webhooks necessários</a> para sua empresa.</li>
    </td>
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
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Ativar o Treasure Chest</a> para experimentar os recursos do piloto.</li>
    <li>Determine os recursos que deseja ativar ou desativar.</li></td>
  </tr>
  <tr>
    <td>Inspetor de campanhas </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Ativar o Inspetor de campanha</a> para exibir todas as suas Campanhas inteligentes em um único local.</li></td>
  </tr>
</tbody>
</table>
