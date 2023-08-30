---
description: Herdar documento 1 - Documentação do Marketo - Documentação do produto
title: Herdar Doc 1
hide: true
hidefromtoc: true
source-git-commit: 8d9ea20f04ec6320b31c2d6000240b72a45be959
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 4%

---

# Herdar Doc 1 {#inherit-doc-1}

As listas de verificação abaixo (listas de verificação subsequentes vinculadas na parte inferior de cada artigo) foram colocadas junto com a entrada de especialistas do Marketo para ajudar você a se familiarizar rapidamente. Você também pode baixar as listas de verificação e acompanhar o progresso.

>[!TIP]
>
>Se você for um novo usuário de Marketo Engage e não estiver familiarizado com muitos dos termos, verifique a [Glossário do Marketo](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Adobe Admin Console {#adobe-admin-console}

<table> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th> 
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Assinatura</td> 
   <td><li>Sua assinatura do Marketo Engage está ativada? <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Sistema Adobe Identity Management</a> (Adobe IMS) ainda? 
<br/>
Em caso afirmativo, você recebeu uma função de "Administrador de produto do Adobe Admin Console" por seu "Administrador de sistema do Adobe Admin Console"? Se você não tem certeza de quem na sua organização tem privilégios de administrador no console, entre em contato com <a href="https://helpx.adobe.com/contact.html" target="_blank">Atendimento ao cliente Adobe</a>.  
<br/>Caso contrário, você prosseguirá com a <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">experiência de funções e permissões do usuário herdadas</a> em Marketo Engage &gt; Admin &gt; Usuários e funções até que sua assinatura seja renovada.</li></td>
  </tr>
  <tr> 
   <td>Perfil do produto</td> 
   <td>(Assinaturas no Adobe IMS <b>somente</b>)
<p>
<li>Você recebeu uma função de "Administrador de produto do Marketo Engage" em Marketo Engage/Administrador/Usuários e funções?</li> 
<li>Você atribuiu o Marketo Engage a todos os perfis de produto dos usuários apropriados na Adobe Admin Console?
<br/>Caso contrário, certifique-se de atribuir o Marketo Engage ao perfil de produto do Adobe IMS antes de atribuir suas funções no Marketo Engage/Admin/Usuários e funções.</li>
<p>Observação: se sua assinatura tiver mais de 75 usuários e tiver acabado de migrar para o Adobe IMS, você terá a opção de selecionar usuários para migrar em lotes e administrar sua Adobe Identificar em grupos ou todos de uma só vez. Leia mais sobre o que esperar do <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md#prepare-users-for-migration-day" target="_blank">Dia da migração do Adobe IMS</a>.</td>
  </tr>
  <tr> 
   <td>API de gerenciamento de usuários</td> 
   <td><li>Sua assinatura do usou alguma API de gerenciamento de usuários do Marketo?
<br/>Em caso afirmativo, será necessário usar <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">APIs do Adobe IMS</a> para convidar, atualizar e excluir usuários daqui em diante.</li></td>
  </tr>
 </tbody> 
</table>

## Usuários e funções {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Quantos usuários</a> existem?</li>
<li>Há usuários que devem ser expirados?</li>
<li>Sua empresa tem políticas para excluir usuários?</li> 
<li>Quantos usuários <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Permissões de administrador</a>?</li>
<li>Se algum desses usuários for alterado para <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">outras funções?</a></li> 
<li>Quem são os usuários da API nessa instância?</li></td>
  </tr>
  <tr> 
   <td>Funções</td> 
   <td><li>Quantas funções existem?</li>  
<li>O que <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permissões/acesso</a> cada função tem? Algum deve ser ajustado?</li>
<li>Há quantos usuários por função?</li>
<li>Com que frequência os usuários <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">efetuando login</a>?</li>
<li>Cada usuário da API tem sua <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">função de usuário própria</a>? Caso contrário, considere implementar isso para facilitar a solução de problemas.</li> 
<li>As funções e permissões do usuário estão alinhadas aos dados corporativos? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">políticas de privacidade</a>?</li></td>
  </tr>
  <tr> 
   <td>Usuários de suporte</td> 
   <td><li>Você configurou o <a href="/help/marketo/getting-started/setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contatos autorizados</a> no Portal de suporte?</li></td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Os usuários e as funções estão claramente definidos em sua organização?</li>
<li>Qual é o seu processo para adicionar um novo usuário/administrador?</li></td>
  </tr>
  <tr> 
   <td>Sandbox (se aplicável)</td> 
   <td><li>Você tem um <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instância de sandbox</a>?
   <br/>  Em caso afirmativo, revise as categorias acima para sua sandbox.</li>
<li>É <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Importação do programa</a> vinculado à sua sandbox?</li></td>
  </tr>
 </tbody> 
</table>

## Trila de auditoria {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Trila de auditoria</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Quem está trabalhando</a> no caso?</li></td>
  </tr>
 </tbody> 
</table>

## Espaços de trabalho e partições {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Espaços de trabalho e partições</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Espaços de Trabalho e/ou Partições</a> você tem?</li>
<li>Qual é o objetivo principal de cada espaço de trabalho e partição?</li>
<li>Faça o seu <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Espaços de trabalho</a> ou <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partições</a> precisa ser auditada/alterada?</li>
<li>Qual é a relação entre seus Espaços de trabalho e Partições?</li>
<li>Quantos usuários <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">ter acesso</a> para cada Espaço de trabalho?</li></td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Como os Espaços de Trabalho e as Partições são definidos?</li>
<li>Qual é o seu processo para adicionar espaços de trabalho à sua instância ou adicionar usuários a um espaço de trabalho?</li></td>
  </tr>
 </tbody> 
</table>

## Campanhas inteligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Configurações da campanha inteligente</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Você tem uma restrição?</a> no tamanho do Smart Campaign? 
   <br/>Caso contrário, considere adicionar um. Recomendamos limitar os limites do Smart Campaign a 25% do seu banco de dados para evitar comunicação excessiva ou o processamento de todo o seu banco de dados em workflows. Isso não só protege a sua marca, mas ajuda a proteger o desempenho da sua instância.</li></td>
  </tr>
 </tbody> 
</table>

## Limites de comunicação {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Limites de comunicação</td> 
   <td><li>Há <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limites de comunicação</a> em vigor? Sua empresa tem políticas em que os limites de comunicação podem ser necessários?</li>
<p>Observação: recomendamos limitar sua comunicação a 1 por dia e 3 por 7 dias, com <b>não</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operacional</a> emails bloqueados.</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-new-program-tag-and-tag-values.md" target="_blank">Quantas tags</a> existem? Quantas tags estão em uso? É necessário adicionar alguma?</li>
<li>As tags são necessárias em seus programas?</li></td>
  </tr>
  <tr> 
   <td>Canais</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Quantos canais</a> existem? Quantas estão em uso?</li>
<li>São todos <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">status do programa do canal apropriado</a>? Eles mostram progressão dentro do programa?</li>
<li>Seus canais estão relacionados a tipos de programas específicos?</li>
<li>Quais status são considerados bem-sucedidos para cada canal? Eles se alinham às suas metas de marketing?</li>
<li>O canal Operacional está sendo usado adequadamente?</li>
<li>Para o Advanced Report Builder (Revenue Cycle Explorer/RCE), o comportamento da análise do seu canal está definido para ser alinhado às práticas do seu programa que incorporam o custo do período?</li></td>
  </tr>
  <tr> 
   <td>Calendário de marketing (se aplicável)</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">tipos de entrada de calendário</a> existem? Elas ainda são relevantes?</li></td>
  </tr>
 </tbody> 
</table>

## Gerenciamento de bancos de dados {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Gerenciamento de campos</td> 
   <td><li>Há quantos campos? 
   <br/>Clique em <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exportar nomes de campo</a> para revisar uma lista de campos, campos personalizados e seus nomes de API.</li>
<li>Quantas <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campos personalizados</a> existem?</li>
<li>Quantos campos estão sendo usados? 
<br/>Selecionar <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Exportação Usada Por</a> no menu suspenso Ações de campo para revisar ativos relacionados de um campo.</li>
<li>Quantos campos são sincronizados entre o Marketo Engage e o CRM?</li>
<li>Os campos do CRM estão sincronizados com os objetos apropriados?</li>
<li>Existe um <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">conjunto de exibição personalizado</a> para detalhes da pessoa? Deveria haver?</li>
<li>Você tem uma convenção de nomenclatura para seus campos com base na origem? 
<br/>Caso contrário, considere implementar isso.</li>
<li>Há algum campo <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">bloqueado</a>? 
<br/>Em caso afirmativo, certifique-se de entender por que eles estão.</li></td>
  </tr>
  <tr> 
   <td>Atividades personalizadas</td> 
   <td><li>Há algum <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">atividades personalizadas</a>?
<br/>Em caso afirmativo, clique nessas atividades para entender quais atividades não estão relacionadas a um formulário, email ou página de aterrissagem do Marketo.</li></td>
  </tr>
  <tr> 
   <td>objetos  personalizados</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">objetos personalizados</a> existem? Como eles são sincronizados ao seu CRM?</li>
<li>Como esses objetos personalizados estão sendo utilizados pelos seus programas e consultas de lista?</li></td>
  </tr>
 </tbody> 
</table>

## Integrações {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>A qual CRM você está sincronizando? Salesforce? MS Dynamics? Veeva?</li>
<li>Você está utilizando um <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">sincronização personalizada</a>?</li>
<li>[Somente Salesforce] Sua instância tem Filtros de sincronização personalizados implementados? 
<p>Observação: entre em contato com o Suporte da Marketo para identificar Filtros de sincronização personalizados ou solicitar a implementação de uma Regra de sincronização personalizada.</li></td>
  </tr>
  <tr> 
   <td>Páginas</td> 
   <td><li>O que é o <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">domínio definido como</a>?</li>
   <li>Como é definida a página inicial?</li>
<li>O que é o <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">fallback definido como</a>?</li>
<li>O preenchimento prévio do formulário está ativado?</li>
<li>São <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">URLs personalizados</a> habilitado?</li>
<li>Há regras configuradas para <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">redirecionamentos</a>?</li>
<li>Você tem aliases de domínio em vigor? Você está rastreando a forma como está utilizando seus aliases de domínio?</li>
<li>É <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Domínios seguros para páginas de aterrissagem</a> habilitado? 
<br/>Confirme se os ativos da página de aterrissagem contêm um URL "http".</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>É seu <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Código de rastreamento do Munchkin</a> no seu site (não no Marketo)?</li>
<li>É um <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track (Não rastrear)</a> Solicitação de navegador ativada?</li>
<li>É seu <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">API do Munchkin</a> configurado? 
<p>Dica: se você não tiver uma documentação sobre onde está o código do munchkin no seu site, poderá ver todos os URLs criando uma <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Relatório de atividades da página da Web</a>.</li></td>
  </tr>
  <tr> 
   <td>Serviços da Web</td> 
   <td><li>São <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">Restrições de IP</a> habilitado? Deveriam ser?</li>
<li>Quais usuários/aplicativos estão fazendo chamadas de API em sua instância?</li>
<li>Você está atingindo ou perto de atingir o limite da API? 
<br/>Nesse caso, considere aumentá-lo ou auditar sua instância para desativar essas chamadas de API.</li></td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (se aplicável)</td> 
   <td><li>Tem o <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Pacote MSI instalado</a>?</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">atualizado para a versão mais recente do Sales Insight</a>?</li>
<li>Você concluiu a configuração do Sales Insight? <br/>Usuários Enterprise/Unlimited <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">clique aqui</a>, Usuários profissionais <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">clique aqui</a>.</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">acesso concedido aos usuários</a> com base no número de vagas que você comprou?</li>
<li>São <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Estrelas e chamas</a> personalizado?</li></td>
  </tr>
  <tr> 
   <td>Ponto de lançamento (se aplicável)</td> 
   <td><li>Quais serviços você configurou (por exemplo, <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>, etc.)? Algum está próximo da expiração?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Quantas chamadas de API</a> suas integrações estão usando o?</li>
<li>Você tem as integrações certas em vigor para seus casos de uso?</li></td>
  </tr>
  <tr> 
   <td>Webhooks (se aplicável)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Quais conexões</a> você configurou?</li>
<li>Não estão mais em uso?</li></td>
  </tr>
  <tr> 
   <td>Aplicativos móveis (se aplicável)</td> 
   <td><li>Qual <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">aplicativos móveis</a> você tem?</li>
<li>Possuir <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">dispositivos de teste</a>  foi adicionado?</li></td>
  </tr>
 </tbody> 
</table>

## Baú do tesouro {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Baú do tesouro</td> 
   <td><li>O que está ativado no <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Tórax Tesouro</a>?</li>
<li>Há recursos que devem ser ativados ou desativados?</li></td>
  </tr>
  <tr> 
   <td>Inspetor de campanhas</td> 
   <td><li>É <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Inspetor de campanha</a> ligado?
<br/>Caso contrário, considere ativá-la para identificar facilmente quais campanhas são: ativas, sincronizando com seu CRM e/ou excluindo registros.</li></td>
  </tr>
 </tbody> 
</table>

## Alertas e atualizações {#alerts-and-updates}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:25%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Atualizações de status do Marketo Engage</td> 
   <td><li>Sua instância está inscrita? <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Atualizações de status do Marketo Engage</a>?</li></td>
  </tr>
  <tr> 
   <td>Alertas</td> 
   <td><li>Há algum <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">alertas ativos</a> sendo enviado para equipes internas do Marketo Engage?</li>
<li>Em caso afirmativo, esses alertas estão funcionando adequadamente?</li></td>
  </tr>
  <tr> 
   <td>Notificações</td> 
   <td><li>Você está inscrito no administrador apropriado? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notificações</a>?</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[Auditoria de uma instância herdada: Base de dados ►](/help/marketo/getting-started/inheriting-a-marketo-instance/new-inherit-doc-2.md)
