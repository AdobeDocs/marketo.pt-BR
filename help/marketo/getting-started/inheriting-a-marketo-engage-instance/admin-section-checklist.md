---
description: Lista de verificação de administrador de instância herdada - Documentação do Marketo - Documentação do produto
title: Lista de Verificação de Administração de Instância Herdada
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 3%

---

# Instância herdada: lista de verificação da seção do administrador {#inherited-instance-admin-section-checklist}

As listas de verificação abaixo (listas de verificação subsequentes vinculadas na parte inferior de cada artigo) foram criadas pelo Adobe Professional Services com a entrada de especialistas do Marketo para ajudar você a se familiarizar rapidamente. Também é possível [baixar as listas de verificação](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) e acompanhe seu progresso.

>[!TIP]
>
>Se você for um novo usuário de Marketo Engage e não estiver familiarizado com muitos dos termos, verifique a [Glossário do Marketo Engage](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Isso só se aplica a assinaturas Marketo Engage integradas ao [Sistema Adobe Identity Management (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Se sua assinatura ainda não tiver integrado o Adobe IMS, continue com o [experiência de funções e permissões do usuário herdadas](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} em Marketo Engage > Administrador > Usuários e funções.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Administrador de assinatura e produto Marketo Engage</td> 
   <td><li>Sua assinatura do Marketo Engage foi migrada para <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> ainda? 
<br/>     Em caso afirmativo, você recebeu uma função de "Administrador de produto do Adobe Admin Console" por seu "Administrador de sistema do Adobe Admin Console"? Se você não tem certeza de quem na sua organização tem privilégios de administrador no console, entre em contato com <a href="https://helpx.adobe.com/contact.html" target="_blank">Atendimento ao cliente Adobe</a>.</li>
<li>Você aceitou o convite 'Marketo Engage Product Admin'? O email é enviado quando a função é atribuída na Adobe Admin Console.
<br/>     Caso contrário, procure a variável <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">email de boas-vindas</a> na sua caixa de entrada e aceite o convite para ativar sua Adobe ID.</li></td>
  </tr>
  <tr> 
   <td>Perfil de produto</td> 
   <td><li>Todos os usuários apropriados estão atribuídos ao perfil de produto Marketo Engage no Adobe Admin Console?
<br/>     Caso contrário, verifique se <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">adicionar e/ou remover usuários</a> dos perfis de produto Marketo Engage na Adobe Admin Console. Não é possível atribuir funções de usuários em Marketo Engage &gt; Admin &gt; Usuários e funções se eles forem adicionados a um Perfil de produto.</li>
<p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: se um usuário indesejado for adicionado a vários perfis de produto, você deverá remover o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Marketo Engage.</td>
  </tr>
  <tr> 
   <td>API de gerenciamento de usuários</td> 
   <td><li>Sua assinatura usa alguma API de gerenciamento de usuários do Marketo?
<br/>     Em caso afirmativo, será necessário usar <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">APIs do Adobe IMS</a> para convidar, atualizar e excluir usuários daqui em diante.</li>
<p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: o "Gerenciamento de funções" permanece no Marketo Engage e as APIs de gerenciamento de usuários do Marketo ainda podem ser usadas para gerenciamento de funções.</td>
  </tr>
 </tbody> 
</table>

## Usuários e funções {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: se sua assinatura já estiver no Adobe IMS, prossiga para a seguinte revisão do gerenciamento de usuários no Adobe Admin Console. Caso contrário, acesse Administrador &gt; Usuários e funções &gt; Usuários no Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Quantos usuários</a> existem?</li>
<li>Há usuários que devem ser <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">removido</a>?</li>
<li>Sua empresa tem políticas para excluir usuários?</li> 
<li>Quantos usuários <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Permissões de administrador</a>?</li>
<li>Se algum desses usuários for alterado para <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">outras funções?</a></li> 
<li>Quem são os <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">Usuários da API</a> neste caso?</li></td>
  </tr>
  <tr> 
   <td>Funções</td> 
   <td><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: se você usa o Marketo com o Adobe Identity ou não, prossiga com a revisão das permissões de função no Marketo Engage em Admin &gt; Usuários e funções &gt; Funções.
   <p><li>Quantas funções existem?</li>  
<li>O que <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permissões/acesso</a> cada função tem? Algum deve ser ajustado?</li>
<li>Há quantos usuários por função?</li>
<li>Com que frequência os usuários <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">efetuando login</a>?</li>
<li>Cada usuário da API tem sua <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">função de usuário própria</a>? Caso contrário, considere implementar isso para facilitar a solução de problemas.</li> 
<li>As suas funções e permissões de usuário estão alinhadas às suas políticas corporativas de privacidade de dados para fins de conformidade normativa (por exemplo, <a href="https://gdpr-info.eu/" target="_blank">GDPR</a>)? Os dados corporativos <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">políticas de privacidade</a> permitir que os usuários baixem e compartilhem dados de usuários do Marketo Engage? O negócio de permissão é necessário?</li></td>
  </tr>
  <tr> 
   <td>Usuários de suporte</td> 
   <td><li>Você configurou o <a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contatos autorizados</a> no Portal de suporte?</li></td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Os usuários e as funções estão claramente definidos em sua organização?</li>
<li>Qual é o seu processo para adicionar um novo usuário/administrador?</li></td>
  </tr>
  <tr> 
   <td>Sandbox (se aplicável)</td> 
   <td><li>Você tem um <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instância de sandbox</a>?
   <br/>     Em caso afirmativo, revise as categorias acima para sua sandbox.</li>
<li>É <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Importação do programa</a> vinculado à sua sandbox?</li></td>
  </tr>
 </tbody> 
</table>

## Trilha de auditoria {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Trilha de auditoria</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Quem está trabalhando</a> no caso?</li></td>
  </tr>
 </tbody> 
</table>

## Áreas de trabalho e partições {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Áreas de trabalho e partições</td> 
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
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Campanhas inteligentes</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Você tem uma restrição?</a> no tamanho do Smart Campaign? 
   <br/>     Caso contrário, considere adicionar um. Recomendamos limitar os limites do Smart Campaign a 25% do seu banco de dados para evitar comunicação excessiva ou o processamento de todo o seu banco de dados em workflows. Isso não só protege a sua marca, mas ajuda a proteger o desempenho da sua instância.</li></td>
  </tr>
 </tbody> 
</table>

## Limites de comunicação {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Limites de comunicação</td> 
   <td><li>Há <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limites de comunicação</a> em vigor? Sua empresa tem políticas em que os limites de comunicação podem ser necessários?</li>
<p><img src="assets/note-icon.png" alt="ícone de nota"> NOTA: recomendamos limitar sua comunicação a uma por dia e três a cada sete dias, com <b>não</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operacional</a> emails bloqueados.</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Quantas tags</a> existem? Quantas tags estão em uso? É necessário adicionar alguma?</li>
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
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Gerenciamento de campos</td> 
   <td><li>Há quantos campos? 
   <br/>     Clique em <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Exportar nomes de campo</a> para revisar uma lista de campos, campos personalizados e seus nomes de API.</li>
<li>Quantas <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campos personalizados</a> existem?</li>
<li>Quantos campos estão sendo usados? 
<br/>     Selecionar <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Exportação Usada Por</a> no menu suspenso Ações de campo para revisar ativos relacionados de um campo.</li>
<li>Quantos campos são sincronizados entre o Marketo Engage e o CRM?</li>
<li>Os campos do CRM estão sincronizados com os objetos apropriados?</li>
<li>Existe um <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">conjunto de exibição personalizado</a> para detalhes da pessoa? Deveria haver?</li>
<li>Você tem uma convenção de nomenclatura para seus campos com base na origem? 
<br/>     Caso contrário, considere implementar isso.</li>
<li>Há algum campo <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">bloqueado</a>? 
<br/>     Em caso afirmativo, certifique-se de entender por que eles estão.</li></td>
  </tr>
  <tr> 
   <td>Atividades personalizadas</td> 
   <td><li>Há algum <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">atividades personalizadas</a>?
<br/>     Em caso afirmativo, clique nessas atividades para entender quais atividades não estão relacionadas a um formulário, email ou página de aterrissagem do Marketo.</li></td>
  </tr>
  <tr> 
   <td>Objetos personalizados</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">objetos personalizados</a> existem? Como eles são sincronizados ao seu CRM?</li>
<li>Como esses objetos personalizados estão sendo utilizados pelos seus programas e consultas de lista?</li></td>
  </tr>
 </tbody> 
</table>

## Email {#email}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Configurações padrão de email</td> 
   <td><li>Em Admin &gt; Email, todas as configurações padrão estão atualizadas (por exemplo, <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">email/rótulo "de"</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">domínio de marca</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">mensagem de cancelamento de inscrição</a>, etc.)?</li></td>
  </tr>
 </tbody> 
</table>

## Integrações {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th>
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>A qual CRM você está sincronizando? Salesforce? MS Dynamics? Veeva?</li>
<li>Você está utilizando um <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">sincronização personalizada</a>?</li>
<li>[Somente Salesforce] Sua instância tem Filtros de sincronização personalizados implementados? 
<p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: Entre em contato com o Suporte da Marketo para identificar Filtros de sincronização personalizados ou solicitar a implementação de uma Regra de sincronização personalizada.</li></td>
  </tr>
  <tr> 
   <td>Páginas de aterrissagem</td> 
   <td><li>O que é o <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">domínio definido como</a>?</li>
   <li>Como é definida a página inicial?</li>
<li>O que é o <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">fallback definido como</a>?</li>
<li>O preenchimento prévio do formulário está ativado?</li>
<li>São <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">URLs personalizados</a> habilitado?</li>
<li>Há regras configuradas para <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">redirecionamentos</a>?</li>
<li>Você tem aliases de domínio em vigor? Você está rastreando a forma como está utilizando seus aliases de domínio?</li>
<li>É <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Domínios seguros para páginas de aterrissagem</a> habilitado? 
<br/>     Confirme se os ativos da página de aterrissagem contêm um URL "http".</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>É seu <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Código de rastreamento do Munchkin</a> em seu site (não é uma página de aterrissagem do Marketo Engage)?</li>
<li>É um <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track (Não rastrear)</a> Solicitação de navegador ativada?</li>
<li>É seu <a href="https://experienceleague.adobe.com/docs/marketo-developer/marketo/javascriptapi/lead-tracking.html" target="_blank">API do Munchkin</a> configurado? 
<p><img src="assets/tip-icon.png" alt="ícone de dica">DICA: se você não tiver uma documentação sobre onde está o código do munchkin no seu site, poderá ver todos os URLs criando uma <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Relatório de atividades da página da Web</a>.</li></td>
  </tr>
  <tr> 
   <td>Serviços da Web</td> 
   <td><li>São <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">Restrições de IP</a> habilitado? Deveriam ser?</li>
<li>Quais usuários/aplicativos estão fazendo chamadas de API em sua instância?</li>
<li>Você está atingindo ou perto de atingir o limite da API?
<br/>     Nesse caso, considere aumentá-lo ou auditar sua instância para desativar essas chamadas de API.</li></td>
  </tr>
  <tr> 
   <td>Adobe Dynamic Chat (se aplicável)</td> 
<td>Seguindo as etapas abaixo, será necessário acessar o <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. Se ainda não tiver configurado uma Adobe ID, <a href="https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html" target="_blank">saiba como fazer isso aqui</a>.
<br/>
<li>Você aceitou o <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">Administrador de produto do Dynamic Chat</a> convidar? O email é enviado quando o Dynamic Chat está ativado na sua instância do Marketo Engage e você é designado como um Administrador do sistema.
<br/>     Caso contrário, procure o email de boas-vindas em sua caixa de entrada e aceite o convite para configurar seu Adobe ID.</li>   
<li>Você adicionou o <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">usuários desejados</a> ao perfil de produto Dynamic Chat no Adobe Admin Console?
<li>Certifique-se de que os usuários qualificados tenham o Perfil de produto Dynamic Chat adicionado à sua Identidade Adobe. Não é possível atribuir funções de "Dynamic Chat de acesso" em Marketo Engage &gt; Administrador &gt; Usuários e funções se eles forem adicionados a um Perfil de produto.</li>
<li>Na guia "Perfis de produto", as Permissões de perfil padrão estão alinhadas às necessidades da sua organização?<br/> 
Caso contrário, edite as permissões para o perfil específico. </li>
<li>Se você tiver mais de uma assinatura, seus usuários estão sendo adicionados às assinaturas corretas?</li>
<br>
Quando terminar de auditar as configurações Usuários e funções, faça logon no Dynamic Chat para continuar sua auditoria.  
<li>Você <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">conectou sua instância do Marketo Engage</a> para o Dynamic Chat?</li>
<li>Os cinco perfis padrão com permissões predefinidas se aplicam à sua organização?<br/> 
     Caso contrário, você pode <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">editá-los no Dynamic Chat</a>. Também é possível <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">criar um perfil personalizado</a> com um conjunto personalizado de permissões.</li>
<li>Para fornecer aos usuários acesso ao Dynamic Chat, você marcou a opção "Dynamic Chat de acesso" à função de Marketo Engage aplicável em Admin &gt; Usuários e funções &gt; Funções?
<br/><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: as funções de "Administrador" e "Usuário de marketing" devem ter acesso ao Dynamic Chat.</li>
</td>
  </tr>
  <td>Marketo Sales Insight (se aplicável)</td> 
   <td><li>Tem o <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Pacote MSI instalado</a>?</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">atualizado para a versão mais recente do Sales Insight</a>?</li>
<li>Você concluiu a configuração do Sales Insight? <br/>     Usuários Enterprise/Unlimited <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">clique aqui</a>, Usuários profissionais <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">clique aqui</a>.</li>
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
   <th style="width:20%">Área</th>
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
   <th style="width:20%">Área</th>
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
