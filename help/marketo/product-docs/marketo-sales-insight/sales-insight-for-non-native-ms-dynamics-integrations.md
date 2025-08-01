---
description: '[!DNL Sales Insight] para MS [!DNL Dynamics] Integrações não nativas - Documentação do Marketo - Documentação do produto'
title: '[!DNL Sales Insight] para MS [!DNL Dynamics] Integrações Não Nativas'
exl-id: 07613ff8-b197-4a3d-88e9-720b68a6b8da
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 0%

---

# [!DNL Sales Insight] para integrações do MS [!DNL Dynamics] não nativo {#sales-insight-for-non-native-ms-dynamics-integrations}

Se sua conta do Adobe Marketo Engage estiver conectada ao MS [!DNL Dynamics] por meio de uma integração personalizada ou não nativa, use este artigo para configurar o [!DNL Sales Insight].

>[!PREREQUISITES]
>
>* O recurso &quot;MSI não nativo&quot; é ativado para a instância do Marketo antes de você iniciar a configuração do MSI. Se não estiver e você já tiver comprado o recurso, contate o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Se você ainda não adquiriu esse recurso, entre em contato com a equipe de conta da Adobe (seu gerente de conta).
>* Baixe o [Pacote MSI para Sincronização Personalizada](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.
>* Uma assinatura do MS Dynamics com Instalação MSI (só há suporte para o [Dynamics Online](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online.md){target="_blank"} no momento).
>* API REST do Marketo [configurada com êxito](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}. As APIs CRUD expostas serão a base para executar a sincronização não nativa.
>* Leia [esta postagem do blog](https://developers.marketo.com/blog/create-and-associate-leads-companies-and-opportunities-with-the-marketo-rest-api/){target="_blank"} para entender o objeto e as relações.

## A sincronização não nativa bem-sucedida para o MSI requer o seguinte {#successful-non-native-sync-for-msi-requires-the-following}

1. Sincronize o Usuário de Vendas do MS [!DNL Dynamics] com o Marketo.

   O Usuário de Vendas do MS [!DNL Dynamics] é um usuário externo que possui os Clientes Potenciais/Contatos no MS [!DNL Dynamics]. Um Vendedor do Marketo precisa ser substituído pelo Usuário de Vendas do MS [!DNL Dynamics]. O campo externalSalesPersonId é obrigatório para a substituição do Vendedor.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo do Vendedor do Marketo</strong></td>
        <td><strong>Campo de usuários do MS <span class="dnl">Dynamics</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>Identificador global exclusivo que não diferencia maiúsculas de minúsculas do usuário do MS <span class="dnl">Dynamics</span></td>
      <td><p>Identifica o registro de Vendedor do Marketo para um objeto de Usuário do MS <span class="dnl">Dynamics</span> externo.</p><p>É obrigatório que o Vendedor seja sincronizado primeiro antes de sincronizar os outros objetos para que os relacionamentos adequados sejam criados.</p></td>
     </tr>
    </tbody>
   </table>

   * [Documentação de API para Vendedor](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/sales-persons){target="_blank"}
   * [Documentação de API para sincronizar o Vendedor](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizar as Contas do MS [!DNL Dynamics] com a Marketo.

   Será necessário substituir uma Empresa Marketo pela Conta MS [!DNL Dynamics]. Os campos _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para a substituição da Empresa.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de empresa do Marketo</strong></td>
        <td><strong>Campo de Conta do MS <span class="dnl">Dynamics</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>Identificador exclusivo global sem diferenciação de maiúsculas e minúsculas da conta do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica um registro da Marketo Company para um objeto externo de Conta do MS <span class="dnl">Dynamics</span>.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>Identificador exclusivo global sem distinção entre maiúsculas e minúsculas do usuário de vendas do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica um registro da Marketo Company para um objeto de usuário de vendas do MS <span class="dnl">Dynamics</span> externo que é o proprietário da conta.<br><br>Também usado no Marketo para associar a Empresa ao Vendedor que possui o registro da Empresa. É obrigatório sincronizar o Vendedor primeiro antes de definir esse campo.</td>
     </tr>
    </tbody>
   </table>

   * Documentação de API para Empresas: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/companies](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/companies){target="_blank"}
   * Documentação da API para sincronização de Empresas: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Sales-Persons/operation/syncSalesPersonsUsingPOST){target="_blank"}

1. Sincronizar Clientes Potenciais/Contatos do MS [!DNL Dynamics] com a Marketo.

   Você precisará substituir um cliente em potencial da Marketo pelo cliente em potencial/contato do MS [!DNL Dynamics]. Os campos _externalPersonId_, _externalSalesPersonId_ e _externalCompanyId_ são obrigatórios para a substituição do lead.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de clientes em potencial do Marketo</strong></td>
        <td><strong>Campo Cliente Potencial/Contato do MS <span class="dnl">Dynamics</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalPersonId</td>
        <td>Identificador exclusivo global do Cliente Potencial/Contato do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica o registro de cliente potencial da Marketo para um objeto de contato/cliente potencial do MS <span class="dnl">Dynamics</span> externo.<br><br>Este é um novo campo introduzido para Não Nativo MSI.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>Identificador exclusivo global sem distinção entre maiúsculas e minúsculas do usuário de vendas do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica o objeto de Usuário de Vendas do MS <span class="dnl">Dynamics</span> externo que é proprietário deste Cliente Potencial/Contato.<br><br>Também relaciona o cliente potencial com o Vendedor na Marketo. É obrigatório sincronizar corretamente o Vendedor primeiro.</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>Identificador exclusivo global sem diferenciação de maiúsculas e minúsculas da conta do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica o objeto de Conta do MS <span class="dnl">Dynamics</span> externo ao qual o Cliente Potencial/Contato pertence.<br><br>Também relaciona o registro de cliente potencial a uma Empresa no Marketo. É obrigatório que a Conta do MS <span class="dnl">Dynamics</span> seja sincronizada corretamente primeiro.</td>
     </tr>
    </tbody>
   </table>

   * Documentação de API para clientes em potencial: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/lead-database](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/lead-database){target="_blank"}
   * Documentação da API para clientes em potencial de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"}

1. Sincronizar as Oportunidades do MS [!DNL Dynamics] ao Marketo.

   Será necessário substituir uma Oportunidade da Marketo pela Oportunidade do MS [!DNL Dynamics]. Os campos _externalOpportunityId_, _externalCompanyId_ e _externalSalesPersonId_ são obrigatórios para a substituição da Oportunidade.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de objeto de oportunidade do Marketo</strong></td>
        <td><strong>Campo de objeto de oportunidade do MS <span class="dnl">Dynamics</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
        <td>Identificador exclusivo global do Cliente Potencial/Contato do MS <span class="dnl">Dynamics</span></td>
      <td>Identifica o registro de Oportunidade da Marketo para um objeto de Oportunidade MS <span class="dnl">Dynamics</span> externo.</td>
     </tr>
     <tr>
      <td>externalCompanyId</td>
        <td>Identificador exclusivo global sem diferenciação de maiúsculas e minúsculas da conta do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica o objeto de Conta do MS <span class="dnl">Dynamics</span> externo ao qual esta Oportunidade pertence. <br><br>É obrigatório que a conta do MS <span class="dnl">Dynamics</span> seja sincronizada corretamente primeiro.</td>
     </tr>
     <tr>
      <td>externalSalesPersonId</td>
        <td>Identificador exclusivo global sem distinção entre maiúsculas e minúsculas do usuário de vendas do MS <span class="dnl">Dynamics</span></td>
        <td>Identifica o objeto de Usuário de Vendas do MS <span class="dnl">Dynamics</span> externo que é proprietário desta Oportunidade. </td>
     </tr>
    </tbody>
   </table>

   * Documentação de API da oportunidade: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentação da API para oportunidades de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar Funções de Contato do MS [!DNL Dynamics] com o Marketo.

   As Funções do Contato do MS [!DNL Dynamics] para uma Oportunidade do MS [!DNL Dynamics] podem ser sincronizadas por meio da Função da Oportunidade do Marketo. O registro da Função de Oportunidade exige os campos _externalOpportunityId_, _role_ e _leadId_.

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de função da oportunidade Marketo</strong></td>
        <td><strong>Campo de Função do Contato do MS <span class="dnl">Dynamics</span></strong></td>
      <td><strong>Descrição</strong></td>
     </tr>
     <tr>
      <td>externalOpportunityId</td>
        <td>Identificador exclusivo global sem diferenciação de maiúsculas e minúsculas de oportunidade do MS <span class="dnl">Dynamics</span></td>
      <td>Identifica a Função de oportunidade do Marketo para um objeto de oportunidade MS <span class="dnl">Dynamics</span> externo.<br><br>É obrigatório que a Oportunidade do MS <span class="dnl">Dynamics</span> seja sincronizada corretamente primeiro.</td>
     </tr>
     <tr>
      <td>leadId</td>
      <td>N/D, essa seria uma ID de cliente potencial da Marketo</td>
        <td>Esta seria a ID do cliente em potencial do Marketo do Contato sincronizado do MS <span class="dnl">Dynamics</span>.<br><br>Depois que o contato for sincronizado no Marketo, você poderá usar o identificador exclusivo global do MS <span class="dnl">Dynamics</span> Contact, que não diferencia maiúsculas de minúsculas, como externalPersonId e consultar o Marketo Lead usando a API REST do Marketo.</td>
     </tr>
     <tr>
      <td>função</td>
        <td>O campo Função do Contato do MS <span class="dnl">Dynamics</span></td>
      <td>Descreve a função do contato para esta oportunidade.</td>
     </tr>
    </tbody>
   </table>

   * Documentação de API da oportunidade: [https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities){target="_blank"}
   * Documentação da API para oportunidades de sincronização: [https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Opportunities/operation/syncOpportunitiesUsingPOST){target="_blank"}

1. Sincronizar campos de Pontuação de Último Momento Interessante/MSI ao MS [!DNL Dynamics].

   Depois que os objetos do MS [!DNL Dynamics] forem sincronizados corretamente com o Marketo, você poderá aproveitar os recursos do MSI. Os campos Último momento interessante/Pontuação do MSI serão expostos na API REST para leads. Esses campos são calculados pelo MSI e são somente leitura.

   Os campos Último momento interessante/Pontuação de um lead da Marketo precisarão ser sincronizados regularmente com o MS [!DNL Dynamics] usando o ponto de extremidade REST API Lead. Consulte esse ponto de extremidade para um cliente potencial da Marketo usando a _externalPersonId_ como o filterType e transmitindo a GUID do cliente potencial do MS [!DNL Dynamics] como o filterValue.

   | GET /rest/v1/leads.json?filterType=externalPersonId&amp;filterValues=MS DynamicsLeadId1,MS DynamicsLeadId2 |
   |---|

   Em seguida, você pode usar os valores desses campos para sincronizar com seu objeto de Cliente Potencial/Contato do MS [!DNL Dynamics].

   <table>
    <colgroup>
     <col>
     <col>
     <col>
    </colgroup>
    <tbody>
     <tr>
      <td><strong>Campo de clientes em potencial do Marketo</strong></td>
        <td><strong>Campo Cliente Potencial/Contato do MS <span class="dnl">Dynamics</span></strong></td>
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
