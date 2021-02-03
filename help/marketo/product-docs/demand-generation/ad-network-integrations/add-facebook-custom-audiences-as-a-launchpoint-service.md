---
unique-page-id: 4720257
description: Adicionar Audiências personalizadas do Facebook como um serviço do LaunchPoint - Documentos do Marketing - Documentação do produto
title: Adicionar Audiências personalizadas do Facebook como um Serviço do LaunchPoint
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---


# Adicionar Audiências personalizadas do Facebook como um Serviço LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Com essa integração, você pode enviar dados de audiência do Marketing para listas estáticas e inteligentes para o Facebook para serem usados como Audiências personalizadas nas Campanhas de anúncios do Facebook. Veja como configurar.

1. Vá para Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vá para **LaunchPoint**, clique em **Novo** e selecione **Novo Serviço**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Digite um **Nome de exibição** para seu serviço e selecione o serviço **Audiência personalizado do Facebook** no menu suspenso **Service**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Abra uma nova guia no mesmo navegador e vá para [facebook.com](http://www.facebook.com/). Faça logon no Facebook usando a conta que deseja usar para a integração.

   >[!CAUTION]
   >
   >Para que o Marketo envie audiências através de várias contas do Ad Manager, o usuário do Facebook autorizado nas etapas a seguir precisa ter acesso a *todas* dessas contas.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Depois que você estiver conectado ao Facebook, volte para Marketo. Clique em **Autorizar**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Você _deve_ usar uma conta do Facebook Business Manager para que sua integração com o Audiência personalizado funcione. Para saber como configurar uma conta do Business Manager, consulte [Ajuda do Facebook](https://www.facebook.com/business/help/1710077379203657).

1. Se solicitado, clique em **OK** para aceitar a instalação do aplicativo Marketo no Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Agora você está autorizado! Selecione um modo correspondente e clique em **Criar**.

   >[!NOTE]
   >
   >**A** Correspondência básica usa somente endereços de email. **A** Correspondência avançada usa sete campos adicionais, o que aumenta a taxa de correspondência para obter mais conversão. No entanto, se sua política de privacidade do empresa não permitir o compartilhamento de campos adicionais ou se seus dados não os incluírem, selecione Correspondência básica.

   ![](assets/fb-custom-adv-matching-hands.png)

   Ótimo trabalho! Agora você pode ir até qualquer lista estática ou inteligente no Marketo e enviar dados de audiência para o Facebook.

   >[!CAUTION]
   >
   >Oh, antes de ir, certifique-se de [Aceitar os Termos de Audiência Personalizados do Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) na sua conta do Facebook! Sem isso, as atualizações de audiência falharão.

>[!MORELIKETHIS]
>
>* [Criar uma Audiência personalizada no Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
   >
   >
* [Configurar Anúncios de venda do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

