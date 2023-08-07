---
description: Herdar documento 1 - Documentação do Marketo - Documentação do produto
title: Herdar Doc 1
hide: true
hidefromtoc: true
source-git-commit: 518c6a84dafd0882f1112caa0356f04a772832a1
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 7%

---

# Herdar Doc 1 {#inherit-doc-1}

A auditoria de uma instância herdada pode parecer um...

Você herdou uma instância de Marketo Engage existente de outro administrador? Em caso afirmativo, este artigo é para você...

A lista de verificação abaixo foi colocada junto com a entrada de especialistas do Marketo para ajudar você a se atualizar rapidamente em sua instância herdada...

>[!TIP]
>
>Se você for um novo usuário de Marketo Engage e não estiver familiarizado com muitos dos termos, verifique a [Glossário do Marketo](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Usuários e funções {#users-and-roles}

<table> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td><li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Quantos usuários</a> existem?</li>
<li>Há usuários que devem ser expirados?</li>
<li>Sua empresa tem políticas para excluir usuários?</li> 
<li>Quantos usuários <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Permissões de administrador</a>?</li>
<li>Se algum desses usuários for alterado para <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">outras funções?</a></li> 
<li>Quem são os usuários da API nessa instância?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Funções</td> 
   <td><li>Quantas funções existem?</li>  
<li>O que <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">permissões/acesso</a> cada função tem? Algum deve ser ajustado?</li>
<li>Há quantos usuários por função?</li>
<li>Com que frequência os usuários <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">efetuando login</a>?</li>
<li>Cada usuário da API tem sua <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">função de usuário própria</a>? Caso contrário, considere implementar isso para facilitar a solução de problemas.</li> 
<li>As funções e permissões do usuário estão alinhadas aos dados corporativos? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">políticas de privacidade</a>?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Os usuários e as funções estão claramente definidos em sua organização?</li>
<li>Qual é o seu processo para adicionar um novo usuário/administrador?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Sandbox (se aplicável)</td> 
   <td><li>Você tem um <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">instância de sandbox</a>? Em caso afirmativo, revise as categorias acima para sua sandbox.</li>
<li>É <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Importação do programa</a> vinculado à sua sandbox?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Trila de auditoria {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Trila de auditoria</td> 
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Quem está trabalhando</a> no caso?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Espaços de trabalho e partições {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Espaços de trabalho e partições</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">espaços de trabalho e/ou partições</a> você tem?</li>
<li>Qual é o objetivo principal de cada espaço de trabalho e partição?</li>
<li>Faça o seu <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Espaços de trabalho</a> ou <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partições</a> precisa ser auditada/alterada?</li>
<li>Qual é a relação entre seus espaços de trabalho e partições?</li>
<li>Quantos usuários <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">ter acesso</a> para cada espaço de trabalho?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Como os espaços de trabalho e as partições são definidos?</li>
<li>Qual é o seu processo para adicionar espaços de trabalho à sua instância ou adicionar usuários a um espaço de trabalho?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Campanhas inteligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Configurações da campanha inteligente</td> 
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Você tem uma restrição?</a> no tamanho do Smart Campaign?</li>
<li>Caso contrário, considere adicionar um. Recomendamos limitar os limites da campanha inteligente para 25% do banco de dados para evitar comunicação excessiva ou processar todo o banco de dados em workflows. Isso não apenas protege a marca, mas ajuda a proteger o desempenho da instância.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Limites de comunicação {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Limites de comunicação</td> 
   <td><li>Há <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limites de comunicação</a> em vigor? Sua empresa tem políticas em que os limites de comunicação podem ser necessários?</li>
<li>A Adobe recomenda limitar sua comunicação a 1 por dia e 3 por 7 dias, com <b>não</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operacional</a> emails bloqueados.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li>Quantas tags há? Quantas tags estão em uso? É necessário adicionar alguma?</li>
<li>As tags são necessárias em seus programas?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Canais</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">canais</a> existem? Quantas estão em uso?</li>
<li>São todos <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">status do programa do canal apropriado</a>? Eles mostram progressão dentro do programa?</li>
<li>Seus canais estão relacionados a tipos de programas específicos?</li>
<li>Quais status são considerados bem-sucedidos para cada canal? Eles se alinham às suas metas de marketing?</li>
<li>O canal Operacional está sendo usado adequadamente?</li>
<li>Para o Advanced Report Builder (Revenue Cycle Explorer\RCE), o comportamento da análise do seu canal está definido para ser alinhado às práticas do seu programa que incorporam o custo do período?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Calendário de marketing (se aplicável)</td> 
   <td><li>Há quantos tipos de entrada de calendário? Elas ainda são relevantes?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Gerenciamento de bancos de dados {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Gerenciamento de campos</td> 
   <td><li>Há quantos campos? Clique em "Exportar nomes de campo" para revisar uma lista de campos, campos personalizados e seus nomes de API.</li>
<li>Quantos campos personalizados há?</li>
<li>Quantos campos estão sendo usados? Selecione "Exportar usado por" no menu suspenso Ações de campo para revisar ativos relacionados de um campo.</li>
<li>Quantos são sincronizados entre o Marketo Engage e o seu CRM?</li>
<li>Os campos do CRM estão sincronizados com os objetos apropriados?</li>
<li>Há um conjunto de exibições personalizado para detalhes da pessoa? Deveria haver?</li>
<li>Você tem uma convenção de nomenclatura para seus campos com base na origem? Caso contrário, considere implementar isso.</li>
<li>Há campos bloqueados? Certifique-se de entender por que eles estão.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Atividades personalizadas</td> 
   <td><li>Há atividades personalizadas?</li>
<li>Em caso afirmativo, clique nessas atividades para entender quais atividades não estão relacionadas a um formulário, email ou página de aterrissagem do Marketo.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>objetos  personalizados</td> 
   <td><li>Quantos objetos personalizados há? Como eles são sincronizados ao seu CRM?</li>
<li>Como esses objetos personalizados estão sendo utilizados pelos seus programas e consultas de lista?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Integrações {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>A qual CRM você está sincronizando? Salesforce? MS Dynamics? Veeva?</li>
<li>A sincronização personalizada ou bidirecional? (KG: CORRIGIR GRAMÁTICA E VERIFICAR IMPORTÂNCIA)</li>
<li>[Somente Salesforce] Sua instância tem Filtros de sincronização personalizados implementados? Entre em contato com o Suporte da Marketo para identificar Filtros de sincronização personalizados ou solicitar que uma regra de sincronização personalizada seja implementada.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Páginas</td> 
   <td><li>Como o domínio é definido?</li>
<li>Como o fallback foi definido?</li>
<li>Como é definida a página inicial?</li>
<li>O preenchimento prévio do formulário está ativado?</li>
<li>Os URLs personalizados estão habilitados?</li>
<li>Há regras configuradas para redirecionamentos?</li>
<li>Você tem aliases de domínio em vigor? Você está rastreando por meio da documentação como está utilizando seus aliases de domínio?</li>
<li>Os domínios seguros para páginas de aterrissagem estão ativados? Confirme se os ativos da página de aterrissagem contêm um URL "http".</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>O seu código de rastreamento do Munchkin está no seu site (não no Marketo)?</li>
<li>Uma solicitação de navegador "Não rastrear" está ativada?</li>
<li>Sua API do Munchkin está configurada? Se você não tiver uma documentação sobre onde está o código do Munchkin no seu site, comece com uma visualização rápida usando o "Relatório do Web Analytics" no "Analytics" básico para entender onde o código do Munchkin é colocado em seu site.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Serviços da Web</td> 
   <td><li>As Restrições de IP estão habilitadas? Deveriam ser?</li>
<li>Quais usuários/aplicativos estão fazendo chamadas de API em sua instância?</li>
<li>Você está atingindo ou perto de atingir o limite da API? Nesse caso, considere aumentá-lo ou auditar sua instância para desativar essas chamadas de API.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (se aplicável)</td> 
   <td><li>Tem o <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Pacote MSI instalado</a>?</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">atualizado para a versão mais recente do Sales Insight</a>?</li>
<li>Você concluiu a configuração do Sales Insight? Usuários Enterprise/Unlimited <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">clique aqui</a>, Usuários profissionais <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">clique aqui</a>.</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">acesso concedido aos usuários</a> com base no número de vagas que você comprou?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Ponto de lançamento (se aplicável)</td> 
   <td><li>Quais serviços você configurou (webinário, publicidade etc.)? Algum está próximo da expiração?</li>
<li>Quantas chamadas de API suas integrações estão usando?</li>
<li>Você tem as integrações certas em vigor para seus casos de uso?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Webhooks (se aplicável)</td> 
   <td><li>Que conexões você configurou?</li>
<li>Não estão mais em uso?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Aplicativos móveis (se aplicável)</td> 
   <td><li>Quais aplicativos móveis você tem?</li>
<li>Quais dispositivos de teste foram adicionados?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Baú do tesouro {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Baú do tesouro</td> 
   <td><li>O que está ligado no Baú do Tesouro?</li>
<li>Há recursos que devem ser ativados ou desativados?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Inspetor de campanhas</td> 
   <td><li>O Inspetor de Campanha está ativado?</li>
<li>Caso contrário, considere ativá-la para identificar facilmente quais campanhas estão ativas, sincronizando com seu CRM e/ou excluindo registros.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Diversos {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Atualizações de status do Marketo Engage</td> 
   <td><li>Sua instância está inscrita para atualizações de status do Marketo Engage?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Contatos autorizados</td> 
   <td><li>Você configurou os contatos autorizados apropriados no Portal de suporte?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Alertas</td> 
   <td><li>Algum alerta ativo está sendo enviado para equipes internas do Marketo Engage?</li>
<li>Em caso afirmativo, esses alertas estão funcionando adequadamente?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Notificações</td> 
   <td><li>Você está inscrito nas notificações administrativas apropriadas?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
