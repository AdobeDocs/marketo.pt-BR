---
unique-page-id: 15695874
description: Connect BrightTALK to Marketo - Documentos do Marketing - Documentação do produto
title: Conexão BrightTALK ao Marketo
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Ligar BrightTALK a Marketo {#connect-brighttalk-to-marketo}

Saiba como conectar seu canal BrightTALK à sua instância do Marketo. Para fazer isso, você deve ser um Administrador para ambos.

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Etapas no BrightTALK {#steps-in-brighttalk}

1. Faça logon em [business.brighttalk.com/demandcentral](http://business.brighttalk.com/demandcentral/login) e clique em **Conectar agora**.
1. Em Conector de marketing avançado, clique em **Connect**.
1. Você verá a tela de credenciais, solicitando: ID do cliente, segredo do cliente, URL do serviço de identidade e URL do serviço de restauração. Para obter essas informações, faça logon no Marketo.

## Etapas no Marketo {#steps-in-marketo}

>[!NOTE]
>
>Nesse ponto, você será solicitado a configurar uma função de usuário somente API e um usuário de API para restringir quais permissões BrightTALK terá na sua instância de Marketo. Como já temos artigos para essas etapas, conectaremos você a elas.

1. Crie uma função de usuário somente [API](http://docs.marketo.com/x/iwMk).
1. [Crie um usuário](http://docs.marketo.com/x/jwMk) da API usando a Função da API BrightTALK criada durante a Etapa 4.
1. Volte para a área Admin.

   ![](assets/one.png)

1. Em Integração, clique em **LaunchPoint**.

   ![](assets/two.png)

1. Clique no menu suspenso **Novo** e selecione **Novo serviço**.

   ![](assets/three.png)

1. Insira um Nome de exibição de sua escolha. Clique na lista suspensa Serviço e selecione **Personalizado** (do **not** selecione BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Lembre-se de não selecionar BrightTALK no menu suspenso. Trata-se de um campo que está sendo removido e sua seleção pode criar problemas significativos com a integração entre o Marketing e o BrightTALK.

1. Informe uma Descrição de sua escolha. Clique no menu suspenso Somente usuário da API e selecione o Usuário da API BrightTALK que você criou durante a Etapa 5. Clique em **Criar**.

   ![](assets/five.png)

1. Clique em **Detalhes da Visualização** para obter o serviço personalizado que você acabou de criar.

   ![](assets/six.png)

1. Copie (e salve) a **ID do cliente** e **Segredo do cliente**. Clique em **Fechar**.

   ![](assets/eight-1.png)

1. Em Integração, selecione **Serviços Web**.

   ![](assets/nine-1.png)

1. Em Restaurar API, copie (e salve) o **Endpoint** e **Identity**.

   ![](assets/ten.png)

## Etapas no BrightTALK {#steps-in-brighttalk-1}

1. Retorne à tela de configuração do conector BrightTALK da Etapa 3 e insira as credenciais salvas das Etapas 12 e 14.

   Depois que as credenciais forem autenticadas, você conectou oficialmente o BrightTALK ao Marketo. A próxima etapa é determinar [quais campos de dados você gostaria de sincronizar](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync).

