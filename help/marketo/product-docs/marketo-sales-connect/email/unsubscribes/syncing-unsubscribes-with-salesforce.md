---
unique-page-id: 14746188
description: Sincronização de cancelamentos de assinatura com o Salesforce - Documentação do Marketo - Documentação do produto
title: Sincronização de cancelamentos de assinatura com o Salesforce
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 1%

---

# Sincronizando Cancelamentos de Assinatura com [!DNL Salesforce] {#syncing-unsubscribes-with-salesforce}

## Requisitos para cancelamentos de assinatura para sincronização com [!DNL Salesforce] {#requirements-for-unsubscribes-to-sync-to-salesforce}

* A sincronização de cancelamento de inscrição deve estar habilitada (para sincronização noturna)
* O campo Recusar deve estar instalado em [!DNL Salesforce]
* Os registros de pessoa em [!DNL Sales Connect] devem ter uma ID de [!DNL Salesforce]

**Cancelamentos de Assinatura por Push**

Quando um cancelamento de inscrição é coletado em [!DNL Sales Connect], nós o enviamos para [!DNL Salesforce] em tempo real e atualizamos qualquer um dos campos de opção de não participação que você selecionou para sincronização. Se você desabilitou a sincronização [!DNL Salesforce], ainda enviaremos o cancelamento de inscrição para a opção de email.

**Cancelar Assinatura da Sincronização**

Após habilitar a sincronização de cancelamento de inscrição (Etapa 3 abaixo), você ativará a sincronização noturna. A sincronização ocorre uma vez por dia, por volta das 20h00 PST. :00 Ele sincronizará bidirecionalmente todas as cancelamentos de subscrições no Marketo Sales com o campo Opt Out no Salesforce.

## Configurar Cancelar Assinatura da Sincronização para [!DNL Salesforce] {#configure-unsubscribe-sync-to-salesforce}

Os usuários podem decidir se desejam sincronizar seus cancelamentos de assinatura com o campo Email Opt Out padrão, com o qual o Marketo também pode sincronizar, ou podem sincronizar com o campo Marketo Sales Opt Out para que os cancelamentos de assinatura de vendas e de marketing possam ser diferenciados.

1. Vá para o [aplicativo Web](https://toutapp.com/login), clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/one-1.png)

1. Em [!UICONTROL Configurações de Administração], selecione **[!UICONTROL Cancelar Assinaturas]**.

   ![](assets/two-2.png)

1. Clique em **[!UICONTROL Sincronizando com o Salesforce]** e habilite a sincronização noturna.

   ![](assets/three-2.png)

1. Selecione o campo que você deseja sincronizar.

   ![](assets/4.png)

   | Campo | Descrição |
   |---|---|
   | **[!UICONTROL Sincronizar com o campo Recusa do Salesforce]** | Selecionado por padrão, atualiza somente o campo [!DNL Salesforce] Recusa. |
   | **[!UICONTROL Sincronizar com o campo Recusa do Marketo Sales]** | Se quiser separar cancelamentos de assinatura de Vendas e Marketing, escolha esta opção para atualizar o campo [Recusa/aceitação de vendas do Marketo.](#msoo) |

## Instalação do campo Recusa no layout da página {#installing-the-opt-out-field-in-the-page-layout}

**Opção de não participação de email**

A Recusa de Email é um campo padrão no [!DNL Salesforce] que está disponível para instalação a partir do [!DNL Salesforce]. Você precisa ser um Administrador [!DNL Salesforce] para instalá-lo.

1. Acesse [Salesforce.com](https://salesforce.com) e entre.

   ![](assets/five-1.png)

1. Clique no seu nome de usuário e selecione **[!UICONTROL Instalação]**.

   ![](assets/six-1.png)

1. Na caixa de localização rápida, procure por Contato ou Cliente Potencial. Neste cenário, estamos instalando o campo no layout da página Contato, mas convém instalar para ambos os registros de pessoa.

   ![](assets/seven-1.png)

1. Selecione **[!UICONTROL Layouts de Página]**.

   ![](assets/eight-1.png)

1. Selecione **[!UICONTROL Editar]** ao lado do layout de página ao qual você deseja adicionar o campo.

   ![](assets/nine.png)

1. Selecione **[!UICONTROL Campos]**.

   ![](assets/ten.png)

1. Arraste e solte a [!UICONTROL Recusa de email] no layout da página.

   ![](assets/11.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/twelve.png)

## Desativação de Marketo Sales {#marketo-sales-opt-out}

O campo Recusa de vendas do Marketo é um campo personalizado disponível para usuários que instalaram as Personalizações do Marketo [!DNL Sales Connect].

Depois de instalar com êxito as Personalizações do Marketo [!DNL Sales Connect] em [!DNL Salesforce], você verá o campo Opção de vendas da Marketo disponível para você.
