---
unique-page-id: 15695874
description: Conecte o BrightTALK ao Marketo - Documentos do Marketo - Documentação do produto
title: Conectar BrightTALK ao Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Conecte o BrightTALK ao Marketo {#connect-brighttalk-to-marketo}

Saiba como conectar seu canal BrightTALK à sua instância do Marketo. Para fazer isso, você deve ser um Administrador de ambos.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Etapas no BrightTALK {#steps-in-brighttalk}

1. Faça logon em [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login) e clique em **Conectar agora**.
1. Em Conector Marketo avançado, clique em **Connect**.
1. Você aparecerá na tela de credenciais, solicitando: ID do cliente, Segredo do cliente, URL do serviço de identidade e URL do serviço de restauração. Para obter essas informações, faça logon no Marketo.

## Etapas no Marketo {#steps-in-marketo}

>[!NOTE]
>
>Neste ponto, você precisará configurar uma função de usuário somente API e um usuário de API para restringir quais permissões o BrightTALK terá em sua instância do Marketo. Como já temos artigos para essas etapas, nós o vincularemos a elas.

1. Crie uma [Função de Usuário Somente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md).
1. [Crie um usuário](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) da API usando a Função da API BrightTALK criada durante a Etapa 4.
1. Volte para a área Admin .

   ![](assets/one.png)

1. Em Integração, clique em **LaunchPoint**.

   ![](assets/two.png)

1. Clique no menu suspenso **New** e selecione **New Service**.

   ![](assets/three.png)

1. Insira um Nome de exibição de sua escolha. Clique no menu suspenso Serviço e selecione **Personalizado** (do _not_ selecione BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Lembre-se de não selecionar BrightTALK no menu suspenso. É um campo que estamos no processo de remoção e selecioná-lo pode criar problemas significativos com sua integração Marketo/BrightTALK.

1. Insira uma Descrição de sua escolha. Clique na lista suspensa Somente usuário da API e selecione o Usuário da API do BrightTALK que você criou durante a Etapa 5. Clique em **Criar**.

   ![](assets/five.png)

1. Clique em **Exibir detalhes** para o serviço personalizado que você acabou de criar.

   ![](assets/six.png)

1. Copie (e salve) o **Client ID** e **Client Secret**. Clique em **Fechar**.

   ![](assets/eight-1.png)

1. Em Integração, selecione **Serviços Web**.

   ![](assets/nine-1.png)

1. Em Rest API, copie (e salve) o **Endpoint** e **Identity**.

   ![](assets/ten.png)

## Etapas adicionais no BrightTALK {#additional-steps-in-brighttalk}

1. Retorne à tela de configuração do conector BrightTALK da Etapa 3 e insira as credenciais salvas das Etapas 12 e 14.

   Depois que as credenciais forem autenticadas, você terá conectado oficialmente o BrightTALK ao Marketo. A próxima etapa é determinar [quais campos de dados você deseja sincronizar](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).
