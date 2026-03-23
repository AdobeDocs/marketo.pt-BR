---
description: Saiba mais sobre o Gerenciamento de agentes no Dynamic Chat. Exibir agentes, gerenciar equipes, definir regras substitutas e controlar como as reuniões e o chat ao vivo são atribuídos.
title: Gerenciamento de agentes
feature: Dynamic Chat
exl-id: 151d8cf2-a5b7-43c4-8418-cc22252108b2
source-git-commit: d762c5a3d644c2c13fd82c55b329af9145ac3125
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 3%

---

# Gerenciamento de agentes {#agent-management}

No Gerenciamento de agentes, visualize uma lista de agentes na instância do Dynamic Chat, gerencie equipes e defina suas regras de fallback.

![](assets/agent-management-1.png)

## Agentes {#agents}

Essa guia lista todos os agentes na instância do Dynamic Chat e inclui informações como nome, endereço de email, status do chat ao vivo e muito mais.

![](assets/agent-management-2.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Não vê um agente que você _acabou_ de adicionar? Pode levar até duas horas para que sejam exibidas aqui após adicioná-las ao Admin Console do Adobe.

## Equipes {#teams}

Os administradores podem criar equipes de agentes para facilitar o roteamento para grupos específicos de agentes de vendas.

>[!AVAILABILITY]
>
>O acesso ao Teams exige uma assinatura do Dynamic Chat Prime. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

![](assets/agent-management-3.png)

### Criar uma equipe {#create-a-team}

1. Clique em **+ Criar Equipe**.

   ![](assets/agent-management-4.png)

1. Nomeie sua equipe.

   ![](assets/agent-management-5.png)

1. Clique na lista suspensa **Adicionar agentes** e selecione os agentes desejados.

   ![](assets/agent-management-6.png)

1. Clique em **Criar**.

   ![](assets/agent-management-7.png)

## Regras de Fallback {#fallback-rules}

### Fallback de Reunião {#meeting-fallback}

Selecione uma mensagem padrão (sistema) ou escreva uma personalizada para os visitantes verem quando a reserva da reunião não estiver disponível.

![](assets/agent-management-8.png)

### Fallback de bate-papo ao vivo {#live-chat-fallback}

Selecione uma mensagem padrão (sistema) ou escreva uma personalizada para os visitantes verem quando o bate-papo ao vivo estiver indisponível.

![](assets/agent-management-9.png)

>[!NOTE]
>
>* Marcar a caixa de seleção _Incluir Opção de Reserva de Reunião_ dará ao visitante do chat a opção de marcar uma reunião quando nenhum agente estiver disponível para o chat ao vivo.
>
>* **Para quaisquer regras/Equipes personalizadas como um cartão de Chat ao Vivo**: ao verificar agentes, se eles não estiverem disponíveis ou não puderem se conectar, recorrerá ao Round Robin para tentar &quot;Agentes Disponíveis&quot; (todos os que estiverem disponíveis naquele momento, independentemente de qual lógica/regra de roteamento foi colocada no fluxo).

>[!TIP]
>
>Ao criar uma mensagem personalizada, você pode estilizar a fonte, usar links e até mesmo inserir emojis! `:)`

## Configurações {#settings}

### Limite de chats ao vivo simultâneos {#concurrent-live-chat}

Defina o número de bate-papos ativos simultâneos que um agente pode realizar de uma vez. Pode definir entre 1 e 10.

![](assets/agent-management-10.png)

### Limite de tempo de espera do visitante {#visitor-wait-time}

Controle a quantidade máxima de tempo que um visitante aguardará (em segundos) para ser conectado a um agente ativo antes que o visitante receba uma mensagem de fallback. Pode ser definido entre 10 e 500 segundos.

![](assets/agent-management-11.png)
