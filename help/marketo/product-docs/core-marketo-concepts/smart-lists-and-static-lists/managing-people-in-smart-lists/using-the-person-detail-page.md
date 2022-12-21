---
unique-page-id: 2953415
description: Usar a página de detalhes da pessoa - Documentos do Marketo - Documentação do produto
title: Usando a Página de detalhes da pessoa
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 49%

---

# Usando a Página de detalhes da pessoa {#using-the-person-detail-page}

A página de detalhes da pessoa contém todas as informações que a Marketo conhece sobre uma pessoa. Você pode editar dados diretamente desta página.

## Página de detalhes da pessoa {#getting-to-person-detail-page}

Há muitas maneiras de abrir pessoas específicas. Alguns exemplos:

* No **Banco de dados**, você pode pesquisar na Localização rápida
* Qualquer inteligente **lista** ou lista
* **Membros** guia de um programa
* **Exibir membros da campanha** em uma Campanha inteligente
* Algumas **relatórios**

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
| Informações da oportunidades | Informações de oportunidade sincronizadas do Salesforce. |
| SFDC - Campo do lead | Campos incorporados do Salesforce. |
| Campo Personalizado SFDC | Campos personalizados do Salesforce. |
| Registro de atividades | Todas as atividades relacionadas à pessoa. |

## Organização de página - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tabulação | Descrição |
|---|---|
| Informações | Informações de contato e campos personalizados sobre uma pessoa. |
| Informações da empresa | Informações e endereço da empresa da pessoa. |
| Informações da oportunidades | Informações da oportunidade sincronizadas do Microsoft. |
| Campos personalizados da Microsoft | Campos Microsoft personalizados. |
| Campo de leads da Microsoft | Campos integrados do Microsoft. |
| Registro de atividades | Todas as atividades relacionadas à pessoa. |

>[!NOTE]
>
>Você também pode ver informações da Oportunidade [inserido via API](https://developers.marketo.com/rest-api/lead-database/opportunities/) para instâncias que não estão sincronizadas com um CRM.

## Editar um campo {#editing-a-field}

Muitos campos são editáveis. Para atualizar as informações de uma pessoa, digite um novo valor e clique fora do campo para salvar.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campos padrão do Marketo anteriores à sincronização do CRM {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| Endereço | Receita anual | IP anônimo | Endereço de cobrança | Cidade de cobrança |
| País de cobrança | Código postal de cobrança | Estado de cobrança | Cidade | Nome da empresa |
| País | Criado em | Data de nascimento | Departamento | Não ligar |
| Motivo para não ligar | Motivo para não ligar | Endereço de e-mail | E-mail inválido | Motivo do e-mail inválido |
| ID da empresa externa | ID da pessoa de vendas da empresa externa | Número de fax | Nome | Nome completo |
| Setor | Cidade indicada | Empresa indicada | País indicado | Área metropolitana indicada |
| Código de área telef. indic. | Código postal indicado | Estado/região indicado | É anônimo | É cliente |
| É parceiro | Nome do cargo | Sobrenome | Classificação | Pontuação |
| Fonte de pessoas | Status | Telefone principal | Marketo - Nome de exibição no perfil social do Facebook | ID social do Marketo no Facebook |
| Marketo - URL da foto no perfil social do Facebook | Marketo - URL do perfil social do Facebook | Marketo - Alcance do perfil social do Facebook | Marketo - Inscrições por indicação no perfil social do Facebook | Marketo - Visitas por indicação no perfil social do Facebook |
| Marketo - Sexo em perfil social | Marketo - Última inscrição por indicação em perfil social | Marketo - Última visita por indicação em perfil social | Marketo - Nome de exibição no perfil social do LinkedIn | ID social do Marketo no LinkedIn |
| Marketo - URL da foto no perfil social do LinkedIn | Marketo - URL do perfil social do LinkedIn | Marketo - Alcance do perfil social do LinkedIn | Marketo - Inscrições por indicação no perfil social do LinkedIn | Marketo - Visitas por indicação no perfil social do LinkedIn |
| Marketo - ID de distribuição social | Marketo - Total de inscrições por indicação em perfil social | Marketo - Total de visitas por indicação em perfil social | Marketo - Nome de exibição no perfil social do Twitter | ID social do Marketo no Twitter |
| Marketo - URL da foto no perfil social do Twitter | Marketo - URL do perfil social do Twitter | Marketo - Alcance do perfil social do Twitter | Marketo - Inscrições por indicação no perfil social do Twitter | Marketo - Visitas por indicação no perfil social do Twitter |
| Segundo nome | Número do celular | Núm. funcionários | Número de telefone | Código postal |
| Prioridade | Pontuação relativa | Função | Saudação | Código SIC |
| Site | Estado | Inscrição cancelada | Motivo do cancelamento de inscr. | Atualizado em |
| Urgência | Site |  |  |  |

>[!NOTE]
>
>Alguns campos são _not_ editável:
>
>* Registro de atividades
>* Informações da empresa
>* Oportunidades para os contatos da SFDC
>* Determinados campos específicos do Marketo, como Data de criação e Tipo de origem original.
>
>Saiba mais sobre [Campos gerenciados pelo sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md).

>[!MORELIKETHIS]
>
>[Criação de uma guia personalizada para a página de detalhes da pessoa](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
