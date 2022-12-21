---
unique-page-id: 11381156
description: Correspondência de conta - Documentos do Marketo - Documentação do produto
title: Lead para a correspondência da conta
exl-id: 676ae500-7691-492d-abec-0cac708216b7
source-git-commit: 98388f1ed941b321449e6e8badac0153dc2245ba
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Lead para a correspondência da conta {#lead-to-account-matching}

O direito de correspondência leva a contas nomeadas corretamente usando a correspondência de lead para conta do Marketo.

>[!NOTE]
>
>**Correspondência de lead para conta** O é um recurso integrado do Gerenciamento de conta do Marketo Target. Ela usa lógica difusa para automaticamente corresponder leads às contas nomeadas certas em tempo quase real. Essas contas nomeadas podem ser contas CRM ou empresas Marketo.

## Visão geral {#overview}

A Correspondência de lead para conta da Marketo segue um processo de quatro etapas:

**Etapa 1 -** Nosso processo correspondente começa usando informações importantes nos registros de lead, como:

* Domínio de email (por exemplo, acme.com)
* Nome da empresa inferido do endereço IP
* Nome da empresa - Pode ser o nome da conta CRM ou o atributo do nome da empresa líder (por exemplo, veio do preenchimento do formulário)

**Etapa 2 -** Normalizamos os nomes de empresas que encontramos com base em vários atributos de lead (por exemplo, Acme Inc. e Acme Corp são automaticamente normalizadas para Acme). Essa etapa garante que tenhamos uma única representação da conta nomeada no Marketo e podemos ver todos os leads em uma única conta nomeada.

**Etapa 3 -** A partição correspondeu os leads em dois compartimentos: Correspondência Forte e Correspondência Fraca.

* Os leads com correspondência fraca são exibidos nas contas nomeadas, que podem ser resolvidas manualmente.

**Etapa 4 -** Apresentamos uma lista de empresas propostas com jogos fortes e fracos. Quando uma conta nomeada é criada com base em uma das empresas propostas, criamos regras de correspondência para associar novos leads automaticamente (por exemplo, formulário de lead preenchido), seguindo para as contas nomeadas certas. Dessa forma, você pode se preocupar menos com a correspondência de leads e muito mais com a obtenção de receita!

Como a correspondência de lead para conta do Marketo é um recurso integrado do Gerenciamento de conta do Marketo Target, a correspondência de leads a contas acontece quase em tempo real (por exemplo, no momento em que um lead preenche um formulário do Marketo, associamos o lead à conta com o nome correto). Esse evento pode ser usado para acionar alertas e notificar os proprietários da conta sobre os novos leads que chegam de suas contas nomeadas.

>[!NOTE]
>
>Se você usar o LeanData no Salesforce para fazer a correspondência de lead para conta, o Marketo tem uma integração que sincronizará essas correspondências com sua instância do Marketo. Para habilitar esse recurso, entre em contato com o [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) Saiba como configurar o LeanData abaixo.

## Usando dados de linha para lead para correspondência da conta {#using-leandata-for-lead-to-account-matching}

Depois [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) tiver ativado o LeanData para sua conta, siga as etapas abaixo para configurá-la.

1. No Salesforce, clique em **Página inicial da configuração** na navegação à esquerda.

1. Ainda na navegação à esquerda, em Administração, clique em **Usuários** then **Perfis**.

1. Localize e selecione o **Marketo Sync** perfil.

1. Role para baixo até a seção Segurança no nível do campo e localize o objeto de lead. Selecionar **Exibir**.

1. Para o nome do campo &quot;Relatório de conta correspondente&quot;, verifique se a caixa de seleção na **Acesso de Leitura** é selecionada.

1. No Marketo, acesse **Administrador** seção.

   ![](assets/lead-to-account-matching-1.png)

1. Selecionar **Gerenciamento de campos**.

   ![](assets/lead-to-account-matching-2.png)

1. Confirme se o campo está lá pesquisando &quot;Relatando Conta Correspondida&quot;.

   ![](assets/lead-to-account-matching-3.png)

>[!MORELIKETHIS]
>
>[Contas do Discover](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md)
