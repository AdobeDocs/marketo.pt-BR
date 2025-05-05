---
unique-page-id: 2953415
description: Uso da página de detalhes da pessoa - Documentação do Marketo - Documentação do produto
title: Usando a Página Detalhes da Pessoa
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 50%

---

# Usando a Página Detalhes da Pessoa {#using-the-person-detail-page}

A página de detalhes da pessoa contém todas as informações que o Marketo sabe sobre uma pessoa. É possível editar dados diretamente nesta página.

## Página de Detalhes da Pessoa {#getting-to-person-detail-page}

Há muitas maneiras de abrir pessoas específicas. Alguns exemplos são:

* No **Banco de Dados**, você pode pesquisar na Localização Rápida
* Qualquer **lista inteligente** ou lista
* Guia **Membros** de um programa
* **Exibir membros da campanha** em uma campanha inteligente
* Alguns **relatórios**
  <br> 

1. Clique duas vezes em qualquer pessoa ou clique uma vez na ID à esquerda.

   ![](assets/one-1.png)

1. Isso abrirá a tela de detalhes da pessoa.

   ![](assets/two-5.png)

## Organização da página - Salesforce {#page-organization-salesforce}

As informações de pessoa são categorizadas nas seguintes guias:

| Guia | Descrição |
|---|---|
| Informações | Informações de contato e campos personalizados sobre uma pessoa. |
| Informações da empresa | Informações e endereço da empresa da pessoa. |
| Informações da oportunidades | Informações da oportunidade sincronizadas do Salesforce. |
| SFDC - Campo do lead | Campos Salesforce integrados. |
| Campo personalizado SFDC | Campos personalizados do Salesforce. |
| Registro de atividades | Todas as atividades relacionadas à pessoa. |

## Organização da página - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Guia | Descrição |
|---|---|
| Informações | Informações de contato e campos personalizados sobre uma pessoa. |
| Informações da empresa | Informações e endereço da empresa da pessoa. |
| Informações da oportunidades | Informações da oportunidade sincronizadas do Microsoft. |
| Campos personalizados da Microsoft | Campos personalizados do Microsoft. |
| Campo de leads da Microsoft | Campos integrados do Microsoft. |
| Registro de atividades | Todas as atividades relacionadas à pessoa. |

>[!NOTE]
>
>Você também pode ver informações de oportunidade [inseridas via API](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/opportunities) para instâncias que não estão sincronizadas com um CRM.

## Edição de um campo {#editing-a-field}

Muitos campos são editáveis. Para atualizar as informações de uma pessoa, digite um novo valor e clique fora do campo para salvar.

![](assets/image2015-2-27-11-3a14-3a2.png)

## Campos Padrão do Marketo Antes da Sincronização com o CRM {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
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
| Nome do meio | Número do celular | Núm. funcionários | Número de telefone | Código postal |
| Prioridade | Pontuação relativa | Função | Saudação | Código SIC |
| Site | Estado | Inscrição cancelada | Motivo do cancelamento de inscr. | Atualizado em |
| Urgência | Site |  |  |  |

>[!NOTE]
>
>Alguns campos _não_ são editáveis:
>
>* Registro de atividades
>* Informações da Empresa
>* Oportunidades para Contatos SFDC
>* Determinados campos específicos do Marketo, como Data de criação e Tipo de Source original.
>
>Saiba mais sobre [Campos Gerenciados pelo Sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Criando uma Guia Personalizada para a Página de Detalhes da Pessoa](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
