---
unique-page-id: 14746470
description: Configuração de um canal de entrega personalizado - Documentos do Marketo - Documentação do produto
title: Configuração de um canal de delivery personalizado
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# Configurando um Canal de Entrega Personalizado {#setting-up-a-custom-delivery-channel}

O Marketo Sales Connect permite integrar com um servidor SMTP personalizado para a entrega de seus emails. Essa é uma ótima opção para aqueles que não desejam enviar emails em massa a partir do canal de delivery do Gmail ou Exchange.

Os usuários podem configurar um servidor SMTP personalizado para uso individual, ou os administradores podem configurar um SMTP de equipe para ser compartilhado em todos os usuários do Sales Connect em sua instância.

>[!NOTE]
>
>* Além de configurar o servidor SMTP, sua [identidade de email deve ser verificada](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) antes de enviar emails.
>* Recomendamos trabalhar com sua equipe de TI ou fornecedor de servidor SMTP para obter as credenciais de servidor certas para seu servidor SMTP.
>* Não é possível conectar seu servidor Gmail e Exchange usando as credenciais do servidor SMTP. Use nosso serviço de Conexão de email para integrar a esses provedores.


## SMTP personalizado {#custom-smtp}

1. Faça logon no [web application](https://toutapp.com/login), clique no ícone de engrenagem na parte superior direita e escolha **Settings**.

   ![](assets/setting-up-a-custom-delivery-channel-1.png)

1. Em Minha conta, clique em **Configurações de email**.

   ![](assets/setting-up-a-custom-delivery-channel-2.png)

1. Clique em **Canal de entrega personalizado**.

   ![](assets/setting-up-a-custom-delivery-channel-3.png)

1. Insira suas credenciais do Servidor SMTP e clique em **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-4.png)

   >[!NOTE]
   >
   >Se este for seu único canal de delivery, ele será automaticamente atribuído a todas as suas identidades de email, e você estará pronto aqui. Se este não for o seu único canal de delivery, continue para a Etapa 5.

1. Ainda em Configurações de email, clique em **Endereço e Assinatura**.

   ![](assets/setting-up-a-custom-delivery-channel-5.png)

1. Encontre a identidade do email para a qual deseja escolher um canal de delivery e clique em **Escolher Canal de Entrega**.

   ![](assets/setting-up-a-custom-delivery-channel-6.png)

1. No Cartão de entrega, clique em **Editar**.

   ![](assets/setting-up-a-custom-delivery-channel-7.png)

1. Clique no menu suspenso Channel e escolha o canal de delivery personalizado que acabou de adicionar. Clique em **Salvar**.

   ![](assets/setting-up-a-custom-delivery-channel-8.png)

   >[!NOTE]
   >
   >Se o administrador da equipe configurar o Team SMTP Server, ele será aplicado automaticamente somente à sua identidade de email padrão e estará disponível como uma opção para suas outras identidades de email.

## Servidor SMTP de Equipe {#team-smtp-server}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no [web application](https://toutapp.com/login), clique no ícone de engrenagem na parte superior direita e escolha **Settings**.

   ![](assets/setting-up-a-custom-delivery-channel-9.png)

1. Em Configurações de administração, clique em **Geral**.

   ![](assets/setting-up-a-custom-delivery-channel-10.png)

1. Clique em **Canal de entrega de equipe**.

   ![](assets/setting-up-a-custom-delivery-channel-11.png)

1. Insira suas credenciais do Servidor SMTP e clique em **Connect**.

   ![](assets/setting-up-a-custom-delivery-channel-12.png)

   >[!NOTE]
   >
   >O Team SMTP Server será o canal de entrega padrão da identidade de email padrão para todos os membros da equipe. Além disso, ele estará disponível como uma opção de canal de delivery para todas as outras identidades de email.

   >[!MORELIKETHIS]
   >
   >* [Conexão de email para usuários do Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
      >
      >
   * [Conexão de email para usuários do Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

