---
unique-page-id: 4719314
description: Mapeamento de campo padrão do Salesforce - Documentos do Marketing - Documentação do produto
title: Mapeamento de campo padrão do Salesforce
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Mapeamento de campo padrão do Salesforce {#default-salesforce-field-mapping}

Quando você sincroniza inicialmente sua conta do Marketo com o Salesforce, o Marketo faz automaticamente essas associações entre os campos incorporados do Salesforce e do Marketo. O Marketo também sincronizará seus campos personalizados em Clientes potenciais, Contas, Oportunidades e Contatos.

## Campos de cliente potencial {#lead-fields}

| Campo SFDC | Campo de marketing |
|---|---|
| Receita anual | Receita anual |
| Cidade | Cidade |
| Empresa | Nome da empresa |
| Data de conversão | Data de conversão do SFDC |
| País | País |
| Data de criação | Data de criação do SFDC |
| Descrição | Notas de pessoa |
| Email | Endereço de email |
| Fax | Número de fax |
| Nome | Nome |
| Opt out de email | Inscrito |
| Indústria | Indústria |
| Convertido | SFDC É Convertido |
| Excluído | O SFDC É Excluído |
| Sobrenome | Sobrenome |
| Fonte de informação | Fonte |
| Pontuação principal | Pontuação |
| Telefone celular | Número de telefone celular |
| Funcionários | Número de funcionários |
| Telefone | Número de telefone |
| CEP/Código postal | Código postal |
| Classificação | Classificação |
| Saudação | Saudação |
| Estado/província | Estado |
| Status | Status |
| Rua | Endereço |
| Título | Cargo |
| Site | Site |

## Campos de contato {#contact-fields}

| Campo SFDC | Campo de marketing |
|---|---|
| Data de nascimento | Data de nascimento |
| Data de criação | Data de criação do SFDC |
| Descrição do contato | Notas de pessoa |
| Email | Endereço de email |
| Fax comercial | Número de fax |
| Nome | Nome |
| Opt out de email | Inscrito |
| Excluído | O SFDC É Excluído |
| Sobrenome | Sobrenome |
| Fonte de informação | Fonte |
| Pontuação principal | Pontuação |
| CidadeCorrespondência | Cidade |
| País para correspondência | País |
| MailPostalCode | Código postal |
| EstadoCorrespondência | Estado |
| EndereçoCorrespondente | Endereço |
| Telefone celular | Número de telefone celular |
| Telefone comercial | Número de telefone |
| Saudação | Saudação |
| Título | Cargo |

## Campos de conta {#account-fields}

| Campo SFDC | Campo de marketing |
|---|---|
| Receita anual | Receita anual |
| Cidade de cobrança | Cidade de cobrança |
| País de cobrança | País de cobrança |
| Código postal/CEP de cobrança | Código postal de cobrança |
| Estado/província de cobrança | Estado de cobrança |
| Billing Street | Endereço de cobrança |
| Descrição da conta | Notas de empresa |
| Indústria | Indústria |
| Excluído | O SFDC É Excluído |
| Nome da conta | Nome da empresa |
| Funcionários | Número de funcionários |
| Telefone da conta | Telefone principal |
| Código SIC | Código SIC |
| Site da conta | Site |
| Tipo de conta | Tipo de SFDC |
| Site | Site |

## Campos de sistema relacionados ao Salesforce no Marketing (somente leitura) {#salesforce-related-system-fields-in-marketo-read-only}

Esses campos são criados no Marketo, mas não podem ser ajustados pelos clientes.

| Campo | Descrição |
|---|---|
| Id SFDC | A ID do Salesforce de 18 caracteres |
| Tipo de SFDC | Cliente potencial ou Contato. Se vazio, o cliente potencial existe somente como uma pessoa em Marketo |
| Data de criação do SFDC | Data de criação no SFDC (pode ser diferente de Criado no Marketing) |
| O SFDC foi Excluído | A pessoa costumava estar no SFDC, mas foi excluída e agora vive apenas em Marketo |
