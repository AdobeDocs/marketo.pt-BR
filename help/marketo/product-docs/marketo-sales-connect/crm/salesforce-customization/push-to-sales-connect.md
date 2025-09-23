---
unique-page-id: 14352477
description: Enviar para [!DNL Sales Connect] - Documentação do Marketo - Documentação do produto
title: Enviar para [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Encaminhar para [!DNL Sales Connect] {#push-to-sales-connect}

Nosso botão [!UICONTROL Encaminhar para Contorno] selecionará uma lista de seus clientes em potencial/contatos em [!DNL Salesforce] e os encaminhará para um grupo em [!DNL Sales Connect]. Você pode enviar rapidamente um email de grupo personalizável com rastreamento Tout anexado.

## Requisitos {#requirements}

* Pacote [!DNL Sales Connect Salesforce] instalado por [!DNL Salesforce] Administrador

* [!UICONTROL Botão Enviar para o Sales Connect] instalado para exibição de lista pelo administrador [!DNL Salesforce]

* [!DNL Salesforce] Conexão estabelecida com [!DNL Sales Connect] para o usuário que está fazendo o Push

## Como {#how-to}

1. Clique na guia **[!UICONTROL Lead/Contato]** em [!DNL Salesforce].
1. Alternar para o Modo de Exibição de Lista que você deseja enviar para [!DNL Sales Connect] ao lado do botão [!UICONTROL Ir].
1. Clique em **[!UICONTROL Ir]**.
1. Selecione todos os clientes em potencial/contatos que você deseja enviar para o tout.
1. Selecione **[!UICONTROL Enviar para o MSE]**.
1. Uma nova janela será exibida verificando o número de leads/contatos que você gostaria de enviar. Selecione **[!UICONTROL Prosseguir para o Grupo]**.[!DNL Sales Connect] não enviará por push nenhum contato marcado como [!UICONTROL Recusa de email] em [!DNL Salesforce] ou [!UICONTROL Cancelamento de assinatura] em [!DNL Sales Connect].

   >[!NOTE]
   >
   >[!DNL Sales Connect] adicionará este grupo chamado &quot;SFDC-...&quot; à página Relações no [aplicativo Web](https://toutapp.com/login).

1. Selecione **[!UICONTROL Enviar Email para o Grupo Inteiro]** para enviar este email de grupo.
