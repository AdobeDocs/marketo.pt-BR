---
description: Roteamento - Documentação do Marketo - Documentação do produto
title: Roteamento
feature: Dynamic Chat
exl-id: e20193b9-55c1-40f2-9e42-5b5dc9b88144
source-git-commit: 19f7a38a6a87bc66084e7e45f5bf49cd0d29c3cd
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 2%

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

>[!PREREQUISITES]
>
>Antes que o _Roteamento de Conta_ esteja visível no Dynamic Chat, as permissões devem ser habilitadas no Admin Console. Consulte [Habilitar permissões](#enable-permissions) abaixo.

### Ativar permissões {#enable-permissions}

+++ Habilitar Permissões de Roteamento de Conta

1. Faça logon em [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/){target="_blank"}.

1. Em _Produtos_, selecione **Dynamic Chat**.

   ![](assets/routing-10.png)

1. Em _Perfis de produto_, selecione o perfil desejado.

   ![](assets/routing-11.png)

1. Clique na guia **Permissões**.

   ![](assets/routing-12.png)

1. Clique no ícone de edição (![Ícone de edição](assets/icon-routing-edit.png)) ao lado de _Configuração_.

   ![](assets/routing-13.png)

1. Clique no sinal **+** ao lado de _Exibir roteamento de conta_.

   ![](assets/routing-14.png){width="600" zoomable="yes"}

1. Clique em **Salvar** quando terminar.

+++

### Adicionar uma conta {#add-an-account}

Neste exemplo, direcionaremos todos os funcionários da Lego diretamente para o agente Steven.

1. Na guia Roteamento de Conta, clique em **+ Adicionar Conta**.

   ![](assets/routing-15.png)

   >[!TIP]
   >
   >É possível criar várias contas de uma só vez, clicando em **Carregar lista de contas** e carregando um CSV.

1. Insira o nome da empresa, o domínio e selecione o agente desejado.

   ![](assets/routing-16.png)
