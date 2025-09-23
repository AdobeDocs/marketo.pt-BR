---
description: Mapeamento de campo padrão do Dynamics - Documentação do Marketo - Documentação do produto
title: Mapeamento de campos padrão do Dynamics
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 3%

---

# Mapeamento de campos padrão do Dynamics {#default-dynamics-field-mapping}

Inicialmente, ao sincronizar sua conta do Marketo Engage com o Microsoft, o Marketo faz automaticamente essas associações entre seus campos integrados do Dynamics e do Marketo.  O Marketo também sincronizará seus campos personalizados em clientes potenciais, contas, oportunidades e contatos.

## Campos de leads {#lead-fields}

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
      <td>[!UICONTROL Data de Criação do Microsoft]</td>
      <td>[!UICONTROL Criado Em]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL Saudação]</td>
      <td>[!UICONTROL Saudação]</td>
      <td>saudação</td>
    </tr>
    <tr>
      <td>[!UICONTROL Primeiro]</td>
      <td>[!UICONTROL Nome]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Meio]</td>
      <td>[!UICONTROL Nome do Meio]</td>
      <td>nome do meio</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último]</td>
      <td>[!UICONTROL Sobrenome]</td>
      <td>sobrenome</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>endereço_de_email1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cargo]</td>
      <td>[!UICONTROL Cargo]</td>
      <td>título do trabalho</td>
    </tr>
    <tr>
      <td>[!UICONTROL Telefone]</td>
      <td>[!UICONTROL Telefone Comercial]</td>
      <td>telefone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Celular]</td>
      <td>celular</td>
    </tr>
    <tr>
      <td>[!UICONTROL Fax]</td>
      <td>[!UICONTROL Fax]</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço]</td>
      <td>[!UICONTROL Rua 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cidade]</td>
      <td>[!UICONTROL Cidade]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado]</td>
      <td>[!UICONTROL Estado/Província]</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>[!UICONTROL País]</td>
      <td>[!UICONTROL País/Região]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL CEP]</td>
      <td>[!UICONTROL CEP]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Pessoa Source]</td>
      <td>[!UICONTROL Source de Cliente Potencial]</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status de Pessoa]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Motivo do Status]</td>
      <td>[!UICONTROL Motivo do Status]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anotações de Pessoa]</td>
      <td>[!UICONTROL Descrição]</td>
      <td>descrição</td>
    </tr>
    <tr>
      <td>[!UICONTROL Não Chamar]</td>
      <td>[!UICONTROL Não Permitir Chamadas Telefônicas]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cancelamento de Assinatura]</td>
      <td>[!UICONTROL Não enviar email em massa]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Classificação de pessoa]</td>
      <td>[!UICONTROL Classificação]</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço 2 do Microsoft]</td>
      <td>[!UICONTROL Rua 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço 3 do Microsoft]</td>
      <td>[!UICONTROL Rua 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Não Enviar Email]</td>
      <td>[!UICONTROL Não Permitir Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Não Enviar Fax]</td>
      <td>[!UICONTROL Não Permitir Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Não Enviar Material de Marketing]</td>
      <td>[!UICONTROL Material de Marketing]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Telefone Residencial Microsoft]</td>
      <td>[!UICONTROL Telefone Residencial]</td>
      <td>telefone2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Método Preferencial De Contato Do Microsoft]</td>
      <td>[!UICONTROL Método Preferencial de Contato]</td>
      <td>preferredcontactmethods code</td>
    </tr>
    <tr>
      <td>[!UICONTROL Tópico Microsoft]</td>
      <td>[!UICONTROL Tópico]</td>
      <td>assunto</td>
    </tr>
    <tr>
      <td>[!UICONTROL Data do último momento interessante]</td>
      <td>[!UICONTROL Data do último momento interessante]</td>
      <td>mkt_lastinteressingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Descrição do último momento interessante]</td>
      <td>[!UICONTROL Descrição do último momento interessante]</td>
      <td>mkt_lastinteressingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Última fonte de momento interessante]</td>
      <td>[!UICONTROL Última fonte de momento interessante]</td>
      <td>mkt_leadinteressingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último tipo de momento interessante]</td>
      <td>[!UICONTROL Último tipo de momento interessante]</td>
      <td>mkt_lastinteressingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Empresa]</td>
      <td>[!UICONTROL Nome da Empresa]</td>
      <td>company name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Pontuação Relativa]</td>
      <td>[!UICONTROL Pontuação Relativa]</td>
      <td>mkt_relativeScore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Prioridade]</td>
      <td>[!UICONTROL Prioridade]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Urgência Relativa]</td>
      <td>[!UICONTROL Urgência]</td>
      <td>mkt_urgência</td>
    </tr>
    <tr>
      <td>[!UICONTROL Assunto]</td>
      <td>[!UICONTROL Tópico]</td>
      <td>assunto</td>
    </tr>
    <tr>
      <td>[!UICONTROL Receita Anual]</td>
      <td>[!UICONTROL Receita Anual]</td>
      <td>Receita</td>
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
      <td>[!UICONTROL Proprietário] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Criado Em]</td>
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
      <td>[!UICONTROL Data de Criação do Microsoft]</td>
      <td>[!UICONTROL Criado Em]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL Saudação]</td>
      <td>[!UICONTROL Saudação]</td>
      <td>saudação</td>
    </tr>
    <tr>
      <td>[!UICONTROL Primeiro]</td>
      <td>[!UICONTROL Nome]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL Meio]</td>
      <td>[!UICONTROL Nome do Meio]</td>
      <td>nome do meio</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último]</td>
      <td>[!UICONTROL Sobrenome]</td>
      <td>sobrenome</td>
    </tr>
    <tr>
      <td>[!UICONTROL Email]</td>
      <td>[!UICONTROL Email]</td>
      <td>endereço_de_email1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cargo]</td>
      <td>[!UICONTROL Cargo]</td>
      <td>título do trabalho</td>
    </tr>
    <tr>
      <td>[!UICONTROL Telefone]</td>
      <td>[!UICONTROL Telefone Comercial]</td>
      <td>telefone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Mobile]</td>
      <td>[!UICONTROL Celular]</td>
      <td>celular</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço]</td>
      <td>[!UICONTROL Endereço 1: Rua 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cidade]</td>
      <td>[!UICONTROL Endereço 1: Cidade]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estado]</td>
      <td>[!UICONTROL Endereço 1: Estado/Província]</td>
      <td>address1_stateorProvince</td>
    </tr>
    <tr>
      <td>[!UICONTROL País]</td>
      <td>[!UICONTROL Endereço 1: País/Região]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL CEP]</td>
      <td>[!UICONTROL Endereço 1: CEP]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status de Pessoa]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Motivo do Status]</td>
      <td>[!UICONTROL Motivo do Status]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Não Chamar]</td>
      <td>[!UICONTROL Não Permitir Chamadas Telefônicas]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cancelamento de Assinatura]</td>
      <td>[!UICONTROL Não enviar email em massa]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço 2 do Microsoft]</td>
      <td>[!UICONTROL Endereço 1: Rua 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço 3 do Microsoft]</td>
      <td>[!UICONTROL Endereço 1: Rua 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Não Enviar Email]</td>
      <td>[!UICONTROL Não Permitir Emails]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Telefone Residencial Microsoft]</td>
      <td>[!UICONTROL Telefone Residencial]</td>
      <td>telefone2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Método Preferencial De Contato Do Microsoft]</td>
      <td>[!UICONTROL Método Preferencial De Contato]</td>
      <td>preferredcontactmethods code</td>
    </tr>
    <tr>
      <td>[!UICONTROL Data do último momento interessante]</td>
      <td>[!UICONTROL Data do último momento interessante]</td>
      <td>mkt_lastinteressingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL Último tipo de momento interessante]</td>
      <td>[!UICONTROL Último tipo de momento interessante]</td>
      <td>mkt_lastinteressingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL Última fonte de momento interessante]</td>
      <td>[!UICONTROL Última fonte de momento interessante]</td>
      <td>mkt_leadinteressingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL Descrição do último momento interessante]</td>
      <td>[!UICONTROL Descrição do último momento interessante]</td>
      <td>mkt_lastinteressingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Não Enviar Material de Marketing]</td>
      <td>[!UICONTROL Material de Marketing]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Não Enviar Fax]</td>
      <td>[!UICONTROL Microsoft Não Enviar Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Prioridade]</td>
      <td>[!UICONTROL Prioridade]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL Urgência Relativa]</td>
      <td>[!UICONTROL Urgência]</td>
      <td>mkt_urgência</td>
    </tr>
    <tr>
      <td>[!UICONTROL Pontuação Relativa]</td>
      <td>[!UICONTROL Pontuação Relativa]</td>
      <td>mkt_relativeScore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anotações de Pessoa]</td>
      <td>[!UICONTROL Descrição]</td>
      <td>descrição </td>
    </tr>
    <tr>
      <td>[!UICONTROL Pontuação de Pessoa]</td>
      <td>[!UICONTROL Pontuação de lead]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anotações de Pessoa]</td>
      <td>[!UICONTROL Descrição]</td>
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
      <td>[!UICONTROL Proprietário] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Criado Em]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL Nome da Empresa]</td>
      <td>parentcustomerid</td>
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
      <td>[!UICONTROL Account (a)]</td>
      <td>[!UICONTROL Conta]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço de Cobrança]</td>
      <td>[!UICONTROL Endereço 1: Rua 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cidade de Cobrança]</td>
      <td>[!UICONTROL Endereço 1: Cidade]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL País de Cobrança]</td>
      <td>[!UICONTROL Endereço 1: País/Região]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código Postal de Cobrança]</td>
      <td>[!UICONTROL Endereço 1: CEP]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço de Cobrança do Microsoft 2]</td>
      <td>[!UICONTROL Endereço 1: Rua 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Endereço de Cobrança 3 do Microsoft]</td>
      <td>[!UICONTROL Endereço 1: Rua 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Telefone Principal]</td>
      <td>[!UICONTROL Telefone Principal]</td>
      <td>telefone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL Tipo de Negócio]</td>
      <td>[!UICONTROL Tipo de Negócio]</td>
      <td>business stypecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Número de Conta do Microsoft]</td>
      <td>[!UICONTROL Número de Conta]</td>
      <td>número da conta</td>
    </tr>
    <tr>
      <td>[!UICONTROL Status da Empresa Microsoft]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Receita Anual]</td>
      <td>[!UICONTROL Receita Anual]</td>
      <td>Receita</td>
    </tr>
    <tr>
      <td>[!UICONTROL Anotações da Empresa]</td>
      <td>[!UICONTROL Descrição]</td>
      <td>descrição</td>
    </tr>
    <tr>
      <td>[!UICONTROL Setor]</td>
      <td>[!UICONTROL Setor]</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código SIC]</td>
      <td>[!UICONTROL Código SIC]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Site]</td>
      <td>[!UICONTROL Site]</td>
      <td>site</td>
    </tr>
    <tr>
      <td>[!UICONTROL Número de Funcionários]</td>
      <td>[!UICONTROL Número de Funcionários]</td>
      <td>numberofemployees</td>
    </tr>
    <tr>
      <td>[!UICONTROL Código SIC]</td>
      <td>[!UICONTROL Código SIC]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Empresa]</td>
      <td>[!UICONTROL Nome da Conta]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Número de Funcionários]</td>
      <td>[!UICONTROL Número de Funcionários]</td>
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
      <td>[!UICONTROL Proprietário] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Criado Em]</td>
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
      <td>[!UICONTROL Fechar Probabilidade]</td>
      <td>[!UICONTROL Probabilidade]</td>
      <td>probabilidade de fechamento</td>
    </tr>
    <tr>
      <td>[!UICONTROL Estágio]</td>
      <td>[!UICONTROL Status]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Data de Fechamento Real]</td>
      <td>[!UICONTROL Data de Fechamento Real]</td>
      <td>data de fechamento real</td>
    </tr>
    <tr>
      <td>[!UICONTROL Nome]</td>
      <td>[!UICONTROL Tópico]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL Valor Estimado]</td>
      <td>[!UICONTROL Est. Receita]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL Descrição]</td>
      <td>[!UICONTROL Descrição]</td>
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
      <td>[!UICONTROL Proprietário] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL Oportunidade]</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL Cliente em Potencial]</td>
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
      <td>[!UICONTROL Tipo Microsoft]</td>
      <td>Cliente Potencial ou Contato. Se estiver vazio, o lead existirá somente como uma pessoa no Marketo</td>
    </tr>
    <tr>
      <td>[!UICONTROL Data de Criação do Microsoft]</td>
      <td>Data de criação em [!DNL MS Dynamics] (pode ser diferente de Criado no Marketo)</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft foi excluído]</td>
      <td>A pessoa costumava estar no Microsoft, mas foi excluída e agora reside somente no Marketo</td>
    </tr>
  </tbody>
</table>
