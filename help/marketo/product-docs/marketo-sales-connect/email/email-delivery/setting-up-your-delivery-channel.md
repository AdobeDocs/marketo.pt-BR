---
unique-page-id: 14746470
description: Configuração do Canal do Delivery - Documentos do Marketing - Documentação do produto
title: Configuração do Canal do Delivery
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---


# Configuração do Canal do Delivery {#setting-up-your-delivery-channel}

Ao start usando o Marketing to Sales Connect, você precisará configurar um servidor SMTP para enviar emails.

>[!NOTE]
>
>Além de configurar seu servidor SMTP, sua [identidade de e-mail deve ser verificada](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/verify-your-email.md) antes que você possa enviar e-mails.

Você pode optar por enviar emails usando um Servidor SMTP Personalizado, um Servidor SMTP de Equipe ou Gmail como canal de delivery. Vamos analisar cada opção.

## SMTP personalizado {#custom-smtp}

1. Faça logon no [aplicativo da Web](https://toutapp.com/login), clique no ícone de engrenagem na parte superior direita e escolha **Configurações**.

   ![](assets/one.png)

1. Em Minha conta, clique em **Configurações de e-mail**.

   ![](assets/two.png)

1. Selecione **Servidor SMTP**.

   ![](assets/three.png)

1. Insira suas credenciais do Servidor SMTP e clique em **Connect**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Se este for seu único canal de delivery, ele será automaticamente atribuído a todas as suas identidades de email, e você estará pronto aqui. Se este não for seu único canal de delivery, continue com a Etapa 5.

1. Ainda em Configurações de email, clique em **Endereço e assinatura**.

   ![](assets/five.png)

1. Localize a identidade de e-mail para a qual você deseja escolher um canal de delivery e clique em **Escolher Canal de Delivery**.

   ![](assets/six.png)

1. No Cartão de entrega, clique em **Editar**.

   ![](assets/seven-new.png)

1. Clique na lista suspensa Canal e escolha o canal de delivery personalizado que você acabou de adicionar. Clique em **Salvar**.

   ![](assets/eight-new.png)

   >[!NOTE]
   >
   >Se o administrador da equipe configurar o Team SMTP Server, ele será automaticamente aplicado somente à sua identidade de email padrão e estará disponível como uma opção para suas outras identidades de email.

## Servidor SMTP de Equipe {#team-smtp-server}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no [aplicativo da Web](https://toutapp.com/login), clique no ícone de engrenagem na parte superior direita e escolha **Configurações**.

   ![](assets/nine.png)

1. Em Configurações administrativas, clique em **Team SMTP Server**.

   ![](assets/ten.png)

1. Insira suas credenciais do Servidor SMTP e clique em **Connect**.

   ![](assets/eleven.png)

   >[!NOTE]
   >
   >O Team SMTP Server será o canal de delivery padrão da identidade de email padrão para todos os membros da equipe. Além disso, ele estará disponível como uma opção de canal de delivery para todas as outras identidades de email.

## Gmail {#gmail}

1. Faça logon no [aplicativo da Web](https://toutapp.com/login), clique no ícone de engrenagem na parte superior direita e escolha **Configurações**.

   ![](assets/twelve.png)

1. Em Minha conta, clique em **Configurações de e-mail**.

   ![](assets/thirteen.png)

1. Clique em **Sincronização de e-mail**.

   ![](assets/fourteen.png)

1. Clique em **Conectar-se ao Google**.

   ![](assets/fifteen.png)

1. Faça logon usando suas credenciais do Google.

1. Quando chegar a esta tela, clique em **Permitir**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Se este for seu único canal de delivery, ele será automaticamente atribuído a todas as suas identidades de email, e você estará pronto aqui. Se o Gmail não for seu único canal de delivery, continue com a Etapa 7.

1. Clique em **Endereço e assinatura**.

   ![](assets/seventeen.png)

1. Clique na identidade de e-mail para a qual você deseja que o Gmail seja o canal do delivery.

   ![](assets/eighteen.png)

1. Quando o painel deslizante abrir, role para baixo até o Cartão de entrega.

   ![](assets/nineteen.png)

1. Clique na lista suspensa Canal e escolha o canal delivery Gmail que você acabou de adicionar. Clique em **Salvar**.

   ![](assets/twenty.png)

   >[!NOTE]
   >
   >Se o administrador da equipe configurar o Team SMTP Server, ele será automaticamente aplicado somente à sua identidade de email padrão e estará disponível como uma opção para suas outras identidades de email.
