---
unique-page-id: 12983619
description: Adicionar o Slack as a LaunchPoint Service - Documentos da Marketo - Documentação do produto
title: Adicionar o Slack como um Serviço do LaunchPoint
exl-id: 38c1501d-27ac-4c6c-967d-4decd10e0cb3
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Adicionar o Slack como um Serviço do LaunchPoint {#add-slack-as-a-launchpoint-service}

Há dois tipos de notificação incluídos na integração do Slack:

* **Notificações** do sistema: Obtenha notificações do Slack sobre eventos importantes em sua instância do Marketo, como alertas sobre os status atuais da campanha e quaisquer problemas que exijam atenção imediata (erros de CRM e limites de API).
* **Momentos** interessantes: Quando um Marketo Insight é acionado por um indivíduo conhecido de uma conta de vendas, os proprietários de leads podem ser notificados por meio do Slack. As notificações incluem informações de cliente potencial, bem como detalhes sobre a conta de vendas.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!PREREQUISITES]
>
>Se você não tiver as Notificações do Sistema do Slack já ativadas, entre em contato com o [Suporte do Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Vá para **LaunchPoint** e, em **New** clique em **New Service**.

   ![](assets/image2017-11-27-14-3a13-3a18.png)

1. Insira um nome de exibição para a integração do Slack. Na lista suspensa **Service**, selecione **Slack**. Clique em **Criar**.

   ![](assets/image2017-11-27-15-3a54-3a11.png)

1. Clique em **Autorizar**. Isso abrirá o Slack em uma nova guia, onde você concluirá a autorização e concederá a permissão do Marketo para obter informações do Slack.

   ![](assets/image2017-11-27-14-3a16-3a6.png)

1. Na nova guia Slack , insira o URL do espaço de trabalho e clique em **Continue**.

   ![](assets/image2017-11-27-15-3a1-3a29.png)

1. Insira suas credenciais do Slack e clique em **Fazer logon**.

   ![](assets/image2017-11-27-15-3a1-3a3.png)

1. Na lista suspensa **Publicar em** , selecione o canal no qual deseja que as notificações do Marketo sejam postadas. Revise as permissões solicitadas e clique em **Autorizar**.

   ![](assets/image2018-1-9-13-3a21-3a50.png)

1. Você deverá ver a tela de confirmação abaixo. A guia é fechada automaticamente.

   ![](assets/image2017-11-27-15-3a51-3a57.png)

1. Atualize a guia Marketo e confirme se o Slack agora está listado como um serviço ativo no LaunchPoint.

   ![](assets/image2017-11-27-15-3a55-3a37.png)

   As notificações começarão a ser postadas no canal selecionado na etapa 6. Eles vão se parecer com isso:

   ![](assets/samplenotification.png)
