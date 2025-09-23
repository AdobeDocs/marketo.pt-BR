---
unique-page-id: 2953415
description: Uso da página de detalhes da pessoa - Documentação do Marketo - Documentação do produto
title: Uso da página Detalhes da pessoa
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 35%

---

# Uso da página Detalhes da pessoa {#using-the-person-detail-page}

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

| Tabulação | Descrição |
|---|---|
| Info | Informações de contato e campos personalizados sobre uma pessoa. |
| Informações da empresa | Informações e endereço da empresa da pessoa. |
| Informações da oportunidades | Informações da oportunidade sincronizadas do Salesforce. |
| SFDC - Campo do lead | Campos integrados do Salesforce. |
| Campo personalizado do SFDC | Campos personalizados do Salesforce. |
| Registro de atividades | Todas as atividades relacionadas à pessoa. |

## Organização da página - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| Tabulação | Descrição |
|---|---|
| Info | Informações de contato e campos personalizados sobre uma pessoa. |
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
| Motivo para não ligar | Motivo para não ligar | Endereço de e-mail | Email inválido | Motivo do e-mail inválido |
| ID da empresa externa | ID da pessoa de vendas da empresa externa | Número de fax | Nome | Nome completo |
| Setor | Cidade indicada | Empresa indicada | País indicado | Área metropolitana indicada |
| Código de área telef. indic. | Código postal indicado | Estado/região indicado | É anônimo | É cliente |
| É parceiro | Nome do cargo | Sobrenome | Classificação | Pontuação |
| Fonte de pessoas | Status | Telefone principal | Nome para Exibição do Marketo Social [!DNL Facebook] | Marketo Social [!DNL Facebook] Id |
| URL da foto [!DNL Facebook] do Marketo Social | URL do perfil [!DNL Facebook] do Marketo Social | Alcance do Marketo Social [!DNL Facebook] | Inscrições Referenciadas do Marketo Social [!DNL Facebook] | Visitas referenciadas [!DNL Facebook] do Marketo Social |
| Marketo - Sexo em perfil social | Marketo - Última inscrição por indicação em perfil social | Marketo - Última visita por indicação em perfil social | Nome para Exibição do Marketo Social [!DNL LinkedIn] | Marketo Social [!DNL LinkedIn] Id |
| URL da foto [!DNL LinkedIn] do Marketo Social | URL do perfil [!DNL LinkedIn] do Marketo Social | Alcance do Marketo Social [!DNL LinkedIn] | Inscrições Referenciadas do Marketo Social [!DNL LinkedIn] | Visitas referenciadas [!DNL LinkedIn] do Marketo Social |
| Marketo - ID de distribuição social | Marketo - Total de inscrições por indicação em perfil social | Marketo - Total de visitas por indicação em perfil social | Nome para Exibição do Marketo Social [!DNL Twitter] | Marketo Social [!DNL Twitter] Id |
| URL da foto [!DNL Twitter] do Marketo Social | URL do perfil [!DNL Twitter] do Marketo Social | Alcance do Marketo Social [!DNL Twitter] | Inscrições Referenciadas do Marketo Social [!DNL Twitter] | Visitas referenciadas [!DNL Twitter] do Marketo Social |
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
>* Oportunidades para contatos da SFDC
>* Determinados campos específicos do Marketo, como Data de criação e Tipo de Source original.
>
>Saiba mais sobre [Campos Gerenciados pelo Sistema](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}.

>[!MORELIKETHIS]
>
>[Criando uma Guia Personalizada para a Página de Detalhes da Pessoa](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
