---
unique-page-id: 45417125
description: Insight de vendas para integrações não nativas do Salesforce - Documentos da Marketo - Documentação do produto
title: Insight de vendas para integrações não nativas do Salesforce
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
source-git-commit: fb663ddf4c0021f258317636fbc7794e8172ab7e
workflow-type: tm+mt
source-wordcount: '1400'
ht-degree: 0%

---

# Insight de vendas para integrações não nativas do Salesforce {#sales-insight-for-non-native-salesforce-integrations}

Se sua conta do Adobe Marketo Engage estiver conectada ao Salesforce por meio de uma integração personalizada ou não nativa, use este artigo para configurar o Sales Insight.

>[!PREREQUISITES]
>
>* O recurso &quot;MSI não nativo&quot; ativado para sua instância do Marketo antes de iniciar a configuração do MSI (se ele não for e você já tiver comprado o recurso), entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} - se ainda não tiver comprado esse recurso, entre em contato com o Gerente de sucesso do cliente).
>* Uma conta do Salesforce com [Configuração do pacote MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target=&quot;_blank&quot;}.
>* API REST do Marketo [configuração com êxito](https://developers.marketo.com/rest-api/){target=&quot;_blank&quot;}. As APIs CRUD expostas serão a base para executar a sincronização não nativa.
>* Ler [esta postagem de blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target=&quot;_blank&quot;} para obter uma compreensão do objeto e dos relacionamentos.
>* Configure objetos Salesforce para exibir o identificador global exclusivo com 18 caracteres, que não diferencia maiúsculas de minúsculas, em vez do identificador global exclusivo com 15 caracteres.


>[!NOTE]
>
>A configuração da API REST no painel de administração MSI do Marketo não pode ser usada para a sincronização não nativa.

## A sincronização não nativa bem-sucedida para MSI requer o seguinte {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizar o usuário de vendas do Salesforce com o Marketo.

   O Usuário de Vendas do Salesforce é um usuário externo proprietário dos Clientes Potenciais/Contatos no Salesforce. Uma Pessoa de Vendas da Marketo precisa ser atualizada para o Usuário de Vendas do Salesforce. O *externalSalesPersonId* é obrigatório para o supervisor da Pessoa de Vendas.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de pessoa de vendas do Marketo</strong></td> 
      <td><strong>Campo do Usuário do Salesforce Sales</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador globalmente exclusivo do usuário do Salesforce Sales</td> 
      <td><p>Identifica o registro da Pessoa de Vendas do Marketo para um objeto de Usuário de Vendas do Salesforce externo.</p><p>É obrigatório que a Pessoa de Vendas seja sincronizada primeiro antes de sincronizar os outros objetos, para que os relacionamentos adequados sejam criados.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação da API da pessoa de vendas: [https://developers.marketo.com/rest-api/lead-database/sales-persons/](https://developers.marketo.com/rest-api/lead-database/sales-persons/){target=&quot;_blank&quot;}
   * Documentação da API para sincronização da pessoa de vendas: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Pessoas/syncSalesPeopleUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Sales_Pessoas/syncSalesPeopleUsingPOST){target=&quot;_blank&quot;}

1. Sincronizar as contas do Salesforce com o Marketo.

   Uma empresa do Marketo precisará ser atualizada para a conta do Salesforce. O _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para o supervisor da Empresa.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo da empresa Marketo</strong></td> 
      <td><strong>Campo de conta do Salesforce</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador globalmente exclusivo da conta do Salesforce</td> 
      <td>Identifica um registro de Empresa do Marketo para um objeto de Conta do Salesforce externo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador globalmente exclusivo do usuário do Salesforce Sales</td> 
      <td>Identifica um registro da Empresa do Marketo para um objeto de Usuário de Vendas do Salesforce externo que é o proprietário da Conta.<br><br>Também usado no Marketo para associar a Empresa à Pessoa de Vendas proprietária do registro da Empresa. É obrigatório ter a Pessoa de vendas sincronizada primeiro antes de definir esse campo.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação da API para empresas: [https://developers.marketo.com/rest-api/lead-database/companies/](https://developers.marketo.com/rest-api/lead-database/companies/){target=&quot;_blank&quot;}
   * Documentação da API para sincronização de empresas: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Empresas/syncEmpresasUsandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Empresas/syncEmpresasUsandoPOST){target=&quot;_blank&quot;}

1. Sincronize os leads/contatos do Salesforce com o Marketo.

   Você precisará atualizar um líder da Marketo para o lead/contato do Salesforce. O _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ são obrigatórios para o supervisor do lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de lead do Marketo</strong></td> 
      <td><strong>Campo de lead/contato do Salesforce</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identificador global sem distinção entre maiúsculas e minúsculas do Salesforce</td> 
      <td>Identifica o registro de lead do Marketo para um objeto de lead/contato externo do Salesforce.<br><br>Este é um novo campo introduzido para MSI não nativo.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador globalmente exclusivo do usuário do Salesforce Sales</td> 
      <td>Identifica o objeto de Usuário de Vendas do Salesforce externo proprietário deste Lead/Contato.<br><br>Também relaciona o lead com a pessoa de vendas no Marketo. É obrigatório ter a Pessoa de Vendas sincronizada corretamente primeiro.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador globalmente exclusivo da conta do Salesforce</td> 
      <td>Identifica o objeto externo de Conta do Salesforce ao qual o Cliente Potencial/Contato pertence.<br><br>Também relaciona o registro de lead a uma Empresa no Marketo. É obrigatório que a conta do Salesforce seja sincronizada corretamente primeiro.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação de API para clientes potenciais: [https://developers.marketo.com/rest-api/lead-database/leads/](https://developers.marketo.com/rest-api/lead-database/leads/)
   * Documentação da API para sincronização de leads: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/syncLeadUsingPOST)

1. Sincronizar oportunidades do Salesforce com o Marketo.

   Você precisará atualizar uma oportunidade da Marketo para a oportunidade do Salesforce. O _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ Os campos são obrigatórios para o cabeçalho da Oportunidade.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo Objeto de Oportunidade do Marketo</strong></td> 
      <td><strong>Campo de Objeto de Oportunidade do Salesforce</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificador global sem distinção entre maiúsculas e minúsculas do Salesforce</td> 
      <td>Identifica o registro de Oportunidade da Marketo para um objeto de Oportunidade do Salesforce externo.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador globalmente exclusivo da conta do Salesforce</td> 
      <td>Identifica o objeto externo da Conta do Salesforce ao qual esta Oportunidade pertence. <br><br>É obrigatório que a conta do Salesforce seja sincronizada corretamente primeiro.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador globalmente exclusivo do usuário do Salesforce Sales</td> 
      <td>Identifica o objeto de Usuário de Vendas do Salesforce externo proprietário desta Oportunidade. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação da API para Oportunidade: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * Documentação da API para sincronização de Oportunidades: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/SyncOportunidadesUsandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/SyncOportunidadesUsandoPOST){target=&quot;_blank&quot;}

1. Sincronizar funções de contato do Salesforce com o Marketo.

   As Funções de Contato do Salesforce para uma Oportunidade do Salesforce podem ser sincronizadas por meio da Função de Oportunidade da Marketo. O registro de Função da Oportunidade atribui a função _externalOpportunityId_, _função_ e _leadId_ campos.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de Função da Oportunidade do Marketo</strong></td> 
      <td><strong>Campo de Função de Contato do Salesforce</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificador global sem distinção entre maiúsculas e minúsculas do Salesforce Oportunity</td> 
      <td>Identifica a Função de Oportunidade da Marketo para um objeto de Oportunidade do Salesforce externo.<br><br>É obrigatório que a Oportunidade do Salesforce seja sincronizada corretamente primeiro.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, isso seria uma ID de cliente potencial do Marketo</td> 
      <td>Essa seria a ID de lead da Marketo do contato sincrônico do Salesforce.<br><br>Depois que o contato é sincronizado no Marketo, você pode usar o identificador global de maiúsculas e minúsculas do Salesforce Contact como externalPersonId e consultar o Marketo Lead usando a API REST do Marketo.</td> 
     </tr> 
     <tr> 
      <td>função</td> 
      <td>O campo Função para o contato do Salesforce</td> 
      <td>Descreve a função do contato para esta oportunidade.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação da API para Oportunidade: [https://developers.marketo.com/rest-api/lead-database/opportunities/](https://developers.marketo.com/rest-api/lead-database/opportunities/){target=&quot;_blank&quot;}
   * Documentação da API para sincronização de Oportunidades: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/SyncOportunidadesUsandoPOST](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Oportunidades/SyncOportunidadesUsandoPOST){target=&quot;_blank&quot;}

1. Sincronize os campos Último momento Interessante/Pontuação MSI para SFDC.

   Depois que os objetos do Salesforce forem sincronizados corretamente com o Marketo, você poderá aproveitar os recursos do MSI. Os campos Último momento interessante/Pontuação do MSI serão expostos na REST API para Leads. Esses campos são calculados pelo MSI e são somente leitura.

   Os campos Último momento interessante/Pontuação de um cliente potencial do Marketo precisarão ser sincronizados regularmente com o Salesforce usando o endpoint de cliente potencial da API REST. Consulte este terminal para obter um lead para Marketo usando o _externalPersonId_ como o filterType e transmitindo o GUID de lead do Salesforce como o filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Em seguida, você pode usar os valores desses campos para sincronizar com seu objeto de lead/contato do Salesforce.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de lead do Marketo</strong></td> 
      <td><strong>Campo de lead/contato do Salesforce</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentType</td> 
      <td>Rótulo: Tipo de Último Momento Interessante<br>Nome: Last_Interesting_Moment_Type_c</td> 
      <td>Tipo do último momento interessante para o Líder</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDate</td> 
      <td><p>Rótulo: Data do Último Momento Interessante</p><p>Nome: Last_Interesting_Moment_Date_c</p></td> 
      <td>Data do último momento interessante para o Líder</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentDesc</td> 
      <td><p>Rótulo: Descrição do Último Momento Interessante</p><p>Nome: Last_Interesting_Moment_Desc__c</p></td> 
      <td>Descrição do último momento interessante para o cliente potencial</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestingMomentSource</td> 
      <td><p>Rótulo: Fonte do Último Momento Interessante</p><p>Nome: Last_Interesting_Moment_Source_c</p></td> 
      <td>Fonte do último momento interessante para o Líder</td> 
     </tr> 
     <tr> 
      <td>prioridade</td> 
      <td><p>Rótulo: Envolvimento</p><p>Nome: Prioridade__c</p></td> 
      <td>Prioridade do cliente potencial</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Rótulo: Valor de Urgência Relativo</p><p>Nome: Urgency_Value_c</p></td> 
      <td>Urgência relativa do cliente potencial</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Rótulo: Valor da pontuação relativo</p><p>Nome: Relative_Score_Value_c</p></td> 
      <td>Pontuação relativa do cliente potencial</td> 
     </tr> 
    </tbody> 
   </table>

   Documentação da API REST de cliente potencial: [https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Leads/getLeadByIdUsingGET){target=&quot;_blank&quot;}.

   O uso adequado dos campos externos é fundamental para uma sincronização não nativa bem-sucedida. Se você não conseguir ver os dados em algumas exibições, é provável que um determinado campo não tenha sido sincronizado corretamente. Por exemplo, se as atividades de um cliente potencial e os momentos interessantes não forem exibidos ao procurar no widget MSI em sua conta, é provável que a empresa do cliente potencial ou a conta não tenham sido sincronizadas corretamente. Executar uma solicitação GET para esse lead ao especificar os campos externos ajudará a verificar se o lead foi sincronizado corretamente. Além disso, o email da pessoa de vendas externa no Marketo deve corresponder ao email desse usuário no Salesforce. Os dados podem não ser exibidos na guia Marketo no Salesforce se os emails não corresponderem.
