---
unique-page-id: 14352477
description: Encaminhar para Conexão de Vendas - Documentação da Marketo - Documentação do produto
title: Enviar por push ao Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 4%

---

# Enviar por push ao Sales Connect {#push-to-sales-connect}

Nosso botão Encaminhar para o Tout pegará uma lista de seus leads/contatos no Salesforce e os encaminhará a um grupo no Sales Connect. Em seguida, você pode enviar rapidamente um email de grupo personalizável com o rastreamento de Tout anexado.

## Requisitos {#requirements}

* Pacote Sales Connect Salesforce instalado pelo Salesforce Admin

* Botão Encaminhar para Conexão de Vendas instalado para exibição em lista pelo Administrador do Salesforce

* Conexão Salesforce feita com o Sales Connect para o usuário que faz o push

## Como {#how-to}

1. Clique no botão **Cliente Potencial/Contato** no Salesforce.
1. Alterne para a Exibição de lista que você gostaria de enviar para Conexão de vendas ao lado do botão Ir.
1. Clique em **Ir**.
1. Selecione todos os leads/contatos que você deseja enviar para o tout.
1. Selecionar **Encaminhar para MSE**.
1. Será exibida uma nova janela verificando o número de leads/contatos que você gostaria de passar por cima. Selecionar **Prosseguir para o grupo**. A Conexão de Vendas não carregará nenhum contato marcado como Recusa de Email no Salesforce ou Cancelada a Assinatura no Conexão de Vendas.

   >[!NOTE]
   >
   >O Sales Connect adicionará esse grupo chamado &quot;SFDC-..&quot; à página Relacionamentos na [aplicação web](https://toutapp.com/login).

1. Selecionar **Email - Grupo inteiro** para enviar este email de grupo.
