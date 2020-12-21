---
unique-page-id: 11381156
description: Correspondência de contas - Documentos do Marketing - Documentação do produto
title: Correspondência de cliente potencial para conta
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Cliente Potencial para Correspondência de Conta {#lead-to-account-matching}

O direito de correspondência leva a contas com nome certo usando a correspondência entre o cliente potencial e a conta.

>[!NOTE]
>
>**A** Correspondência entre contas é um recurso incorporado do Marketing baseado em conta do Marketing. Ela usa lógica difusa para automaticamente corresponder clientes potenciais às contas nomeadas certas em tempo quase real. Essas contas nomeadas podem ser contas CRM ou empresas de marketing.

A Correspondência de cliente potencial para conta segue um processo de 4 etapas:

**Etapa 1 -** Nosso processo de correspondência começa usando as principais informações nos registros de cliente potencial, como:

* Domínio de email (por exemplo, acme.com)
* Nome da empresa inferido do endereço IP
* Nome da empresa - pode ser o nome da conta CRM ou o atributo do nome da empresa principal (por exemplo, veio do preenchimento do formulário)

**Etapa 2 -** normalizamos os nomes das empresas que encontramos com base em vários atributos de lead (por exemplo, a Acme Inc. e a Acme Corp são normalizadas automaticamente para a Acme). Essa etapa garante que tenhamos uma única representação da conta nomeada no Marketo e que possamos ver todos os clientes potenciais em uma única conta nomeada.

**Etapa 3 -** A partição correspondeu os clientes potenciais em 2 compartimentos: Correspondência forte e Correspondência fraca.

* Os clientes potenciais com correspondência fraca aparecem nas contas nomeadas, que podem ser resolvidos manualmente.

**Etapa 4 -** Apresentamos uma lista de empresas propostas com partidas fortes e fracas. Quando uma conta nomeada é criada com base em uma das empresas propostas, criamos regras de correspondência para associar automaticamente novos clientes potenciais (por exemplo, clientes potenciais preenchidos em um formulário), encaminhando-os para as contas nomeadas certas. Desta forma, você pode se preocupar menos com a correspondência de clientes potenciais e mais com a obtenção de receita!

Como a correspondência entre o cliente em potencial e a conta é um recurso incorporado do Marketing Baseado em Conta do Marketing, a correspondência de clientes em potencial para contas ocorre em tempo quase real (por exemplo, no momento em que um cliente em potencial preenche um formulário do Marketing, associamos o usuário dito lead à conta nomeada correta). Este evento pode ser usado para disparar alertas e notificar os proprietários de conta dos novos clientes potenciais que entram em suas contas nomeadas.

>[!NOTE]
>
>Se você usar o LeanData no Salesforce para fazer a correspondência de cliente potencial para conta, o Marketo terá uma integração que sincronizará essas correspondências com a sua instância do Marketo. Para habilitar esse recurso, entre em contato com o [Suporte de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[Contas do Discover](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md)
