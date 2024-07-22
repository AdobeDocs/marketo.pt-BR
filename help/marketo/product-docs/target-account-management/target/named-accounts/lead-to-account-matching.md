---
unique-page-id: 11381156
description: Correspondência de contas de lead - Documentação do Marketo - Documentação do produto
title: Lead para Correspondência de Conta
exl-id: 676ae500-7691-492d-abec-0cac708216b7
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Lead para Correspondência de Conta {#lead-to-account-matching}

Corresponder leads certos a contas nomeadas certas usando a correspondência entre lead e conta da Marketo.

>[!NOTE]
>
>**Correspondência entre lead e conta** é um recurso interno do Gerenciamento de conta do Marketo Target. Ele usa lógica difusa para corresponder leads automaticamente às contas nomeadas certas em tempo quase real. Essas contas nomeadas podem ser contas CRM ou empresas Marketo.

## Visão geral {#overview}

A Vinculação entre lead e conta Marketo segue um processo de quatro etapas:

**Etapa 1 -** Nosso processo de correspondência começa usando as principais informações nos registros de clientes em potencial, como:

* Domínio de email (por exemplo, acme.com)
* Nome da empresa inferido do endereço IP
* Nome da empresa — pode ser o nome da conta do CRM ou o atributo do nome da empresa do cliente potencial (por exemplo, veio do preenchimento do formulário)

**Etapa 2 -** Normalizamos os nomes de empresas encontrados com base em vários atributos de clientes potenciais (por exemplo, Acme Inc. e Acme Corp são normalizados automaticamente para Acme). Essa etapa garante que tenhamos uma única representação da conta nomeada na Marketo e possamos ver todos os leads em uma única conta nomeada.

**Etapa 3 -** Particionamos clientes em potencial correspondentes em dois compartimentos: Correspondência Forte e Correspondência Fraca.

* Clientes potenciais com correspondência fraca aparecem nas contas nomeadas que podem ser resolvidos manualmente.

**Etapa 4 -** Apresentamos uma lista de empresas propostas com correspondência forte e fraca. Quando uma conta nomeada é criada com base em uma das empresas propostas, criamos regras de correspondência para associar automaticamente novos leads (por exemplo, lead preenchido em um formulário) seguindo para as contas nomeadas certas. Dessa forma, você pode se preocupar menos com leads correspondentes e mais com a obtenção de receita!

Como a correspondência entre lead e conta do Marketo é um recurso incorporado do Gerenciamento de conta do Marketo Target, a correspondência de leads com contas ocorre em tempo quase real (por exemplo, no momento em que um lead preenche um formulário do Marketo, associamos esse lead à conta nomeada correta). Esse evento pode ser usado para acionar alertas e notificar os proprietários da conta sobre os novos leads que entram de suas contas nomeadas.

>[!NOTE]
>
>Se você usar LeanData no Salesforce para fazer a correspondência entre lead e conta, a Marketo terá uma integração que sincronizará essas correspondências com a sua instância do Marketo. Para habilitar esse recurso, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support). Saiba como configurar o LeanData abaixo.

## Utilização de LeanData para correspondência entre lead e conta {#using-leandata-for-lead-to-account-matching}

Depois que o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) tiver habilitado o LeanData para sua conta, siga as etapas abaixo para configurá-lo.

1. No Salesforce, clique em **Configurar início** na navegação à esquerda.

1. Ainda na navegação à esquerda, em Administração, clique em **Usuários** e depois em **Perfis**.

1. Localize e selecione o perfil **Marketo Sync**.

1. Role para baixo até a seção Segurança de nível de campo e localize o objeto de cliente potencial. Selecione **Exibir**.

1. Para o nome do campo &quot;Conta com Correspondência do Relatório&quot;, verifique se a caixa de seleção na coluna **Acesso de Leitura** está marcada.

1. No Marketo, vá para a seção **Administrador**.

   ![](assets/lead-to-account-matching-1.png)

1. Selecione **Gerenciamento de campos**.

   ![](assets/lead-to-account-matching-2.png)

1. Confirme se o campo está lá, pesquisando &quot;Reportando conta correspondente&quot;.

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Descobrir Contas](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
