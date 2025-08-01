---
unique-page-id: 45417125
description: '[!DNL Sales Insight] para Integrações  [!DNL Salesforce]  Não Nativas - Documentação do Marketo - Documentação do Produto'
title: '[!DNL Sales Insight] para integrações  [!DNL Salesforce]  não nativas'
exl-id: a771ecdf-c610-44e4-9e93-7fdcc9d79f4b
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---

# [!DNL Sales Insight] para integrações [!DNL Salesforce] não nativas {#sales-insight-for-non-native-salesforce-integrations}

Se sua conta do Adobe Marketo Engage estiver conectada ao [!DNL Salesforce] por meio de uma integração personalizada ou não nativa, use este artigo para configurar o [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* O recurso &quot;MSI não nativo&quot; é ativado para a instância do Marketo antes de você iniciar a configuração do MSI. Se não estiver e você já tiver comprado o recurso, contate o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se você ainda não adquiriu esse recurso, entre em contato com a equipe de conta da Adobe (seu gerente de conta).
>* Uma conta do Salesforce com [Pacote MSI configurado](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
>* API REST do Marketo [configurada com êxito](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. As APIs CRUD expostas serão a base para executar a sincronização não nativa.
>* Leia [esta postagem do blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para entender o objeto e as relações.
>* Configure objetos [!DNL Salesforce] para exibir o identificador global exclusivo que não diferencia maiúsculas de minúsculas de 18 caracteres, em vez do identificador global exclusivo que diferencia maiúsculas de minúsculas de 15 caracteres.

>[!NOTE]
>
>A configuração da API REST no Painel de administração do MSI do Marketo não pode ser usada para a sincronização não nativa.

## A sincronização não nativa bem-sucedida para o MSI requer o seguinte {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronizar o Usuário de Vendas [!DNL Salesforce] com o Marketo.

   O Usuário de Vendas [!DNL Salesforce] é um usuário externo que possui os Clientes Potenciais/Contatos em [!DNL Salesforce]. Um Vendedor do Marketo precisa ser substituído pelo Usuário de Vendas [!DNL Salesforce]. O campo *externalSalesPersonId* é obrigatório para a substituição do Vendedor.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo do Vendedor do Marketo</strong></td>
        <td><strong>Campo de usuário de vendas <span class="dnl">Salesforce</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador exclusivo global que não diferencia maiúsculas de minúsculas do Usuário de Vendas</td>
      <td><p>Identifica o registro de Vendedor do Marketo para um objeto de Usuário de Vendas <span class="dnl">Salesforce</span> externo.</p><p>É obrigatório que o Vendedor seja sincronizado primeiro antes de sincronizar os outros objetos para que os relacionamentos adequados sejam criados.</p></td>
     </tr>
    </tbody>
   </table>

   * Documentação de API do Vendedor: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/sales-persons](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * Documentação da API para sincronizar o Vendedor: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizar as Contas do [!DNL Salesforce] com a Marketo.

   Será necessário substituir uma Empresa do Marketo pela Conta [!DNL Salesforce]. Os campos _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para a substituição da Empresa.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de empresa do Marketo</strong></td>
        <td><strong>Campo de Conta do <span class="dnl">Salesforce</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>Identificador exclusivo global, sem distinção entre maiúsculas e minúsculas, da conta do <span class="dnl">Salesforce</span></td>
        <td>Identifica um registro de Empresa da Marketo para um objeto de Conta externa <span class="dnl">Salesforce</span>.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador exclusivo global que não diferencia maiúsculas de minúsculas do Usuário de Vendas</td>
        <td>Identifica um registro da Marketo Company para um objeto de usuário de vendas <span class="dnl">Salesforce</span> externo que é o proprietário da conta.<br><br>Também usado no Marketo para associar a Empresa ao Vendedor que possui o registro da Empresa. É obrigatório sincronizar o Vendedor primeiro antes de definir esse campo.</td>
     </tr>
    </tbody>
   </table>

   * Documentação de API para Empresas: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentação da API para sincronização de Empresas: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Companies/operation/syncCompaniesUsingPOST){target="_blank"}

1. Sincronizar os Clientes Potenciais/Contatos do [!DNL Salesforce] com a Marketo.

   Você precisará substituir um cliente em potencial da Marketo pelo [!DNL Salesforce] cliente em potencial/contato. Os campos _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ são obrigatórios para a substituição do lead.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de clientes em potencial do Marketo</strong></td>
        <td><strong>Campo de clientes em potencial/contatos do <span class="dnl">Salesforce</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalPersonId</td>
        <td>Salesforce <span class="dnl">Identificador exclusivo global de cliente potencial/contato </span>, que não diferencia maiúsculas de minúsculas</td>
        <td>Identifica o registro de cliente potencial da Marketo para um objeto de contato/cliente potencial <span class="dnl">Salesforce</span> externo.<br><br>Este é um novo campo introduzido para Não Nativo MSI.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador exclusivo global que não diferencia maiúsculas de minúsculas do Usuário de Vendas</td>
        <td>Identifica o objeto de Usuário de Vendas <span class="dnl">Salesforce</span> externo que é proprietário deste Cliente Potencial/Contato.<br><br>Também relaciona o cliente potencial com o Vendedor na Marketo. É obrigatório sincronizar corretamente o Vendedor primeiro.</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>Identificador exclusivo global, sem distinção entre maiúsculas e minúsculas, da conta do <span class="dnl">Salesforce</span></td>
        <td>Identifica o objeto de Conta externa <span class="dnl">Salesforce</span> ao qual o Cliente Potencial/Contato pertence.<br><br>Também relaciona o registro de cliente potencial a uma Empresa no Marketo. É obrigatório que a conta do Salesforce seja sincronizada corretamente primeiro.</td>
     </tr>
    </tbody>
   </table>

   * Documentação de API para clientes em potencial: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/leads](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/leads)
   * Documentação da API para clientes em potencial de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST)

1. Sincronizar [!DNL Salesforce] Oportunidades para o Marketo.

   Será necessário substituir uma Oportunidade do Marketo pela Oportunidade [!DNL Salesforce]. Os campos _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para a substituição da Oportunidade.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de objeto de oportunidade do Marketo</strong></td>
        <td><strong>Campo de objeto de oportunidade <span class="dnl">Salesforce</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
      <td>Identificador global exclusivo que não diferencia maiúsculas de minúsculas do Cliente Potencial/Contato da Salesforce</td>
      <td>Identifica o registro de Oportunidade da Marketo para um objeto de Oportunidade da Salesforce externo.</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>Identificador exclusivo global, sem distinção entre maiúsculas e minúsculas, da conta do <span class="dnl">Salesforce</span></td>
        <td>Identifica o objeto de Conta externa <span class="dnl">Salesforce</span> ao qual esta Oportunidade pertence. <br><br>É obrigatório que a Conta <span class="dnl">Salesforce</span> seja sincronizada corretamente primeiro.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td><span class="dnl">Salesforce</span> Identificador exclusivo global que não diferencia maiúsculas de minúsculas do Usuário de Vendas</td>
        <td>Identifica o objeto de Usuário de Vendas <span class="dnl">Salesforce</span> externo que é proprietário desta Oportunidade. </td>
     </tr>
    </tbody>
   </table>

   * Documentação de API da oportunidade: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentação da API para oportunidades de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar Funções de Contato do [!DNL Salesforce] com a Marketo.

   As Funções de Contato do [!DNL Salesforce] para uma Oportunidade do [!DNL Salesforce] podem ser sincronizadas por meio da Função da Oportunidade do Marketo. O registro da Função de Oportunidade exige os campos _externalOpportunityId_, _role_ e _leadId_.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de função da oportunidade Marketo</strong></td>
      <td><strong>Campo de função do contato do Salesforce</strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
        <td><span class="dnl">Salesforce</span> Identificador exclusivo global, que não diferencia maiúsculas de minúsculas, da oportunidade</td>
        <td>Identifica a Função de Oportunidade da Marketo para um objeto de oportunidade <span class="dnl">Salesforce</span> externo.<br><br>É obrigatório que a Oportunidade <span class="dnl">Salesforce</span> seja sincronizada corretamente primeiro.</td>
     </tr>
     <tr>
      <td>leadId</td>
      <td>N/D, essa seria uma ID de cliente potencial da Marketo</td>
        <td>Esta seria a ID de cliente em potencial da Marketo do contato sincronizado do <span class="dnl">Salesforce</span>.<br><br>Depois que o contato for sincronizado no Marketo, você poderá usar o identificador exclusivo global, que não diferencia maiúsculas de minúsculas, do Contato do <span class="dnl">Salesforce</span> como externalPersonId e consultar o Marketo Lead usando a API REST do Marketo.</td>
     </tr>
     <tr>
      <td>função</td>
        <td>O campo Função do Contato <span class="dnl">Salesforce</span></td>
      <td>Descreve a função do contato para esta oportunidade.</td>
     </tr>
    </tbody>
   </table>

   * Documentação de API da oportunidade: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentação da API para oportunidades de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar campos de Última Pontuação de Momento Interessante/MSI com o SFDC.

   Depois que os objetos do [!DNL Salesforce] forem sincronizados corretamente com o Marketo, você poderá aproveitar os recursos MSI. Os campos Último momento interessante/Pontuação do MSI serão expostos na API REST para leads. Esses campos são calculados pelo MSI e são somente leitura.

   Os campos Último momento interessante/Pontuação de um cliente potencial da Marketo precisarão ser sincronizados regularmente com [!DNL Salesforce] usando o ponto de extremidade REST API Lead. Consulte este ponto de extremidade para um cliente potencial da Marketo usando a _externalPersonId_ como o filterType e transmitindo a GUID do cliente potencial [!DNL Salesforce] como o filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=salesforceLeadId1,salesforceLeadId2 |
   |---|

   Você pode usar os valores desses campos para sincronizar com seu objeto de Cliente Potencial/Contato do [!DNL Salesforce].

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de clientes em potencial do Marketo</strong></td>
        <td><strong>Campo de clientes em potencial/contatos do <span class="dnl">Salesforce</span></strong></td>
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

   Documentação da API REST de cliente potencial: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/getLeadByIdUsingGET){target="_blank"}.

   O uso adequado dos campos externos é a chave para uma sincronização bem-sucedida não nativa. Se não conseguir ver os dados em algumas exibições, é provável que um determinado campo não tenha sido sincronizado corretamente. Por exemplo, se as atividades e os momentos interessantes de um lead não forem exibidos ao pesquisar o widget MSI em sua Conta, é provável que a empresa do lead ou a Conta não tenha sido sincronizada corretamente. Executar uma solicitação GET para este cliente potencial ao especificar os campos externos ajudará a verificar se o cliente potencial foi sincronizado corretamente. Além disso, o email do vendedor externo no Marketo deve corresponder ao email desse usuário no Salesforce. Os dados podem não ser exibidos na guia Marketo no Salesforce se os emails não corresponderem.
