---
unique-page-id: 2953415
description: Usar a página de detalhes da pessoa - Documentos do Marketo - Documentação do produto
title: Usando a Página de detalhes da pessoa
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---


# Usando a Página de Detalhes da Pessoa {#using-the-person-detail-page}

A página de detalhes da pessoa contém todas as informações que o Marketo conhece sobre uma pessoa. Você pode editar dados diretamente desta página.

## Página de Detalhes da Pessoa {#getting-to-person-detail-page}

Há muitas maneiras de abrir pessoas específicas. Alguns exemplos:

* No **Banco de Dados**, você pode pesquisar no Localização Rápida
* Qualquer **lista** ou lista inteligente
* **** Membros de um programa
* **Exibir** membros da campanha em uma campanha inteligente
* Alguns **relatórios**

   <br> 

1. Clique duas vezes em qualquer pessoa ou clique uma vez na ID à esquerda.

   ![](assets/one-1.png)

1. Isso abrirá a tela de detalhes da pessoa.

   ![](assets/two-5.png)

## Organização de página - Salesforce {#page-organization-salesforce}

As informações de pessoa são categorizadas nas seguintes guias:

| Tabulação | Descrição |
|---|---|
| Informações | Informações de contato e campos personalizados sobre uma pessoa. |
| Informações da empresa | Informações e endereço da empresa da pessoa. |
| Informações da Oportunidade | Informações de oportunidade sincronizadas do Salesforce. |
| Campo de lead SFDC | Campos incorporados do Salesforce. |
| Campo Personalizado SFDC | Campos personalizados do Salesforce. |
| Log de atividades | Todas as atividades relacionadas à pessoa. |

## Organização de página - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tabulação | Descrição |
|---|---|
| Informações | Informações de contato e campos personalizados sobre uma pessoa. |
| Informações da empresa | Informações e endereço da empresa da pessoa. |
| Informações da Oportunidade | Informações da oportunidade sincronizadas da Microsoft. |
| Campos personalizados da Microsoft | Campos personalizados da Microsoft. |
| Campo de lead da Microsoft | Campos integrados da Microsoft. |
| Log de atividades | Todas as atividades relacionadas à pessoa. |

>[!NOTE]
>
>Você também pode ver as informações da Oportunidade [inseridas via API](http://developers.marketo.com/rest-api/lead-database/opportunities/) para instâncias que não estão sincronizadas com um CRM.

## Editar um campo {#editing-a-field}

Muitos campos são editáveis. Para atualizar as informações de uma pessoa, digite um novo valor e clique fora do campo para salvar.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campos padrão do Marketo antes da sincronização do CRM {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Endereço | Receita anual | IP Anônimo | Endereço de cobrança | Cidade de Faturamento |
| País de Faturamento | Código postal de cobrança | Estado de Faturamento | Cidade | Nome da empresa |
| País | Criado em | Data de nascimento | Departamento | Não Chame |
| Não Chamar Causa | Não Chamar Motivo | Endereço de email | Email Inválido | Causa Inválida do Email |
| Id Da Empresa Externa | Id Da Pessoa De Vendas Externa | Número de fax | Nome | Nome completo |
| Setor | Cidade Inferida | Empresa Inferior | País Inferior | Área Metropolitana Inferida |
| Código da Área do Telefone Inferior | Código postal Inferior | Região do Estado Inferior | Is Anonymous | É cliente |
| É Parceiro | Cargo | Sobrenome | Classificação | Pontuação |
| Origem da Pessoa | Status | Telefone principal | Nome de exibição do Facebook do Marketo Social | ID do Facebook do Marketo Social |
| URL de foto do Facebook do Marketo Social | URL de perfil do Facebook do Marketo Social | Alcance do Facebook do Marketo Social | Inscrições Referenciadas do Marketo Social no Facebook | Marketo Social Facebook Referenciou visitas |
| Marketo Social Gender | Última Inscrição do Marketo Social Referenciada | Última visita referenciada do Marketo Social | Nome de exibição do Marketo Social LinkedIn | Id Do LinkedIn Do Marketo Social |
| URL de foto do Marketo Social LinkedIn | URL de perfil do Marketo Social LinkedIn | Alcance do LinkedIn do Marketo Social | Inscrições Referenciadas do Marketo Social LinkedIn | Visitas referenciadas do Marketo Social LinkedIn |
| ID de sindicalização do Marketo Social | Total de inscrições referenciadas do Marketo Social | Total de visitas referenciadas do Marketo Social | Nome de exibição do Twitter do Marketo Social | Id Do Twitter Do Marketo Social |
| URL de foto do Twitter do Marketo Social | URL de perfil do Twitter do Marketo Social | Alcance do Twitter do Marketo Social | Matrícula referenciada do Marketo Social Twitter | Visitas referenciadas do Twitter do Marketo Social |
| Nome do meio | Número de telefone celular | Número de funcionários | Número de telefone | Código postal |
| Prioridade | Pontuação relativa | Função | Saudação | Código SIC |
| Site | Estado | Inscrições canceladas | Motivo da assinatura cancelada | Atualizado em |
| Urgência | Site |  |  |  |

>[!NOTE]
>
>Alguns campos são _não_ editáveis:
>
>* Log de atividades
>* Informações da empresa
>* Oportunidades para os contatos da SFDC
>* Determinados campos específicos do Marketo, como Data de criação e Tipo de origem original.

>
>
Saiba mais sobre [Campos gerenciados pelo sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Criação de uma guia personalizada para a página de detalhes da pessoa](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
