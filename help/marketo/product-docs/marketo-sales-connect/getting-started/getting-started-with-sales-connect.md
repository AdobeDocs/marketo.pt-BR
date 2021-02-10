---
unique-page-id: 13796466
description: Introdução ao Sales Connect - Documentos do Marketing - Documentação do produto
title: Introdução ao Sales Connect
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# Introdução ao Sales Connect {#getting-started-with-sales-connect}

Se preferir observar essas etapas do que lê-las, pule para as [Instruções de vídeo abaixo](#video).

>[!AVAILABILITY]
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com o Gerente de sucesso do cliente para obter mais informações.

## O que você precisa para começar {#what-you-need-to-get-started}

* Subscrição de marketing
* Subscrição do Sales Connect
* Subscrição do Salesforce (com chamadas de API e classes Apex ativadas)

## Quem você precisa para começar {#who-you-need-to-get-started}

* Usuário administrador de marketing
* Usuário administrador do Sales Connect
* Administrador do Salesforce
* Usuários do Sales Connect

## Administradores do Sales Connect {#sales-connect-admins}

Você receberá um email do Marketo com um link para redefinir sua senha. Depois de criar uma nova senha, faça logon no Sales Connect.

Para concluir a configuração, faça o seguinte:

* [Connect Sales Connect e Salesforce](#sfdc)
* [Adquira credenciais antes de conectar o Sales Connect com o Marketo](#acquire)
* [Connect Sales Connect com marketing](#mkto)
* [Convidar/provisionar usuários](#IPU)

Opcionalmente, você também pode:

* [Testar o Sales Connect em sua caixa de proteção](#sandbox)

## Conecte sua conta do Sales Connect ao Salesforce {#connect-your-sales-connect-account-to-salesforce}

Para conectar sua conta do Sales Connect à sua conta do Salesforce, como um Administrador ou não-Administrador, siga as etapas em [este artigo](http://docs.marketo.com/x/JwDb).

>[!NOTE]
>
>A instância do Salesforce à qual você se conecta deve ser a mesma que está (ou será) conectada ao Marketo.

## Adquirir credenciais antes de conectar o Sales Connect com o Marketing {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Você precisará obter um conjunto de credenciais de dentro de Marketo. Essas credenciais serão usadas posteriormente pelo administrador do Sales Connect para conectar o Marketing ao Sales Connect.

1. Em Marketo, clique em **Admin**.

   ![](assets/one.png)

1. Na árvore, clique em **Ligação de Vendas**.

   ![](assets/two.png)

1. Selecione e envie as seguintes credenciais de marketing para seu administrador do Sales Connect: ID de Munchkin, ID do cliente, Segredo do cliente.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Ao copiar e colar as informações acima, certifique-se de que nenhum espaço seja adicionado.

## Connect Sales Connect para Marketing {#connect-sales-connect-to-marketo}

1. No Sales Connect, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/four.png)

1. Em Configurações administrativas, selecione **Marketo**.

   ![](assets/eight.png)

1. Insira as credenciais de Marketo fornecidas pelo Administrador de marketing e clique em **Connect**.

   ![](assets/credentials.png)

## Convidar/provisionar usuários {#invite-provision-users}

Se algum usuário já existir em sua conta (anteriormente do ToutApp), ele será exibido na guia **Team Access** da seção Marketo do Sales Connect.

Você pode provisionar sua equipe como um usuário do Marketing to Sales Connect desta página. Se você nunca usou o ToutApp ou ainda não convidou usuários, siga as etapas em [este artigo](http://docs.marketo.com/display/TOUT/Invite+Team+Members).

>[!CAUTION]
>
>Aguarde dez minutos após conectar o Sales Connect com o Marketo antes de executar essas etapas.

1. Selecione um ou mais usuários e clique em **Connect**.

   >[!NOTE]
   >
   >Você só pode fazer a atribuição do espaço de trabalho uma vez no momento de convidar usuários. Depois de definido, você terá que desconectar o usuário para alterá-lo.

   ![](assets/users.png)

1. Se sua subscrição de marketing tiver espaços de trabalho ativados, você poderá atribuir espaços de trabalho a cada usuário ou conjunto de usuários em massa. Se nenhum espaço de trabalho for selecionado, nós os atribuiremos à área de trabalho de marketing padrão.

   ![](assets/nine.jpg)

1. Clique na lista suspensa Espaço de trabalho, selecione os espaços de trabalho desejados e clique em **Connect**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Se quiser adicionar novos usuários, vá para a seção Gerenciamento de equipe de Configurações de administrador e clique no botão **Convidar usuários**.

Você pode incluir usuários adicionais na página Gerenciamento de equipe e seguir as etapas acima para conectá-los.

## Testar conexão de vendas em sua caixa de proteção {#test-sales-connect-in-your-sandbox}

Para equipes que desejam testar o Marketing to Sales Connect com sua Marketo Sandbox, uma conta adicional do Sales Connect pode ser provisionada mediante solicitação. Isso se aplica somente aos clientes que compraram uma Marketo Sandbox, ou àqueles que a tiverem como parte de seu pacote Marketo. Se você estiver interessado em adquirir um Sandbox, entre em contato com seu Gerente de conta do Marketing Cloud.

>[!NOTE]
>
>Não é possível provisionar uma conta do Sales Connect com a mesma ID de email para várias instâncias. Isso significa que, se você quiser ter uma conta extra do Sales Connect para testar sua instância do Marketo Sandbox, será necessário usar uma ID de email diferente em cada uma das contas.
