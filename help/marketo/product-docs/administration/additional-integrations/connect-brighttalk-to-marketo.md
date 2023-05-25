---
unique-page-id: 15695874
description: "Conectar [!DNL BrightTALK] para Marketo - Documentação do Marketo - Documentação do produto"
title: "Conectar [!DNL BrightTALK] para o Marketo"
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# Conectar [!DNL BrightTALK] para o Marketo {#connect-brighttalk-to-marketo}

Saiba como conectar seu [!DNL BrightTALK] para sua instância do Marketo. Para fazer isso, você deve ser um Administrador para ambos.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Etapas em [!DNL BrightTALK] {#steps-in-brighttalk}

1. Efetue logon no [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} e clique em **[!UICONTROL Conectar agora]**.
1. Em [!UICONTROL Conector avançado do Marketo], clique em **[!UICONTROL Conectar]**.
1. Você chegará à tela de credenciais solicitando: ID do cliente, Segredo do cliente, URL do serviço de identidade e URL do serviço Rest. Para obter essas informações, faça logon no Marketo.

## Etapas no Marketo {#steps-in-marketo}

>[!NOTE]
>
>Neste ponto, será necessário configurar um [!DNL API Only User Role] e [!DNL API User] para restringir quais permissões [!DNL BrightTALK] terá na instância do Marketo. Como já temos artigos para essas etapas, vincularemos você a elas.

1. Criar um [Função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Criar um usuário da API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}, utilizando o [!DNL BrightTALK] Função de API criada durante a Etapa 4.

1. Volte para o **[!UICONTROL Admin]** área.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Em **[!UICONTROL Integração]**, clique em **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo serviço]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Insira um **[!UICONTROL Nome de exibição]** de sua escolha. Clique em **[!UICONTROL Serviço]** e selecione **[!UICONTROL Personalizado]** (fazer _não_ selecionar [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Lembre-se de não selecionar [!DNL BrightTALK] no menu suspenso. É um campo que estamos removendo, e selecioná-lo pode criar problemas significativos com seu [!DNL Marketo/BrightTALK] integração.

1. Insira um [!UICONTROL Descrição] de sua escolha. Clique em **[!UICONTROL Somente usuário da API]** e selecione o [!DNL BrightTALK API User] você criou durante a Etapa 5. Clique em **[!UICONTROL Criar]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Clique em **[!UICONTROL Exibir detalhes]** para o serviço personalizado que acabou de criar.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copie (e salve) o **[!UICONTROL ID do cliente]** e **[!UICONTROL Segredo do cliente]**. Clique em **[!UICONTROL Fechar]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Em **[!UICONTROL Integração]**, selecione **[!UICONTROL Serviços da Web]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Em **[!UICONTROL API Rest]**, copie (e salve) o **[!UICONTROL Endpoint]** e **[!UICONTROL Identidade]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Etapas adicionais no [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Retorne para a [!DNL BrightTALK] tela de configuração do conector da Etapa 3 e insira as credenciais salvas nas Etapas 12 e 14.

Depois que as credenciais forem autenticadas, você terá se conectado oficialmente [!DNL BrightTALK] para o Marketo. A próxima etapa é determinar [quais campos de dados você deseja sincronizar](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
