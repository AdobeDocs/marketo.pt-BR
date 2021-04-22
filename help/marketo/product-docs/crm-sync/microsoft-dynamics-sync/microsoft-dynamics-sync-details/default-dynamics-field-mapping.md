---
description: Mapeamento de campo dinâmico padrão - Documentos do Marketo - Documentação do produto
title: Mapeamento de campo dinâmico padrão
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 47%

---

# Mapeamento de campo dinâmico padrão {#default-dynamics-field-mapping}

Ao sincronizar inicialmente sua conta do Marketo com a Microsoft, a Marketo faz automaticamente essas associações entre os campos incorporados do Dynamics e do Marketo.  O Marketo também sincronizará os campos personalizados nos Leads, Accounts, Oportunidades e Contatos.

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
   <td>Criado(a) em</td> 
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
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Último</td> 
   <td>Sobrenome</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>E-mail</td> 
   <td>E-mail</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Nome do cargo</td> 
   <td>Nome do cargo</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Telefone</td> 
   <td>Telefone comercial</td> 
   <td>phone1</td> 
  </tr> 
  <tr> 
   <td>Celular</td> 
   <td>Celular</td> 
   <td>telefone celular</td> 
  </tr> 
  <tr> 
   <td>Fax</td> 
   <td>Fax</td> 
   <td>fax</td> 
  </tr> 
  <tr> 
   <td>Endereço</td> 
   <td>Rua 1</td> 
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
   <td>address1_stateorprovíncia</td> 
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
   <td>Não Permitir chamadas telefônicas</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Inscrição cancelada</td> 
   <td>Não enviar emails em massa</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Classificação da pessoa</td> 
   <td>Classificação</td> 
   <td>leadqualitycode</td> 
  </tr> 
  <tr> 
   <td>Microsoft - Endereço 2</td> 
   <td>Rua 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft - Endereço 3</td> 
   <td>Rua 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft - Não enviar e-mail</td> 
   <td>Não Permitir Emails</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft - Não enviar fax</td> 
   <td>Não Permitir fax</td> 
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
   <td>Telefone2</td> 
  </tr> 
  <tr> 
   <td>Método de Contato Preferencial da Microsoft</td> 
   <td>Método preferencial de contato</td> 
   <td>preferredcontactmetodcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft - Tópico</td> 
   <td>Tópico</td> 
   <td>assunto</td> 
  </tr> 
 </tbody> 
</table>

## Campos de contato {#contact-fields}

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
   <td>Criado(a) em</td> 
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
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>Último</td> 
   <td>Sobrenome</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>E-mail</td> 
   <td>E-mail</td> 
   <td>email address1</td> 
  </tr> 
  <tr> 
   <td>Nome do cargo</td> 
   <td>Nome do cargo</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>Telefone</td> 
   <td>Telefone comercial</td> 
   <td>phone1</td> 
  </tr> 
  <tr> 
   <td>Celular</td> 
   <td>Celular</td> 
   <td>telefone celular</td> 
  </tr> 
  <tr> 
   <td>Endereço</td> 
   <td>Endereço 1: Rua 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>Cidade</td> 
   <td>Endereço 1: Cidade</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>Estado</td> 
   <td>Endereço 1: Estado/Província</td> 
   <td>address1_stateorprovíncia</td> 
  </tr> 
  <tr> 
   <td>País</td> 
   <td>Endereço 1: País/Região</td> 
   <td>address1_country</td> 
   <tr> 
   <td>Código postal</td> 
   <td>Endereço 1: CEP/Código Postal</td> 
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
   <td>Não Permitir chamadas telefônicas</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>Inscrição cancelada</td> 
   <td>Não enviar emails em massa</td> 
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
   <td>Telefone2</td> 
  </tr> 
  <tr> 
   <td>Método de Contato Preferencial da Microsoft</td> 
   <td>Método Preferido De Contato</td> 
   <td>preferredcontactmetodcode</td> 
  </tr> 
 </tbody> 
</table>

## Campos de conta {#account-fields}

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
   <td>Conta (a)</td> 
   <td>Conta</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>Endereço de cobrança</td> 
   <td>Endereço 1: Rua 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>Cidade de cobrança</td> 
   <td>Endereço 1: Cidade</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>País de cobrança</td> 
   <td>Endereço 1: País/Região</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>Código postal de cobrança</td> 
   <td>Endereço 1: CEP/Código Postal</td> 
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
   <td>phone1</td> 
  </tr> 
  <tr> 
   <td>Tipo de negócio</td> 
   <td>Tipo de negócio</td> 
   <td>business esstypecode</td> 
  </tr> 
  <tr> 
   <td>Número de Conta da Microsoft</td> 
   <td>Número da conta</td> 
   <td>accountnumber</td> 
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
 </tbody> 
</table>

## Campos do sistema relacionados à Microsoft no Marketo (somente leitura) {#microsoft-related-system-fields-in-marketo}

Esses campos são criados no Marketo, mas não podem ser ajustados por clientes.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Campo do Marketo</th> 
   <th>Descrição</th> 
  </tr> 
  <tr> 
   <td>Microsoft - Tipo</td> 
   <td>Líder ou Contato. Se estiver vazio, o lead existe apenas como uma pessoa no Marketo</td> 
  </tr> 
  <tr> 
   <td>Microsoft - Data de criação</td> 
   <td>Data de criação no MS Dynamics (pode ser diferente de Criado no Marketo)</td> 
  </tr> 
  <tr> 
   <td>A Microsoft é Excluída</td> 
   <td>A pessoa costumava estar na Microsoft, mas foi excluída e agora vive somente no Marketo</td> 
  </tr> 
 </tbody> 
</table>
