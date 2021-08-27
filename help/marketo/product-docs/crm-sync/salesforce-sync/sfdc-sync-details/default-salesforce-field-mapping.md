---
unique-page-id: 4719314
description: Mapeamento de campo padrão do Salesforce - Documentos do Marketo - Documentação do produto
title: Mapeamento de campo padrão do Salesforce
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 57%

---

# Mapeamento de campo padrão do Salesforce {#default-salesforce-field-mapping}

Quando você sincroniza inicialmente sua conta do Marketo com o Salesforce, a Marketo faz automaticamente essas associações entre seus campos incorporados do Salesforce e do Marketo. O Marketo também sincronizará os campos personalizados nos Leads, Accounts, Oportunidades e Contatos.

## Campos de lead {#lead-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Receita anual | Receita anual |
| Cidade | Cidade |
| Empresa | Nome da empresa |
| Data de conversão | SFDC - Data de conversão |
| País | País |
| Data de criação | SFDC - Data de criação |
| Descrição | Observações sobre a pessoa |
| E-mail | Endereço de e-mail |
| Fax | Número de fax |
| Nome | Nome |
| Cancelamento de opção de e-mail | Inscrição cancelada |
| Setor | Setor |
| Convertido | SFDC é convertido |
| Excluído | SFDC é excluído |
| Sobrenome | Sobrenome |
| Fonte do lead | Fonte |
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
| Título | Cargo |
| Site | Site |

## Campos de contato {#contact-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Data de nascimento | Data de nascimento |
| Data de criação | SFDC - Data de criação |
| Descrição do contato | Observações sobre a pessoa |
| E-mail | Endereço de e-mail |
| Fax comercial | Número de fax |
| Nome | Nome |
| Cancelamento de opção de e-mail | Inscrição cancelada |
| Excluído | SFDC é excluído |
| Sobrenome | Sobrenome |
| Fonte do lead | Fonte |
| Pontuação do lead | Pontuação |
| Cidade de correspondência | Cidade |
| PaísCorrespondente | País |
| CEPodeCorreio | Código postal |
| EstadoCorrespondente | Estado |
| MailingStreet | Endereço |
| Celular | Número do celular |
| Telefone comercial | Número de telefone |
| Saudação | Saudação |
| Título | Cargo |

## Campos de conta {#account-fields}

| Campo SFDC | Campo Marketo |
|---|---|
| Receita anual | Receita anual |
| Cidade de cobrança | Cidade de cobrança |
| País de cobrança | País de cobrança |
| Código postal/CEP de cobrança | Código postal de cobrança |
| Estado/Província de Faturamento | Estado de cobrança |
| Rua de Faturamento | Endereço de cobrança |
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

## Campos do sistema relacionados ao Salesforce no Marketo (somente leitura) {#salesforce-related-system-fields-in-marketo-read-only}

Esses campos são criados no Marketo, mas não podem ser ajustados por clientes.

| Campo | Descrição |
|---|---|
| SFDC - ID | A ID do Salesforce de 18 caracteres |
| SFDC - Tipo | Líder ou Contato. Se estiver vazio, o lead existe apenas como uma pessoa no Marketo |
| SFDC - Data de criação | Data de criação no SFDC (pode ser diferente de Criado no Marketo) |
| SFDC Excluído | A pessoa estava no SFDC, mas foi excluída e agora vive somente no Marketo |
