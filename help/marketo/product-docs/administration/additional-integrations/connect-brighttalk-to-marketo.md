---
unique-page-id: 15695874
description: Conecte o BrightTALK ao Marketo - Documentos do Marketo - Documentação do produto
title: Conectar BrightTALK ao Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Conectar BrightTALK ao Marketo {#connect-brighttalk-to-marketo}

Saiba como conectar seu canal BrightTALK à sua instância do Marketo. Para fazer isso, você deve ser um Administrador de ambos.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Etapas no BrightTALK {#steps-in-brighttalk}

1. Faça logon em [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} e clique em **Conectar agora**.
1. Em Conector Marketo avançado, clique em **Connect**.
1. Você aparecerá na tela de credenciais, solicitando: ID do cliente, Segredo do cliente, URL do serviço de identidade e URL do serviço de restauração. Para obter essas informações, faça logon no Marketo.

## Etapas no Marketo {#steps-in-marketo}

>[!NOTE]
>
>Neste ponto, você precisará configurar uma função de usuário somente API e um usuário de API para restringir quais permissões o BrightTALK terá em sua instância do Marketo. Como já temos artigos para essas etapas, nós o vincularemos a elas.

1. Crie um [Função de usuário somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}.

1. [Criar um usuário de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;}, usando a Função da API BrightTALK criada durante a Etapa 4.

1. Volte para a área Admin .

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Em Integração, clique em **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Clique no botão **Novo** e selecione **Novo Serviço**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Insira um Nome de exibição de sua escolha. Clique no menu suspenso Service e selecione **Personalizado** (do _not_ selecione BrightTALK).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Lembre-se de não selecionar BrightTALK no menu suspenso. É um campo que estamos no processo de remoção e selecioná-lo pode criar problemas significativos com sua integração Marketo/BrightTALK.

1. Insira uma Descrição de sua escolha. Clique na lista suspensa Somente usuário da API e selecione o Usuário da API do BrightTALK que você criou durante a Etapa 5. Clique em **Criar**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Clique em **Exibir detalhes** para o serviço personalizado que você acabou de criar.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Copie (e salve) a variável **ID do cliente** e **Segredo do cliente**. Clique em **Fechar**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Em Integração, selecione **Serviços Web**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Em Rest API, copie (e salve) a variável **Endpoint** e **Identidade**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Etapas adicionais no BrightTALK {#additional-steps-in-brighttalk}

1. Retorne à tela de configuração do conector BrightTALK da Etapa 3 e insira as credenciais salvas das Etapas 12 e 14.

   Depois que as credenciais forem autenticadas, você terá conectado oficialmente o BrightTALK ao Marketo. A próxima etapa é determinar [quais campos de dados você deseja sincronizar](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}.
