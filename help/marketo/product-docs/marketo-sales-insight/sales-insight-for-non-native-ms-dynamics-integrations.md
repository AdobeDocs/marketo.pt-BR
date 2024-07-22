---
description: Sales Insight for Non-Native MS Dynamics Integrations - Marketo Docs - Documentação do produto
title: Sales Insight para integrações não-nativas do MS Dynamics
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 0%

---

# Sales Insight para integrações não-nativas do MS Dynamics {#sales-insight-for-non-native-ms-dynamics-integrations}

Se sua conta do Adobe Marketo Engage estiver conectada ao MS Dynamics por meio de uma integração personalizada ou não nativa, use este artigo para configurar o Sales Insight.

>[!PREREQUISITES]
>
>* O recurso &quot;MSI não nativo&quot; é ativado para a instância do Marketo antes de você iniciar a configuração do MSI. Se não estiver e você já tiver comprado o recurso, contate o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se você ainda não adquiriu esse recurso, entre em contato com a equipe da conta do Adobe (seu gerente de conta).
>* Baixe o [Pacote MSI para Sincronização Personalizada](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* Uma assinatura do MS Dynamics com Instalação MSI (só há suporte para o [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} no momento).
>* API REST do Marketo [configurada com êxito](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. As APIs CRUD expostas serão a base para executar a sincronização não nativa.
>* Leia [esta postagem do blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para entender o objeto e as relações.

## A sincronização não nativa bem-sucedida para o MSI requer o seguinte {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizar o Usuário de Vendas do MS Dynamics com o Marketo.

   O Usuário de Vendas do MS Dynamics é um usuário externo que possui os Clientes Potenciais/Contatos no MS Dynamics. Um Vendedor do Marketo precisa ser substituído pelo Usuário de Vendas do MS Dynamics. O campo externalSalesPersonId é obrigatório para a substituição do Vendedor.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo do Vendedor do Marketo</strong></td> 
      <td><strong>Campo de usuário do MS Dynamics</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas do usuário do MS Dynamics</td> 
      <td><p>Identifica o registro do Vendedor do Marketo para um objeto externo de Usuário do MS Dynamics.</p><p>É obrigatório que o Vendedor seja sincronizado primeiro antes de sincronizar os outros objetos para que os relacionamentos adequados sejam criados.</p></td> 
     </tr> 
    </tbody> 
   </table>

   * [Documentação de API para Vendedor](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [Documentação de API para sincronizar o Vendedor](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizar as Contas do MS Dynamics com o Marketo.

   Uma Empresa do Marketo precisará ser substituída pela Conta do MS Dynamics. Os campos _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para a substituição da Empresa.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de empresa do Marketo</strong></td> 
      <td><strong>Campo de conta do MS Dynamics</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas da conta do MS Dynamics</td> 
      <td>Identifica um registro da Marketo Company para um objeto externo de conta do MS Dynamics.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas do usuário do MS Dynamics Sales</td> 
      <td>Identifica um registro da Marketo Company para um objeto externo de usuário do MS Dynamics Sales que é o proprietário da conta.<br><br>Também usado no Marketo para associar a Empresa ao Vendedor que possui o registro da Empresa. É obrigatório sincronizar o Vendedor primeiro antes de definir esse campo.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação de API para Empresas: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentação da API para sincronização de Empresas: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizar Clientes Potenciais/Contatos do MS Dynamics com a Marketo.

   Você precisará substituir um cliente em potencial da Marketo pelo contato/cliente em potencial do MS Dynamics. Os campos _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ são obrigatórios para a substituição do lead.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de clientes em potencial do Marketo</strong></td> 
      <td><strong>Campo de Cliente Potencial/Contato do MS Dynamics</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalPersonId</td> 
      <td>Identificador global exclusivo que não diferencia maiúsculas de minúsculas do Cliente Potencial/Contato do MS Dynamics</td> 
      <td>Identifica o registro de cliente potencial da Marketo para um objeto de contato/cliente potencial externo do MS Dynamics.<br><br>Este é um novo campo introduzido para Não Nativo MSI.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas do usuário do MS Dynamics Sales</td> 
      <td>Identifica o objeto externo Usuário de Vendas do MS Dynamics que é proprietário deste Cliente Potencial/Contato.<br><br>Também relaciona o cliente potencial com o Vendedor na Marketo. É obrigatório sincronizar corretamente o Vendedor primeiro.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas da conta do MS Dynamics</td> 
      <td>Identifica o objeto de Conta externa do MS Dynamics ao qual o Cliente Potencial/Contato pertence.<br><br>Também relaciona o registro de cliente potencial a uma Empresa no Marketo. É obrigatório que a Conta do MS Dynamics seja sincronizada corretamente primeiro.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação de API para clientes em potencial: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * Documentação da API para clientes em potencial de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. Sincronizar Oportunidades do MS Dynamics com o Marketo.

   Será necessário substituir uma Oportunidade do Marketo pela Oportunidade do MS Dynamics. Os campos _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para a substituição da Oportunidade.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de objeto de oportunidade do Marketo</strong></td> 
      <td><strong>Campo de objeto de oportunidade do MS Dynamics</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificador global exclusivo que não diferencia maiúsculas de minúsculas do Cliente Potencial/Contato do MS Dynamics</td> 
      <td>Identifica o registro de Oportunidade da Marketo para um objeto de Oportunidade externo do MS Dynamics.</td> 
     </tr> 
     <tr> 
      <td>externalCompanyId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas da conta do MS Dynamics</td> 
      <td>Identifica o objeto externo da Conta do MS Dynamics ao qual essa Oportunidade pertence. <br><br>É obrigatório que a Conta do MS Dynamics seja sincronizada corretamente primeiro.</td> 
     </tr> 
     <tr> 
      <td>externalSalesPersonId</td> 
      <td>Identificador exclusivo global que não diferencia maiúsculas de minúsculas do usuário do MS Dynamics Sales</td> 
      <td>Identifica o objeto externo Usuário de Vendas do MS Dynamics que é proprietário desta Oportunidade. </td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação de API da oportunidade: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentação da API para oportunidades de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar Funções de Contato do MS Dynamics com o Marketo.

   As funções de contato do MS Dynamics para uma oportunidade do MS Dynamics podem ser sincronizadas por meio da função Oportunidade do Marketo. O registro da Função de Oportunidade exige os campos _externalOpportunityId_, _role_ e _leadId_.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de função da oportunidade Marketo</strong></td> 
      <td><strong>Campo de Função do Contato do MS Dynamics</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>externalOpportunityId</td> 
      <td>Identificador global exclusivo que não diferencia maiúsculas de minúsculas no MS Dynamics Opportunity</td> 
      <td>Identifica a função de oportunidade da Marketo para um objeto de oportunidade externo do MS Dynamics.<br><br>É obrigatório que a Oportunidade do MS Dynamics seja sincronizada corretamente primeiro.</td> 
     </tr> 
     <tr> 
      <td>leadId</td> 
      <td>N/D, essa seria uma ID de cliente potencial da Marketo</td> 
      <td>Essa seria a ID do cliente potencial da Marketo do Contato sincronizado do MS Dynamics.<br><br>Depois que o contato for sincronizado no Marketo, você poderá usar o identificador exclusivo global, que não diferencia maiúsculas de minúsculas, do Contato do MS Dynamics como externalPersonId e consultar o cliente potencial do Marketo usando a API REST do Marketo.</td> 
     </tr> 
     <tr> 
      <td>função</td> 
      <td>O campo Função do Contato do MS Dynamics</td> 
      <td>Descreve a função do contato para esta oportunidade.</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação de API da oportunidade: [https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentação da API para oportunidades de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar campos de Última Pontuação de Momento Interessante/MSI com o MS Dynamics.

   Depois que os objetos do MS Dynamics forem sincronizados corretamente com o Marketo, você poderá aproveitar os recursos do MSI. Os campos Último momento interessante/Pontuação do MSI serão expostos na API REST para leads. Esses campos são calculados pelo MSI e são somente leitura.

   Os campos Último momento interessante/Pontuação de um lead da Marketo precisarão ser sincronizados regularmente com o MS Dynamics usando o endpoint do lead da API REST. Consulte este ponto de extremidade para um cliente potencial do Marketo usando a _externalPersonId_ como o filterType e transmitindo a GUID do cliente potencial do MS Dynamics como o filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Em seguida, você pode usar os valores desses campos para sincronizar com o objeto de Cliente Potencial/Contato do MS Dynamics.

   <table> 
    <colgroup> 
     <col> 
     <col> 
     <col> 
    </colgroup> 
    <tbody> 
     <tr> 
      <td><strong>Campo de clientes em potencial do Marketo</strong></td> 
      <td><strong>Campo de Cliente Potencial/Contato do MS Dynamics</strong></td> 
      <td><strong>Descrição</strong></td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentType</td> 
      <td>Rótulo: Tipo do Último Momento Interessante<br>Nome: Last_Interested_Moment_Type__c</td> 
      <td>Tipo do último momento interessante para o lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDate</td> 
      <td><p>Rótulo: Última data de momento interessante</p><p>Nome: Last_Interested_Moment_Date__c</p></td> 
      <td>Data do último momento interessante do cliente potencial</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentDesc</td> 
      <td><p>Rótulo: Descrição do último momento interessante</p><p>Nome: Last_Interested_Moment_Desc__c</p></td> 
      <td>Descrição do último momento interessante do lead</td> 
     </tr> 
     <tr> 
      <td>msiLastInterestedMomentSource</td> 
      <td><p>Rótulo: Source do último momento interessante</p><p>Nome: Last_Interested_Moment_Source__c</p></td> 
      <td>Source do último momento interessante para o lead</td> 
     </tr> 
     <tr> 
      <td>prioridade</td> 
      <td><p>Rótulo: Engajamento</p><p>Nome: Priority_c</p></td> 
      <td>Prioridade do cliente em potencial</td> 
     </tr> 
     <tr> 
      <td>relativeUrgency</td> 
      <td><p>Rótulo: valor relativo de urgência</p><p>Nome: Urgency_Value__c</p></td> 
      <td>Urgência relativa do lead</td> 
     </tr> 
     <tr> 
      <td>relativeScoring</td> 
      <td><p>Rótulo: valor de pontuação relativo</p><p>Nome: Relative_Score_Value__c</p></td> 
      <td>Pontuação relativa do lead</td> 
     </tr> 
    </tbody> 
   </table>

   * Documentação da API REST de cliente potencial: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   O uso adequado dos campos externos é a chave para uma sincronização bem-sucedida não nativa. Se não conseguir ver os dados em algumas exibições, é provável que um determinado campo não tenha sido sincronizado corretamente. Por exemplo, se as atividades e os momentos interessantes de um lead não forem exibidos ao pesquisar o widget MSI em sua Conta, é provável que a empresa do lead ou a Conta não tenha sido sincronizada corretamente. Executar uma solicitação GET para este cliente potencial ao especificar os campos externos ajudará a verificar se o cliente potencial foi sincronizado corretamente. Além disso, o email do vendedor externo no Marketo deve corresponder ao email desse usuário no MS Dynamics. Os dados podem não ser exibidos na guia Marketo no MS Dynamics se os emails não corresponderem.
