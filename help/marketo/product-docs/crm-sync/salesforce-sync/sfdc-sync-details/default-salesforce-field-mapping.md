---
unique-page-id: 4719314
description: Mapeamento de campo padrão do Salesforce - Documentação do Marketo - Documentação do produto
title: Mapeamento de campos padrão do Salesforce
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 59%

---

# Mapeamento de campos padrão do Salesforce {#default-salesforce-field-mapping}

Inicialmente, ao sincronizar sua conta do Marketo Engage com o Salesforce, a Marketo faz automaticamente essas associações entre seus campos integrados do Salesforce e do Marketo. O Marketo também sincronizará seus campos personalizados em clientes potenciais, contas, oportunidades e contatos.

## Campos de leads {#lead-fields}

| Campo SFDC | Campo do Marketo |
|---|---|
| Receita anual | Receita anual |
| Cidade | Cidade |
| Empresa | Nome da empresa |
| Data de conversão | SFDC - Data de conversão |
| País | País |
| Data de criação | Data de criação SFDC |
| Descrição | Observações sobre a pessoa |
| Email | Endereço de e-mail |
| Fax | Número de fax |
| Nome | Nome |
| Cancelamento de opção de e-mail | Inscrição cancelada |
| Setor | Setor |
| Convertido | SFDC é convertido |
| Excluído | SFDC é excluído |
| Sobrenome | Sobrenome |
| Fonte do lead | Origem |
| Pontuação do lead | Pontuação |
| Celular | Número do celular |
| Funcionários | Núm. funcionários |
| Telefone | Número de telefone |
| CEP/Código postal | Código postal |
| Classificação | Classificação |
| Saudação | Saudação |
| Estado/Província | Estado |
| Status | Status |
| Rua | Endereço |
| Título | Nome do cargo |
| Site | Site |

## Campos de contato {#contact-fields}

| Campo SFDC | Campo do Marketo |
|---|---|
| Data de nascimento | Data de nascimento |
| Data de criação | Data de criação SFDC |
| Descrição do contato | Observações sobre a pessoa |
| Email | Endereço de e-mail |
| Fax comercial | Número de fax |
| Nome | Nome |
| Cancelamento de opção de e-mail | Inscrição cancelada |
| Excluído | SFDC é excluído |
| Sobrenome | Sobrenome |
| Fonte do lead | Origem |
| Pontuação do lead | Pontuação |
| MailingCity | Cidade |
| MailingCountry | País |
| MailingPostalCode | Código postal |
| MailingState | Estado |
| MailingStreet | Endereço |
| Celular | Número do celular |
| Telefone comercial | Número de telefone |
| Saudação | Saudação |
| Título | Nome do cargo |

## Campos de conta {#account-fields}

| Campo SFDC | Campo do Marketo |
|---|---|
| Receita anual | Receita anual |
| Cidade de cobrança | Cidade de cobrança |
| País de cobrança | País de cobrança |
| Código postal/CEP de cobrança | Código postal de cobrança |
| Estado/Província de Cobrança | Estado de cobrança |
| Rua de Cobrança | Endereço de cobrança |
| Descrição da conta | Observações sobre a empresa |
| Setor | Setor |
| Excluído | SFDC é excluído |
| Nome da conta | Nome da empresa |
| Funcionários | Núm. funcionários |
| Telefone da conta | Telefone principal |
| Código SIC | Código SIC |
| Site da conta | Site |
| Tipo de conta | SFDC - Tipo |
| Site | Site |

## Campos de sistema relacionados ao Salesforce no Marketo (somente leitura) {#salesforce-related-system-fields-in-marketo-read-only}

Esses campos são criados no Marketo, mas não podem ser ajustados pelos clientes.

| Campo | Descrição |
|---|---|
| SFDC - ID | A ID do Salesforce de 18 caracteres |
| SFDC - Tipo | Cliente Potencial ou Contato. Se estiver vazio, o lead existirá somente como uma pessoa no Marketo |
| Data de criação SFDC | Data de criação no SFDC (pode ser diferente de Criado no Marketo) |
| SFDC excluído | A pessoa costumava estar no SFDC, mas foi excluída e agora reside somente no Marketo |
