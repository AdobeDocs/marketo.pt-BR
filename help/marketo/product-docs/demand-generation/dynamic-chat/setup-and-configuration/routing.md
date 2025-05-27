---
description: Roteamento - Documentação do Marketo - Documentação do produto
title: Roteamento
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: 42e2a23c1c451c61fd62237fd1305924b51437b2
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Roteamento {#routing}

As reuniões reservadas no Dynamic Chat podem ser encaminhadas de duas maneiras. Round robin ou usando uma regra personalizada.

Round robin: as reuniões são atribuídas a agentes sequencialmente. Então, se você tiver cinco agentes e o agente três tiver realizado a última reunião, o agente quatro terá a próxima reunião, seguido do agente cinco, e então voltará para o agente um.

Regra personalizada: você pode escolher agentes específicos para receber reuniões com base nos atributos selecionados.

>[!NOTE]
>
>O Roteamento de conta recebe a prioridade mais alta. Quando um visitante atinge o ponto na conversa para marcar uma reunião ou iniciar um chat ao vivo, o [Roteamento de Conta](#account-routing) é verificado primeiro antes que outras opções de roteamento sejam consideradas.

## Criar uma regra personalizada {#create-a-custom-rule}

Neste exemplo, estamos enviando todas as reuniões dos estados inferidos de CA, OR e WA para o agente John.

1. Em Configuração, clique em **Regras de Roteamento**.

   ![](assets/routing-1.png)

1. A guia **Regras personalizadas** é aberta por padrão.

   ![](assets/routing-2.png)

1. Clique em **Criar regra**.

   ![](assets/routing-3.png)

1. Dê um nome à regra. Como opção, você pode adicionar uma descrição e definir seu nível de prioridade. Clique em **Avançar**.

   ![](assets/routing-4.png)

1. Escolha os agentes desejados.

   ![](assets/routing-5.png)

1. Arraste sobre os atributos desejados.

   ![](assets/routing-6.png)

1. Localize e selecione os valores desejados.

   ![](assets/routing-7.png)

1. Quando todos os valores desejados forem selecionados, clique em **Salvar**.

   ![](assets/routing-8.png)

## Roteamento de Conta {#account-routing}

Identifique e faça upload da sua conta de público alvo e respectivos proprietários de vendas e encaminhe os visitantes provenientes dessas contas diretamente para o respectivo proprietário da conta.

![](assets/routing-9.png)

### Adicionar uma conta {#add-an-account}

Neste exemplo, direcionaremos todos os funcionários da Lego diretamente para o agente Steven.

1. Na guia Roteamento de Conta, clique em **+ Adicionar Conta**.

   ![](assets/routing-10.png)

   >[!TIP]
   >
   >É possível criar várias contas de uma só vez, clicando em **Carregar lista de contas** e carregando um CSV.

1. Insira o nome da empresa, o domínio e selecione o agente desejado.

   ![](assets/routing-11.png)
