---
unique-page-id: 13796466
description: Introdução ao Sales Connect - Documentos da Marketo - Documentação do produto
title: Introdução ao Sales Connect
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Introdução ao Sales Connect {#getting-started-with-sales-connect}

Se preferir assistir a essas etapas do que lê-las, pule diretamente para as [Instruções de vídeo abaixo](#video).

>[!AVAILABILITY]
>
>Nem todos os clientes compraram essa funcionalidade. Entre em contato com o Gerente de sucesso do cliente para obter mais informações.

## O que é necessário para começar {#what-you-need-to-get-started}

* assinatura Marketo
* assinatura do Sales Connect
* Assinatura do Salesforce (com chamadas de API e classes Apex ativadas)

## Quem você precisa começar {#who-you-need-to-get-started}

* Usuário administrador do Marketo
* Usuário administrador do Sales Connect
* Administrador do Salesforce
* Usuários do Sales Connect

## Administradores do Connect de Vendas {#sales-connect-admins}

Você receberá um email do Marketo com um link para redefinir sua senha. Depois de criar uma nova senha, faça logon no Sales Connect.

Para concluir a configuração, você deve fazer o seguinte:

* [Connect Sales Connect e Salesforce](#connect-your-sales-connect-account-to-salesforce)
* [Adquira credenciais antes de conectar o Sales Connect com a Marketo](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Conexão de vendas do Connect com a Marketo](#connect-sales-connect-to-marketo)
* [Convidar/provisionar usuários](#invite-provision-users)

Opcionalmente, também é possível:

* [Testar Conexão de Vendas no Sandbox](#test-sales-connect-in-your-sandbox)

## Conecte sua conta de conexão de vendas ao Salesforce {#connect-your-sales-connect-account-to-salesforce}

Para conectar sua conta do Sales Connect à sua conta do Salesforce, como um Administrador ou um não Administrador, siga as etapas em [this article](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md).

>[!NOTE]
>
>A instância do Salesforce à qual você se conecta deve ser a mesma instância que está (ou será) conectada ao Marketo.

## Adquirir credenciais antes de conectar o Sales Connect com o Marketo {#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Você precisará obter um conjunto de credenciais do Marketo. Essas credenciais serão usadas posteriormente pelo administrador do Sales Connect para se conectar ao Marketo com o Sales Connect.

1. No Marketo, clique em **Admin**.

   ![](assets/one.png)

1. Na árvore, clique em **Sales Connect**.

   ![](assets/two.png)

1. Selecione e envie as seguintes credenciais do Marketo para o administrador do Sales Connect: ID do Munchkin, ID do cliente, Segredo do cliente.

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >Ao copiar e colar as informações acima, certifique-se de que nenhum espaço seja adicionado.

## Conectar-se de Vendas ao Marketo {#connect-sales-connect-to-marketo}

1. No Sales Connect, clique no ícone de engrenagem e selecione **Settings**.

   ![](assets/four.png)

1. Em Configurações de administração, selecione **Marketo**.

   ![](assets/eight.png)

1. Insira as credenciais do Marketo fornecidas pelo Administrador do Marketo e clique em **Connect**.

   ![](assets/credentials.png)

## Convidar/provisionar usuários {#invite-provision-users}

Se algum usuário já existir em sua conta (anteriormente do ToutApp), ele será exibido na guia **Team Access** da seção Marketo do Sales Connect.

Você pode provisionar sua equipe como um Usuário do Marketo Sales Connect nesta página. Se você nunca tiver usado o ToutApp ou ainda tiver que convidar usuários, siga as etapas em [este artigo](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md).

>[!CAUTION]
>
>Aguarde dez minutos após a conexão do Sales Connect com a Marketo antes de executar essas etapas.

1. Selecione um ou mais usuários e clique em **Conectar**.

   >[!NOTE]
   >
   >Você só pode fazer a atribuição do espaço de trabalho uma vez no momento de convidar usuários. Depois que estiver definido, você terá que desconectar o usuário para alterá-lo.

   ![](assets/users.png)

1. Se a assinatura do Marketo tiver espaços de trabalho ativados, você poderá atribuir espaços de trabalho a cada usuário ou conjunto de usuários em massa. Se nenhum espaço de trabalho for selecionado, nós os atribuiremos ao espaço de trabalho Padrão do Marketo.

   ![](assets/nine.jpg)

1. Clique na lista suspensa Espaço de trabalho , selecione os espaços de trabalho desejados e clique em **Connect**.

   ![](assets/ten.png)

   >[!NOTE]
   >
   >Se quiser adicionar novos usuários, vá para a seção Gerenciamento de equipe das Configurações de administração e clique no botão **Convidar usuários**.

Você pode incluir usuários adicionais na página Gerenciamento de equipe e seguir as etapas acima para conectá-los.

## Testar Conexão de Vendas no Sandbox {#test-sales-connect-in-your-sandbox}

Para equipes que desejam testar o Marketo Sales Connect com a Marketo Sandbox, uma conta adicional do Sales Connect pode ser provisionada mediante solicitação. Isso é somente para clientes que compraram uma sandbox da Marketo ou aqueles que a têm como parte de seu pacote do Marketo. Se você estiver interessado em adquirir uma sandbox, entre em contato com o Gerente de conta da Marketo.

>[!NOTE]
>
>Não é possível provisionar uma conta do Sales Connect com a mesma ID de email para várias instâncias. Isso significa que, se você quiser ter uma conta extra do Sales Connect para testar com sua instância do Marketo Sandbox, será necessário usar uma ID de email diferente em cada uma das contas.
