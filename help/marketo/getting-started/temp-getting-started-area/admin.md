---
description: NOVA ÁREA - Documentação do Marketo - Documentação do produto
title: NOVA ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: c0f0134972138eb4fa3498028a4acf5233dbe2fe
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 7%

---

# NOVA ÁREA: Lista de verificação do administrador {#new-area-admin-checklist}

Abrindo a lixeira

## Funções {#roles}

<table>
<thead>
  <tr>
    <th>Área </th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Funções </td>
    <td><li>Revise as funções pré-criadas e confirme quais permissões/acesso cada função tem.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Criar uma nova função</a> ou <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">editar as funções</a> com base nas necessidades de sua organização e na frequência com que os usuários fazem logon.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Atribuir usuários às funções apropriadas</a>.</li>
    <li>Depois de atribuir as funções para usuários, revise o número de usuários por função.</li>  <li>Implemente uma função exclusiva para cada usuário da API para facilitar a solução de problemas.</li></td>
  </tr>
  <tr>
    <td>Documentação </td>
    <td>Defina usuários e funções para sua organização. <br>Defina seu processo para adicionar um novo usuário/administrador. </td>
  </tr>
  <tr>
    <td>Sandbox (se aplicável) </td>
    <td>Revise as categorias acima para sua sandbox, se você tiver uma. </td>
  </tr>
</tbody>
</table>

## Espaços de trabalho e partições {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Espaços de trabalho e partições </td>
    <td><li>Determine o número de<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> espaços de trabalho</a> e/ou partições que sua organização precisa ter e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">quantos usuários têm acesso a cada espaço de trabalho.</a></li>
    <li>Defina o objetivo principal de cada espaço de trabalho e partição.</li>
    <li>Defina o relacionamento entre seus espaços de trabalho e partições.</li></td>
  </tr>
  <tr>
    <td>Documentação </td>
    <td><li>Documente como os espaços de trabalho são definidos e como eles se relacionam com as partições de banco de dados (ou seja, um espaço de trabalho global que vê todos, em comparação aos setores de negócios).</li>
    <li>Importar novos registros para a partição apropriada.</li>
    <li>Defina o valor no CRM que coloca os usuários na partição apropriada.</li></td>
  </tr>
</tbody>
</table>

## Configurações da campanha inteligente {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Configurações da campanha inteligente </td>
    <td><li>Adicionar um <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restrição no tamanho da Campanha inteligente</a>, evitando o envio acidental por email de todo o banco de dados.</li>
    <li>Ativar restrições de pessoa para Campanhas inteligentes</li></td>
  </tr>
</tbody>
</table>

## Configurações de e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Padrões de email</td>
    <td><li>Em Domínio de marca, selecione seu domínio e adicione seu CNAME de email. Isso deve estar no formato: [EmailTrackingCNAME].[Domínio da empresa].com.</li></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configurar SPF e DKIM</a> para capacidade de entrega de email.</li></td>
  </tr>
</tbody>
</table>

## Limites de comunicação {#communication-limits}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limites de comunicação</td>
    <td><li>Local <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Limites de comunicação</a>.</li>
    <li>Determine se sua empresa requer uma política de limites de comunicação.</li></td>
  </tr>
</tbody>
</table>

## Tags {tags}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canais</td>
    <td><li>Definir como usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">canais</a>.</li></td>
  </tr>
  <tr>
    <td>Tags </td>
    <td><li>Definir como usar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tags</a>.</li></td>
  </tr>
  <tr>
    <td>Calendário (se aplicável) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Emitir vagas do Calendário de marketing</a> a quem precisa de acesso.</li> 
    <li>Configurar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendário</a>.</li></td>
  </tr>
</tbody>
</table>

## Gerenciamento de bancos de dados {#database-management}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gerenciamento de campos</td>
    <td><li>Implementar a convenção de nomenclatura para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">campos personalizados.</a> Por exemplo, comece com "MKTO".</li>
    <li>Seja seletivo quanto aos campos sincronizados. Quanto mais campos você sincronizar, mais lento será o ciclo de sincronização.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Bloquear atualizações de campos</a> você deseja gravar no uma vez (ou seja, fonte de lead original, detalhes da fonte de lead original, campos de UTM de primeiro contato etc.).</li></td>
  </tr>
  <tr>
    <td>Atividades personalizadas </td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank" rel="noopener noreferrer">Atividades personalizadas</a> que são específicos para a sua empresa.</li></td>
  </tr>
  <tr>
    <td>Objetos personalizados </td>
    <td><li>Analise quantas <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank" rel="noopener noreferrer">Objetos personalizados</a> você precisa.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank" rel="noopener noreferrer">Sincronizar esses Objetos Personalizados com seu CRM</a>.</li></td>
  </tr>
</tbody>
</table>

## Integrações {#integrations}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Iniciar Sincronização do CRM. Escolha uma das opções a seguir, dependendo do CRM que sua empresa usa: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank" rel="noopener noreferrer">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank" rel="noopener noreferrer">Microsoft Dynamics</a>.</li>
    <li>Identifique o tipo de acesso necessário para acessar seu CRM.</li>
    <li>Identifique o administrador do CRM para solucionar problemas.</li></td>
  </tr>
  <tr>
    <td>Sales Insight (se aplicável)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank" rel="noopener noreferrer">Configurar o Sales Insight.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank" rel="noopener noreferrer">Emita vagas para os usuários apropriados.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank" rel="noopener noreferrer">Configurar a API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank" rel="noopener noreferrer">Personalizar as pontuações dos clientes potenciais.</a></li></td>
  </tr>
</tbody>
</table>
