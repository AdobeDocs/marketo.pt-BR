---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Documentação do produto
title: Push para Conexão de Vendas
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Push para Conexão de Vendas {#push-to-sales-connect}

Nosso botão &quot;Push to Tout&quot; selecionará uma lista de clientes potenciais/contatos no Salesforce e os colocará em um grupo no Sales Connect. Você pode enviar rapidamente um email de grupo personalizável com rastreamento Tout anexado.

## Requisitos {#requirements}

* Pacote do Sales Connect Salesforce instalado pelo administrador do Salesforce

* Botão Enviar para o Sales Connect instalado para exibição de lista pelo administrador do Salesforce

* Conexão do Salesforce feita com o Sales Connect para o usuário que está fazendo o push

## Como {#how-to}

1. Clique na guia **Lead/Contato** no Salesforce.
1. Alternar para a Exibição de Lista que você deseja enviar para o Sales Connect ao lado do botão Ir.
1. Clique em **Ir**.
1. Selecione todos os clientes em potencial/contatos que você deseja enviar para o tout.
1. Selecione **Enviar para o MSE**.
1. Uma nova janela será exibida verificando o número de leads/contatos que você gostaria de enviar. Selecione **Prosseguir para o Grupo**. O Sales Connect não transferirá nenhum contato marcado como Recusa de email no Salesforce ou Cancelamento de assinatura no Sales Connect.

   >[!NOTE]
   >
   >O Sales Connect adicionará este grupo denominado &quot;SFDC-...&quot; à página Relações no [aplicativo Web](https://toutapp.com/login).

1. Selecione **Enviar Email para o Grupo Inteiro** para enviar este email de grupo.
