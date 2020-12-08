---
unique-page-id: 45417125
description: Insight de vendas para integrações Salesforce não nativas - Documentos do Marketing - Documentação do produto
title: Insight de vendas para integrações não nativas do Salesforce
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 0%

---


# Insight de vendas para integrações não nativas do Salesforce {#sales-insight-for-non-native-salesforce-integrations}

Se sua conta do Marketing for conectada ao Salesforce por meio de uma integração personalizada ou não nativa, use esse documento para configurar o Sales Insight.

>[!NOTE]
>
>**Pré-requisitos**
>
>* Entre em contato com o Gerente de sucesso do cliente para ativar o recurso &quot;MSI não nativo&quot; para a sua instância de Marketo.
>* Uma conta do Salesforce com a configuração do Pacote MSI.
>* API REST do Marketo configurada [com êxito](http://developers.marketo.com/rest-api/). As APIs CRUD expostas serão a base para executar a sincronização não nativa.
>* Leia [essa postagem](http://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/) no blog para entender o objeto e os relacionamentos.
>* Configure objetos do Salesforce para exibir o identificador global exclusivo com 18 caracteres que não diferencia maiúsculas e minúsculas em vez do identificador global exclusivo com 15 caracteres.

>



>[!NOTE]
>
>A Configuração da API REST no Painel de administração MSI do Marketing não pode ser usada para a sincronização Não Nativa.

## Sincronização não nativa bem-sucedida para MSI requer o seguinte {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronize o usuário de vendas do Salesforce com o Marketing.

   O Usuário de Vendas do Salesforce é um usuário externo proprietário dos Contatos/Clientes Potenciais no Salesforce. Uma Pessoa de Vendas do Marketing Cloud precisa ser atualizada para o Usuário de Vendas do Salesforce. O campo *externalSalesPersonId* é obrigatório para a atualização da Pessoa de Vendas.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de Pessoa de Vendas do Marketo</strong></td> 
   <td><strong>Campo de Usuário do Salesforce Sales</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificador global exclusivo do Usuário do Salesforce Sales</td> 
   <td><p>Identifica o registro da Pessoa de Vendas do Marketing para um objeto de Usuário de Vendas do Salesforce externo.</p><p>É obrigatório que a Pessoa de Vendas seja sincronizada primeiro antes de sincronizar os outros objetos para que os relacionamentos apropriados sejam criados.</p></td> 
  </tr> 
 </tbody> 
</table>

Documentação da API para a pessoa de vendas: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](http://developers.marketo.com/rest-api/lead-database/sales-persons/)\
Documentação da API para sincronizar a Pessoa de vendas: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_People/syncSalesPeopleUsingPOST)

1. Sincronize as contas do Salesforce com o Marketing.

   Será necessário atualizar uma Empresa de marketing para a conta do Salesforce. Os campos *externalCompanyId* e *externalSalesPersonId* são obrigatórios para a atualização da Empresa.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de Empresa de marketing</strong></td> 
   <td><strong>Campo Conta do Salesforce</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificador global exclusivo da conta Salesforce</td> 
   <td>Identifica um registro de Empresa de marketing para um objeto externo da conta do Salesforce.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificador global exclusivo do Usuário do Salesforce Sales</td> 
   <td>Identifica um registro de Empresa de marketing para um objeto de Usuário de Vendas do Salesforce externo que é o proprietário da Conta.<br><br>Também usado no Marketo para associar a Empresa à Pessoa de vendas que possui o registro da Empresa. É obrigatório que a Pessoa de Vendas seja sincronizada primeiro antes de definir esse campo.</td> 
  </tr> 
 </tbody> 
</table>

Documentação da API para Empresa: [https://developers.marketo.com/rest-api/lead-database/companies/](http://developers.marketo.com/rest-api/lead-database/companies/)\
`API documentation for syncing Companies:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Companies/syncCompaniesUsingPOST)`

1. Sincronize os clientes potenciais/contatos do Salesforce com o Marketing.

   Será necessário atualizar um líder de marketing para o líder/contato do Salesforce. Os campos *externalPersonId*, *externalSalesPersonId* e *externalCompanyId* são obrigatórios para a atualização do Lead.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de cliente potencial do Marketing</strong></td> 
   <td><strong>Campo de cliente potencial/contato do Salesforce</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>externalPersonId</td> 
   <td>Identificador global exclusivo do cliente potencial/contato do Salesforce</td> 
   <td>Identifica o registro de cliente potencial de marketing para um objeto principal/contato externo do Salesforce.<br><br>Este é um novo campo introduzido para MSI Não Nativo.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificador global exclusivo do Usuário do Salesforce Sales</td> 
   <td>Identifica o objeto de Usuário de Vendas do Salesforce externo que é proprietário deste Lead/Contato.<br><br>Relaciona também o cliente em potencial com a pessoa de vendas no mercado. É obrigatório que a Pessoa de Vendas seja sincronizada corretamente primeiro.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificador global exclusivo da conta Salesforce</td> 
   <td>Identifica o objeto externo da conta do Salesforce ao qual o cliente potencial/contato pertence.<br><br>Relaciona também o registro de cliente potencial a uma Empresa em Marketo. É obrigatório que a Conta Salesforce seja sincronizada corretamente primeiro.</td> 
  </tr> 
 </tbody> 
</table>

Documentação da API para clientes potenciais: [`https://developers.marketo.com/rest-api/lead-database/leads/`](http://developers.marketo.com/rest-api/lead-database/leads/)\
Documentação da API para sincronização de clientes potenciais:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronizar oportunidades do Salesforce com o Marketing.

   Será necessário atualizar uma oportunidade de marketing para a oportunidade do Salesforce. Os campos *externalOpportunityId*, *externalCompanyId* e *externalSalesPersonId* são obrigatórios para a atualização da Oportunidade.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de objeto de oportunidade de marketing</strong></td> 
   <td><strong>Campo de Objeto de Oportunidade do Salesforce</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificador global exclusivo do cliente potencial/contato do Salesforce</td> 
   <td>Identifica o registro de Oportunidade de Marketing para um objeto de Oportunidade de Salesforce externo.</td> 
  </tr> 
  <tr> 
   <td>externalCompanyId</td> 
   <td>Identificador global exclusivo da conta Salesforce</td> 
   <td>Identifica o objeto externo da Conta Salesforce ao qual esta Oportunidade pertence. <br><br>É obrigatório que a Conta Salesforce seja sincronizada corretamente primeiro.</td> 
  </tr> 
  <tr> 
   <td>externalSalesPersonId</td> 
   <td>Identificador global exclusivo do Usuário do Salesforce Sales</td> 
   <td>Identifica o objeto de Usuário de Vendas do Salesforce externo proprietário desta Oportunidade. </td> 
  </tr> 
 </tbody> 
</table>

Documentação da API para Oportunidade: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizar funções de contato do Salesforce com o Marketo.

   As Funções de Contato do Salesforce para uma Oportunidade do Salesforce podem ser sincronizadas por meio da Função de Oportunidade de Marketing. O registro de Função de Oportunidade determina os campos *externalOpportunityId*, *função* e *leadId* .

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo Função de Oportunidade de Marketing</strong></td> 
   <td><strong>Campo de Função de Contato do Salesforce</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>externalOpportunityId</td> 
   <td>Identificador global exclusivo para maiúsculas e minúsculas do Salesforce Opportunity</td> 
   <td>Identifica a função de oportunidade de marketing para um objeto de oportunidade externo do Salesforce.<br><br>É obrigatório que a Oportunidade Salesforce seja sincronizada corretamente primeiro.</td> 
  </tr> 
  <tr> 
   <td>leadId</td> 
   <td>N/A, esta seria uma ID de cliente potencial</td> 
   <td>Essa seria a ID líder de mercado do contato sinalizado Salesforce.<br><br>Depois que o contato é sincronizado no Marketo, você pode usar o identificador global exclusivo de maiúsculas e minúsculas do Salesforce Contact como externalPersonId e query para o líder de marketing usando a API REST do Marketo.</td> 
  </tr> 
  <tr> 
   <td>função</td> 
   <td>O campo Função para o Contato do Salesforce</td> 
   <td>Descreve a função do contato para esta oportunidade.</td> 
  </tr> 
 </tbody> 
</table>

Documentação da API para Oportunidade: [`https://developers.marketo.com/rest-api/lead-database/opportunities/`](http://developers.marketo.com/rest-api/lead-database/opportunities/)\
`API documentation for syncing Opportunities:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Opportunities/syncOpportunitiesUsingPOST)`

1. Sincronizar campos de Pontuação do Último Momento Interessante/MSI para SFDC.

   Depois que os objetos do Salesforce forem sincronizados corretamente com o Marketo, você poderá aproveitar os recursos MSI. Os campos Último momento interessante/Pontuação do MSI serão expostos na REST API para clientes potenciais. Esses campos são calculados pelo MSI e são somente leitura.

   Os campos Último momento interessante/Pontuação de um cliente potencial de marketing precisarão ser sincronizados regularmente com o Salesforce usando o endpoint REST API. Query este terminal para um cliente potencial de marketing usando o *externalPersonId* como filterType e transmitindo o GUID de cliente potencial do Salesforce como filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Em seguida, você pode usar os valores desses campos para sincronizar com o objeto de cliente potencial/contato do Salesforce.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Campo de cliente potencial do Marketing</strong></td> 
   <td><strong>Campo de cliente potencial/contato do Salesforce</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentType</td> 
   <td>Rótulo: Último<br>TypeName de Momento Interessante: Last_Interesting_Moment_Type_c</td> 
   <td>Tipo do último momento interessante para o cliente potencial</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDate</td> 
   <td><p>Rótulo: Data do Último Momento Interessante</p><p>Nome: Last_Interesting_Moment_Date_c</p></td> 
   <td>Data do último momento interessante para o cliente potencial</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentDesc</td> 
   <td><p>Rótulo: Descrição do Último Momento Interessante</p><p>Nome: Last_Interesting_Moment_Desc__c</p></td> 
   <td>Descrição do último momento interessante para o cliente potencial</td> 
  </tr> 
  <tr> 
   <td>msiLastInterestingMomentSource</td> 
   <td><p>Rótulo: Origem do Último Momento Interessante</p><p>Nome: Last_Interesting_Moment_Source_c</p></td> 
   <td>Fonte do último momento interessante para o líder</td> 
  </tr> 
  <tr> 
   <td>prioridade</td> 
   <td><p>Rótulo: Envolvimento</p><p>Nome: Priority_c</p></td> 
   <td>Prioridade do cliente potencial</td> 
  </tr> 
  <tr> 
   <td>relativeUrgency</td> 
   <td><p>Rótulo: Valor de Urgência Relativo</p><p>Nome: Urgency_Value_c</p></td> 
   <td>Urgência relativa do cliente potencial</td> 
  </tr> 
  <tr> 
   <td>relativeScoring</td> 
   <td><p>Rótulo: Valor de Pontuação Relativo</p><p>Nome: Relative_Score_Value_c</p></td> 
   <td>Pontuação relativa do cliente potencial</td> 
  </tr> 
 </tbody> 
</table>

Documentação da API REST de cliente potencial:  [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](http://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET).

O uso correto dos campos externos é a chave para uma sincronização não nativa bem-sucedida. Se você não conseguir ver os dados em algumas visualizações, é provável que um determinado campo não tenha sido sincronizado corretamente. Por exemplo, se atividades de um cliente potencial e momentos interessantes não aparecerem ao procurar no widget MSI sob sua Conta, é provável que a empresa do cliente potencial ou a Conta não tenham sido sincronizadas corretamente. Executar uma solicitação de GET para este cliente potencial ao especificar os campos externos o ajudará a verificar se o cliente potencial foi sincronizado corretamente. Além disso, o email do vendedor externo no Marketo deve corresponder ao email desse usuário no Salesforce. Os dados podem não ser exibidos na guia Marketo no Salesforce se os e-mails não corresponderem.

