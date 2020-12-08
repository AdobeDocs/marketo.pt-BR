---
unique-page-id: 14352477
description: Push to Sales Connect - Documentos do Marketing - Documentação do produto
title: Encaminhar para o Connect de Vendas
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Encaminhar para o Connect de Vendas {#push-to-sales-connect}

Nosso botão Enviar para o Tout tirará uma lista de seus clientes potenciais/contatos no Salesforce e os encaminhará para um grupo no Sales Connect. Você pode enviar rapidamente um email de grupo personalizável com o rastreamento de Tout anexado.

## Requisitos {#requirements}

* Pacote do Sales Connect [Salesforce](http://docs.marketo.com/x/C4PS) instalado por `Salesforce Admin`

* `Push to Sales Connect`botão instalado na lista da visualização por `Salesforce Admin`

* Conexão Salesforce feita com o Sales Connect para usuário que faz o push

## Como {#how-to}

1. Clique na guia **Lead/Contact** no Salesforce.
1. Alterne para a Visualização da Lista que você deseja encaminhar para o Sales Connect ao lado do botão Ir.
1. Clique em **Ir**.
1. Selecione todos os clientes potenciais/contatos que você deseja que sejam forçados a participar.
1. Selecione **Enviar para MSE**.
1. Será exibida uma nova janela verificando o número de clientes potenciais/contatos que você gostaria de passar. Selecione **Prosseguir para grupo**. Vendas Connect `will not push over` todos os contatos marcados como `Email Opt Out` no Salesforce ou `Unsubscribed` no Sales Connect.

   >[!NOTE]
   >
   >O Sales Connect adicionará este grupo intitulado &quot;SFDC-...&quot; para a página Relacionamentos no aplicativo [da](http://toutapp.com/login)Web.

1. Selecione **Enviar email para todo o grupo** para enviar este email de grupo.

