---
unique-page-id: 14746188
description: Sincronização de cancelamentos de assinatura com o Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronização de cancelamentos de assinatura com o Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---

# Sincronização de cancelamentos de assinatura com o Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisitos para cancelamentos de assinatura para sincronização com o Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* A sincronização de cancelamento de inscrição deve estar habilitada (para sincronização noturna)
* O campo Recusar deve estar instalado no Salesforce
* Os registros de pessoa no Sales Connect devem ter uma ID do Salesforce

**Cancelamentos de Assinatura por Push**

Quando um cancelamento de inscrição é coletado no Sales Connect, ele é enviado ao Salesforce em tempo real e atualizamos qualquer um dos campos de opção de não participação que você selecionou para sincronização. Se você desativou a sincronização do Salesforce, ainda enviaremos o cancelamento de inscrição para a opção de não participação de email.

**Cancelar Assinatura da Sincronização**

Após habilitar a sincronização de cancelamento de inscrição (Etapa 3 abaixo), você ativará a sincronização noturna. A sincronização ocorre uma vez por dia, por volta das 20h PST. Ele sincronizará bidirecionalmente todas as cancelamentos de subscrições no Marketo Sales com o campo Recusa no Salesforce.

## Configurar cancelar inscrição da sincronização com o Salesforce {#configure-unsubscribe-sync-to-salesforce}

Os usuários podem decidir se desejam sincronizar seus cancelamentos de assinatura com o campo Email Opt Out padrão, com o qual o Marketo também pode sincronizar, ou podem sincronizar com o campo Marketo Sales Opt Out para que os cancelamentos de assinatura de vendas e de marketing possam ser diferenciados.

1. Vá para o [aplicativo Web](https://toutapp.com/login), clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one-1.png)

1. Em Configurações do administrador, selecione **Cancelar assinatura**.

   ![](assets/two-2.png)

1. Clique em **Sincronizando com o Salesforce** e habilite a sincronização noturna.

   ![](assets/three-2.png)

1. Selecione o campo que você deseja sincronizar.

   ![](assets/4.png)

   | Campo | Descrição |
   |---|---|
   | **Sincronizar com o campo Recusa do Salesforce** | Selecionado por padrão, atualiza somente o campo Recusa do Salesforce. |
   | **Sincronizar com o campo Recusa do Marketo Sales** | Se quiser separar cancelamentos de assinatura de Vendas e Marketing, escolha esta opção para atualizar o campo [Recusa/aceitação de vendas do Marketo.](#msoo) |

## Instalação do campo Recusa no layout da página {#installing-the-opt-out-field-in-the-page-layout}

**Opção de não participação de email**

Recusa de email é um campo padrão no Salesforce que está disponível para instalação no Salesforce. Você precisa ser um administrador do Salesforce para instalá-lo.

1. Acesse o [Salesforce.com](https://salesforce.com) e faça logon.

   ![](assets/five-1.png)

1. Clique no seu nome de usuário e selecione **Instalação**.

   ![](assets/six-1.png)

1. Na caixa de localização rápida, procure por Contato ou Cliente Potencial. Neste cenário, estamos instalando o campo no layout da página Contato, mas convém instalar para ambos os registros de pessoa.

   ![](assets/seven-1.png)

1. Selecione **Layouts de Página**.

   ![](assets/eight-1.png)

1. Selecione **Editar** ao lado do layout de página ao qual você deseja adicionar o campo.

   ![](assets/nine.png)

1. Selecione **Campos**.

   ![](assets/ten.png)

1. Arraste e solte Recusa de email no layout da página.

   ![](assets/11.png)

1. Clique em **Salvar**.

   ![](assets/twelve.png)

## Desativação de Marketo Sales {#marketo-sales-opt-out}

O campo Recusa de vendas do Marketo é um campo personalizado disponível para usuários que instalaram as Personalizações do Marketo Sales Connect.

Depois de instalar com êxito as Personalizações do Marketo Sales Connect no Salesforce, você verá o campo Recusa do Marketo Sales disponível para você.
