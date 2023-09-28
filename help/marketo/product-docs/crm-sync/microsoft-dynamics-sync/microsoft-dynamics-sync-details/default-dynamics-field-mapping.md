---
description: Mapeamento de campo padrão do Dynamics - Documentação do Marketo - Documentação do produto
title: Mapeamento de campos padrão do Dynamics
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 09c70bb891f5cc93553c1f8dd0fb58dfd407fa81
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 42%

---

# Mapeamento de campos padrão do Dynamics {#default-dynamics-field-mapping}

Inicialmente, ao sincronizar sua conta do Marketo com o Microsoft, o Marketo faz automaticamente essas associações entre seus campos integrados do Dynamics e do Marketo.  O Marketo também sincronizará seus campos personalizados em clientes potenciais, contas, oportunidades e contatos.

## Campos de lead {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do Marketo</th>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Microsoft - Data de criação</td>
      <td>Criado em</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>Saudação</td>
      <td>Saudação</td>
      <td>saudação</td>
    </tr>
    <tr>
      <td>Primeiro</td>
      <td>Nome</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Meio</td>
      <td>Nome do meio</td>
      <td>nome do meio</td>
    </tr>
    <tr>
      <td>Último</td>
      <td>Sobrenome</td>
      <td>sobrenome</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Email</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>Cargo</td>
      <td>Cargo</td>
      <td>título do trabalho</td>
    </tr>
    <tr>
      <td>Telefone</td>
      <td>Telefone comercial</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Celular</td>
      <td>Celular</td>
      <td>celular</td>
    </tr>
    <tr>
      <td>Fax</td>
      <td>Fax</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>Endereço</td>
      <td>Folha 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Cidade</td>
      <td>Cidade</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Estado</td>
      <td>Estado/Província</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>País</td>
      <td>País/Região</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal</td>
      <td>CEP/Código postal</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Fonte de pessoas</td>
      <td>Fonte do lead</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>Status da pessoa</td>
      <td>Status</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Motivo do status</td>
      <td>Motivo do status</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Observações sobre a pessoa</td>
      <td>Descrição</td>
      <td>descrição</td>
    </tr>
    <tr>
      <td>Não ligar</td>
      <td>Não Permitir Chamadas Telefônicas</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Inscrição cancelada</td>
      <td>Não enviar email em massa</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Classificação da pessoa</td>
      <td>Classificação</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>Microsoft - Endereço 2</td>
      <td>Folha 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft - Endereço 3</td>
      <td>Folha 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft - Não enviar e-mail</td>
      <td>Não Permitir Emails</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft - Não enviar fax</td>
      <td>Não Permitir Fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Microsoft - Não enviar material de marketing</td>
      <td>Material de marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft - Telefone residencial</td>
      <td>Telefone residencial</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Método Preferencial De Contato Da Microsoft</td>
      <td>Método preferencial de contato</td>
      <td>preferredcontactmethods code</td>
    </tr>
    <tr>
      <td>Microsoft - Tópico</td>
      <td>Tópico</td>
      <td>assunto</td>
    </tr>
    <tr>
      <td>Data do último momento interessante</td>
      <td>Data do último momento interessante</td>
      <td>mkt_lastinteressingmomentdate</td>
    </tr>
    <tr>
      <td>Desc. Último momento interessante</td>
      <td>Desc. Último momento interessante</td>
      <td>mkt_lastinteressingmomentdesc</td>
    </tr>
    <tr>
      <td>Última origem de momento interessante</td>
      <td>Última origem de momento interessante</td>
      <td>mkt_leadinteressingmomentsource</td>
    </tr>
    <tr>
      <td>Último tipo de momento interessante</td>
      <td>Último tipo de momento interessante</td>
      <td>mkt_lastinteressingmomenttype</td>
    </tr>
    <tr>
      <td>Empresa</td>
      <td>Nome da empresa</td>
      <td>company name</td>
    </tr>
    <tr>
      <td>Pontuação relativa</td>
      <td>Pontuação relativa</td>
      <td>mkt_relativeScore</td>
    </tr>
    <tr>
      <td>Prioridade</td>
      <td>Prioridade</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgência relativa</td>
      <td>urgência</td>
      <td>mkt_urgência</td>
    </tr>
    <tr>
      <td>Assunto</td>
      <td>Tópico</td>
      <td>assunto</td>
    </tr>
    <tr>
      <td>Receita anual</td>
      <td>Receita anual</td>
      <td>receita</td>
    </tr>
  </tbody>
</table>

Os campos de cliente em potencial abaixo são sincronizados para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietário </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>criado em</td>
      <td>createdon</td>
    </tr>
  </tbody>
</table>

## Campos de contato {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do Marketo</th>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Microsoft - Data de criação</td>
      <td>Criado em</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>Saudação</td>
      <td>Saudação</td>
      <td>saudação</td>
    </tr>
    <tr>
      <td>Primeiro</td>
      <td>Nome</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>Meio</td>
      <td>Nome do meio</td>
      <td>nome do meio</td>
    </tr>
    <tr>
      <td>Último</td>
      <td>Sobrenome</td>
      <td>sobrenome</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Email</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>Cargo</td>
      <td>Cargo</td>
      <td>título do trabalho</td>
    </tr>
    <tr>
      <td>Telefone</td>
      <td>Telefone comercial</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Celular</td>
      <td>Celular</td>
      <td>celular</td>
    </tr>
    <tr>
      <td>Endereço</td>
      <td>Endereço 1: Rua 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Cidade</td>
      <td>Endereço 1: Cidade</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>Estado</td>
      <td>Endereço 1: Estado/Província</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>País</td>
      <td>Endereço 1: País/Região</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal</td>
      <td>Endereço 1: CEP</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Status da pessoa</td>
      <td>Status</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Motivo do status</td>
      <td>Motivo do status</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>Não ligar</td>
      <td>Não Permitir Chamadas Telefônicas</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>Inscrição cancelada</td>
      <td>Não enviar email em massa</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>Microsoft - Endereço 2</td>
      <td>Endereço 1: Rua 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft - Endereço 3</td>
      <td>Endereço 1: Rua 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Microsoft - Não enviar e-mail</td>
      <td>Não Permitir Emails</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>Microsoft - Telefone residencial</td>
      <td>Telefone residencial</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>Método Preferencial De Contato Da Microsoft</td>
      <td>Forma Preferencial De Contato</td>
      <td>preferredcontactmethods code</td>
    </tr>
    <tr>
      <td>Data do último momento interessante</td>
      <td>Data do último momento interessante</td>
      <td>mkt_lastinteressingmomentdate</td>
    </tr>
    <tr>
      <td>Último tipo de momento interessante</td>
      <td>Último tipo de momento interessante</td>
      <td>mkt_lastinteressingmomenttype</td>
    </tr>
    <tr>
      <td>Última origem de momento interessante</td>
      <td>Última origem de momento interessante</td>
      <td>mkt_leadinteressingmomentsource</td>
    </tr>
    <tr>
      <td>Desc. Último momento interessante</td>
      <td>Desc. Último momento interessante</td>
      <td>mkt_lastinteressingmomentdesc</td>
    </tr>
    <tr>
      <td>Microsoft - Não enviar material de marketing</td>
      <td>Material de marketing</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>Microsoft - Não enviar fax</td>
      <td>Microsoft - Não enviar fax</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>Prioridade</td>
      <td>Prioridade</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>Urgência relativa</td>
      <td>urgência</td>
      <td>mkt_urgência</td>
    </tr>
    <tr>
      <td>Pontuação relativa</td>
      <td>Pontuação relativa</td>
      <td>mkt_relativeScore</td>
    </tr>
    <tr>
      <td>Observações sobre a pessoa</td>
      <td>Descrição</td>
      <td>descrição </td>
    </tr>
    <tr>
      <td>Pontuação de pessoas</td>
      <td>Pontuação do lead</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>Observações sobre a pessoa</td>
      <td>Descrição</td>
      <td>descrição </td>
    </tr>
  </tbody>
</table>

Os campos Contato abaixo são sincronizados para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietário </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>criado em</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>parentcustomerid</td>
      <td>Nome da empresa</td>
    </tr>
  </tbody>
</table>

## Campos de conta {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do Marketo</th>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Conta (a)</td>
      <td>Conta</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>Endereço de faturamento</td>
      <td>Endereço 1: Rua 1</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>Cidade de faturamento</td>
      <td>Endereço 1: Cidade</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>País de faturamento</td>
      <td>Endereço 1: País/Região</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>Código postal de faturamento</td>
      <td>Endereço 1: CEP</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>Microsoft - Endereço de cobrança 2</td>
      <td>Endereço 1: Rua 2</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>Microsoft - Endereço de cobrança 3</td>
      <td>Endereço 1: Rua 3</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>Telefone principal</td>
      <td>Telefone principal</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>Tipo de negócio</td>
      <td>Tipo de negócio</td>
      <td>business stypecode</td>
    </tr>
    <tr>
      <td>Número da conta do Microsoft</td>
      <td>Número da conta</td>
      <td>número da conta</td>
    </tr>
    <tr>
      <td>Microsoft - Status da empresa</td>
      <td>Status</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Receita anual</td>
      <td>Receita anual</td>
      <td>receita</td>
    </tr>
    <tr>
      <td>Observações sobre a empresa</td>
      <td>Descrição</td>
      <td>descrição</td>
    </tr>
    <tr>
      <td>Setor</td>
      <td>Setor</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Site</td>
      <td>Site</td>
      <td>site</td>
    </tr>
    <tr>
      <td>Núm. funcionários</td>
      <td>Número de funcionários</td>
      <td>numberofemployees</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>Empresa</td>
      <td>Nome da conta</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Núm. funcionários</td>
      <td>Número de funcionários</td>
      <td>numberofemployees</td>
    </tr>
  </tbody>
</table>

Os campos Conta abaixo são sincronizados para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietário </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>criado em</td>
      <td>createdon</td>
    </tr>
  </tbody>
</table>

## Campos de oportunidade {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do Marketo</th>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Fechar probabilidade</td>
      <td>Probabilidade</td>
      <td>probabilidade de fechamento</td>
    </tr>
    <tr>
      <td>Estágio</td>
      <td>status</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>Data de fechamento real</td>
      <td>Data de fechamento real</td>
      <td>data de fechamento real</td>
    </tr>
    <tr>
      <td>Nome</td>
      <td>Tópico</td>
      <td>name</td>
    </tr>
    <tr>
      <td>Valor estimado</td>
      <td>Est. Receita</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>Descrição</td>
      <td>Descrição</td>
      <td>descrição</td>
    </tr>
  </tbody>
</table>

Os campos Conta abaixo são sincronizados para uso interno.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do MS Dynamics</th>
      <th>Nome da API do MS Dynamics</th>
    </tr>
    <tr>
      <td>Proprietário </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>Oportunidade</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>Cliente potencial</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Campos de sistema relacionados ao Microsoft no Marketo (somente leitura) {#microsoft-related-system-fields}

Os campos abaixo são criados no Marketo, mas não podem ser ajustados pelos usuários.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Campo do Marketo</th>
      <th>Descrição</th>
    </tr>
    <tr>
      <td>Tipo Microsoft</td>
      <td>Cliente Potencial ou Contato. Se estiver vazio, o lead existirá somente como uma pessoa no Marketo</td>
    </tr>
    <tr>
      <td>Microsoft - Data de criação</td>
      <td>Data de criação no MS Dynamics (pode ser diferente de Criado no Marketo)</td>
    </tr>
    <tr>
      <td>O Microsoft foi excluído</td>
      <td>A pessoa costumava estar no Microsoft, mas foi excluída e agora reside somente no Marketo</td>
    </tr>
  </tbody>
</table>
