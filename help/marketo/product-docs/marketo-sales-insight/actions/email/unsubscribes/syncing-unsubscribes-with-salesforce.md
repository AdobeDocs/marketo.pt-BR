---
description: Sincronização de cancelamentos de assinatura com o Salesforce - Documentos do Marketo - Documentação do produto
title: Sincronização de cancelamentos de assinatura com o Salesforce
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: 27ca6c3efc5d49729ca4473853688be9cc8cdbc9
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 5%

---

# Sincronização de cancelamentos de assinatura com o Salesforce {#syncing-unsubscribes-with-salesforce}

## Requisitos para cancelamentos de assinatura para sincronização com o Salesforce {#requirements-for-unsubscribes-to-sync-to-salesforce}

* Cancelar assinatura A sincronização deve estar ativada (para sincronização noturna)
* O campo Recusar deve ser instalado no Salesforce
* Os registros de pessoas no Marketo Sales devem ter uma ID do Salesforce

**Enviar cancelamentos de assinaturas**

Quando uma cancelamento de subscrição é coletada no Marketo Sales, a enviamos para o Salesforce em tempo real e atualizamos qualquer um dos campos de recusa selecionados para sincronização. Se você tiver desativado a sincronização do Salesforce, ainda enviaremos o cancelamento de inscrição para o cancelamento de e-mail.

**Cancelar assinatura sincronizada**

Ao ativar a sincronização de cancelamento de inscrição (Etapa 3 abaixo), você estará ativando a sincronização noturna. A sincronização ocorre uma vez por dia, por volta das 20:00 PST. Como alternativa, ela sincronizará todas as assinaturas canceladas no Marketo Sales com o campo Recusar no Salesforce.

## Configurar Unsubscribe Sync para Salesforce {#configure-unsubscribe-sync-to-salesforce}

Os usuários podem decidir se desejam sincronizar seus cancelamentos de assinatura com o campo de Rejeição de email padrão com o qual o Marketo também pode sincronizar ou se podem sincronizar com o campo Rejeição de vendas do Marketo para que os cancelamentos de assinatura de Vendas e cancelamentos de assinatura de Marketing possam ser diferenciados.

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. Em Configurações de administração , selecione **Cancelamentos de assinatura**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. Clique no botão **Integrações** guia . Em Sincronizar com o Salesforce, ative a sincronização noturna.

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. Selecione o campo para o qual deseja sincronizar.

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | Campo | Descrição |
   |---|---|
   | **Sincronizar com o campo de cancelamento de opção do Salesforce** | Selecionado por padrão, o atualiza somente o campo Não participação do Salesforce . |
   | **Sincronizar com o campo de cancelamento do Marketo Sales** | Se quiser separar cancelamentos de vendas e marketing, escolha esta opção para atualizar os [Campo Rejeição de vendas da Marketo.](#msoo) |

## Instalação do campo Recusar no Layout da página {#installing-the-opt-out-field-in-the-page-layout}

**Cancelamento de opção de e-mail**

Recusar email é um campo padrão no Salesforce que está disponível para instalação no Salesforce. Você precisa ser um administrador do Salesforce para instalá-lo.

1. Ir para [Salesforce.com](https://salesforce.com) e faça logon.

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. Clique em seu nome de usuário e selecione **Configuração**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. Na caixa de descoberta rápida, procure Contato ou Lead. Neste cenário, estamos instalando o campo no layout da página Contato, mas você desejará instalar para ambos os registros pessoais.

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. Selecionar **Layouts de página**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. Selecionar **Editar** ao lado do layout da página que você deseja adicionar o campo.

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. Selecionar **Campos**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. Arraste e solte a opção Recusa de email no layout da página.

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. Clique em **Salvar**.

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Cancelamento de inscrição no Marketo Sales Engage {#marketo-sales-opt-out}

O campo Rejeição de vendas do Marketo é um campo personalizado disponível para usuários que instalaram as Personalizações de vendas do Marketo.

Depois de instalar com sucesso as Personalizações de vendas da Marketo no Salesforce, você verá o campo Rejeição de vendas da Marketo disponível para você.
