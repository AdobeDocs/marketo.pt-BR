---
description: Saiba como configurar a segurança do Dynamic Chat com domínios bloqueados ou permitidos. Restrinja quais domínios de email os agentes veem e quais sites podem usar seu script de bate-papo.
title: Configurações de segurança
feature: Dynamic Chat
exl-id: 68a53986-6f42-4aa2-86f6-0b2097f94963
TQID: https://experienceleague.adobe.com/7ans6J5WCXbTalK7ubMCrWBLWaJm3prPCoxsrCWEKtg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 88949407423d12a95bf39470e3c29835d934e2f6
workflow-type: tm+mt
source-wordcount: 238
ht-degree: 3%

---

# Configurações de segurança {#security-settings}

Nas configurações de segurança, você pode adicionar domínios a uma lista de permissões ou bloqueada.

![](assets/security-settings-1.png)

>[!IMPORTANT]
>
>A filtragem Bloquear e Permitir domínio de email se aplica somente quando um visitante insere seu endereço de email diretamente no Dynamic Chat, no chatbot ou em um fluxo de conversação. Isso não se aplica a endereços de email que a Dynamic Chat recebe de produtos integrados, como o Marketo Engage. Para obter mais informações, consulte a tabela abaixo.

| Cenário | A filtragem se aplica? |
|---|---|
| O visitante digita seu email diretamente no chatbot do Dynamic Chat | Sim |
| O visitante digita seu email diretamente em um fluxo de conversação do Dynamic Chat | Sim |
| O email é pré-preenchido a partir do envio de um formulário do Marketo (o fluxo de conversação é exibido após o preenchimento do formulário) | Não |
| O email é transmitido para a Dynamic Chat a partir de qualquer outro sistema integrado | Não |

## Domínios de email bloqueados {#blocked-email-domains}

Se houver visitantes com domínios de email com os quais você não deseja que seus agentes interajam (por exemplo, um concorrente), adicione o domínio de email deles à pesquisa.

1. Selecione o controle deslizante **Habilitar Validação** para ativar o arquivo de inclui na lista de bloqueios. Insira até 50 domínios e clique em **Salvar**.

   ![](assets/security-settings-2.png)

## Domínios permitidos {#allowed-domains}

A adição de domínios permitidos garante que terceiros não possam remover o javascript do seu site e adicioná-lo aos seus próprios.

1. Selecione o controle deslizante **Habilitar Validação** para ativar o incluo na lista de permissões. Insira os domínios permitidos e clique em **Salvar**.

   ![](assets/security-settings-3.png)
