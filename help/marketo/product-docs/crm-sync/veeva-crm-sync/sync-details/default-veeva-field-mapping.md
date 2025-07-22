---
description: Padrão [!DNL Veeva] Mapeamento de campos - Documentação do Marketo - Documentação do produto
title: 'Mapeamento de Campo Padrão [!DNL Veeva] '
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 47%

---

# Mapeamento de Campo [!DNL Veeva] Padrão {#default-veeva-field-mapping}

Inicialmente, ao sincronizar sua conta do Marketo Engage com o [!DNL Veeva], a Marketo faz automaticamente essas associações entre seus campos internos do [!DNL Veeva] e do Marketo. O Marketo também sincronizará os campos personalizados em suas Contas e Contatos.

## Campos de contato {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>Campo do SFDC</th>
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
      <td>Endereço de email</td>
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
      <th>Campo do SFDC</th>
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
      <td>Tipo SFDC</td>
    </tr>
    <tr>
      <td>Site</td>
      <td>Site</td>
    </tr>
  </tbody>
</table>

## Campos do sistema relacionados a [!DNL Veeva] no Marketo (somente leitura) {#veeva-related-system-fields-in-marketo}

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
      <td>[!DNL Veeva] ID</td>
      <td>A Id de [!DNL Salesforce] de 18 caracteres</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] Tipo</td>
      <td>Entre em contato com. Se estiver vazio, o lead existirá somente como uma pessoa no Marketo</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] Data de criação</td>
      <td>Data de criação no SFDC (pode ser diferente de Criado no Marketo)</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] foi excluído</td>
      <td>A pessoa costumava estar no SFDC, mas foi excluída e agora reside somente no Marketo</td>
    </tr>
  </tbody>
</table>
