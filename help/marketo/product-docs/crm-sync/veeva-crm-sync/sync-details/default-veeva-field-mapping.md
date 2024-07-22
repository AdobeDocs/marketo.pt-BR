---
description: Mapeamento De Campo Padrão Do Veeva - Documentação Do Marketo - Documentação Do Produto
title: Mapeamento de campo Veeva padrão
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 44%

---

# Mapeamento de campo Veeva padrão {#default-veeva-field-mapping}

Quando você sincroniza inicialmente sua conta Marketo Engage com o Veeva, o Marketo faz automaticamente essas associações entre seus campos Veeva e Marketo incorporados. O Marketo também sincronizará os campos personalizados em suas Contas e Contatos.

## Campos de contato {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo SFDC</th>
      <th>Campo do Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Data de nascimento</td>
      <td>Data de nascimento</td>
    </tr>
    <tr>
      <td>Data de criação</td>
      <td>Data de criação SFDC</td>
    </tr>
    <tr>
      <td>Descrição do contato</td>
      <td>Observações sobre a pessoa</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Endereço de e-mail</td>
    </tr>
    <tr>
      <td>Fax comercial</td>
      <td>Número de fax</td>
    </tr>
    <tr>
      <td>Nome</td>
      <td>Nome</td>
    </tr>
    <tr>
      <td>Cancelamento de opção de e-mail</td>
      <td>Inscrição cancelada</td>
    </tr>
    <tr>
      <td>Excluído</td>
      <td>SFDC é excluído</td>
    </tr>
    <tr>
      <td>Sobrenome</td>
      <td>Sobrenome</td>
    </tr>
    <tr>
      <td>Fonte do lead</td>
      <td>Origem</td>
    </tr>
    <tr>
      <td>Pontuação do lead</td>
      <td>Pontuação</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>Cidade</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>País</td>
    </tr>
    <tr>
      <td>MailingPostalCode</td>
      <td>Código postal</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>Estado</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>Endereço</td>
    </tr>
    <tr>
      <td>Celular</td>
      <td>Número do celular</td>
    </tr>
    <tr>
      <td>Telefone comercial</td>
      <td>Número de telefone</td>
    </tr>
    <tr>
      <td>Saudação</td>
      <td>Saudação</td>
    </tr>
    <tr>
      <td>Título</td>
      <td>Nome do cargo</td>
    </tr>
  </tbody>
</table>

## Campos de conta {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo SFDC</th>
      <th>Campo do Marketo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Receita anual</td>
      <td>Receita anual</td>
    </tr>
    <tr>
      <td>Cidade de cobrança</td>
      <td>Cidade de cobrança</td>
    </tr>
    <tr>
      <td>País de cobrança</td>
      <td>País de cobrança</td>
    </tr>
    <tr>
      <td>Código postal/CEP de cobrança</td>
      <td>Código postal de cobrança</td>
    </tr>
    <tr>
      <td>Estado/Província de Cobrança</td>
      <td>Estado de cobrança</td>
    </tr>
    <tr>
      <td>Rua de Cobrança</td>
      <td>Endereço de cobrança</td>
    </tr>
    <tr>
      <td>Descrição da conta</td>
      <td>Observações sobre a empresa</td>
    </tr>
    <tr>
      <td>Setor</td>
      <td>Setor</td>
    </tr>
    <tr>
      <td>Excluído</td>
      <td>SFDC é excluído</td>
    </tr>
    <tr>
      <td>Nome da conta</td>
      <td>Nome da empresa</td>
    </tr>
    <tr>
      <td>Funcionários</td>
      <td>Núm. funcionários</td>
    </tr>
    <tr>
      <td>Telefone da conta</td>
      <td>Telefone principal</td>
    </tr>
    <tr>
      <td>Código SIC</td>
      <td>Código SIC</td>
    </tr>
    <tr>
      <td>Site da conta</td>
      <td>Site</td>
    </tr>
    <tr>
      <td>Tipo de conta</td>
      <td>SFDC - Tipo</td>
    </tr>
    <tr>
      <td>Site</td>
      <td>Site</td>
    </tr>
  </tbody>
</table>

## Campos de sistema relacionados ao Veeva no Marketo (somente leitura) {#veeva-related-system-fields-in-marketo}

Esses campos são criados no Marketo, mas não podem ser ajustados pelos clientes.

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo</th>
      <th>Descrição</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Veeva Id</td>
      <td>A ID do Salesforce de 18 caracteres</td>
    </tr>
    <tr>
      <td>Veeva Type</td>
      <td>Entre em contato com. Se estiver vazio, o lead existirá somente como uma pessoa no Marketo</td>
    </tr>
    <tr>
      <td>Data de criação da Veeva</td>
      <td>Data de criação no SFDC (pode ser diferente de Criado no Marketo)</td>
    </tr>
    <tr>
      <td>Veeva é excluído</td>
      <td>A pessoa costumava estar no SFDC, mas foi excluída e agora reside somente no Marketo</td>
    </tr>
  </tbody>
</table>
