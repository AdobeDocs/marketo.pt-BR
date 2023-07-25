---
unique-page-id: 4720257
description: Adicionar públicos-alvo personalizados da Facebook como um serviço do LaunchPoint - Documentação da Marketo - Documentação do produto
title: Adicionar públicos-alvo personalizados do Facebook como um serviço do LaunchPoint
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Adicionar públicos-alvo personalizados do Facebook como um serviço do LaunchPoint {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Com essa integração, você pode enviar dados de público-alvo de listas estáticas e inteligentes do Marketo para o Facebook para serem usados como públicos-alvo personalizados em campanhas de anúncios do Facebook. Veja como configurar isso.

1. Ir para o Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Ir para **LaunchPoint**, clique em **Novo** e selecione **Novo serviço**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Insira um **Nome de exibição** para o seu serviço e selecione o **Públicos-alvo personalizados do facebook** serviço do **Serviço** menu suspenso.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Abra uma nova guia no mesmo navegador e vá para [facebook.com](https://www.facebook.com/). Faça logon no Facebook usando a conta que deseja usar para a integração.

   >[!CAUTION]
   >
   >Para que o Marketo envie públicos-alvo em várias contas do Ad Manager, o usuário do Facebook autorizado nas etapas a seguir precisa ter acesso a *all* dessas contas.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Depois de fazer logon no Facebook, volte para a Marketo. Clique em **Autorizar**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Você _deve_ use uma conta do Facebook Business Manager para que a integração de Públicos personalizados funcione. Para saber como configurar uma conta do Business Manager, consulte [Ajuda do facebook](https://www.facebook.com/business/help/1710077379203657).

1. Se solicitado, clique em **OK** para aceitar a instalação do aplicativo Marketo no Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Agora você está autorizado! Selecione um modo correspondente e clique em **Criar**.

   >[!NOTE]
   >
   >**Correspondência básica** O usa somente endereços de email. **Correspondência avançada** O usa sete campos adicionais, o que aumenta a taxa de correspondência, para obter mais conversão. No entanto, se a política de privacidade da sua empresa não permitir o compartilhamento de campos adicionais ou se os dados não os incluírem, selecione Correspondência básica.

   ![](assets/fb-custom-adv-matching-hands.png)

   Excelente trabalho! Agora é possível acessar qualquer lista estática ou inteligente no Marketo e enviar dados de público-alvo para o Facebook.

   >[!CAUTION]
   >
   >Oh, antes de ir, certifique-se de [Aceitar os termos de públicos-alvo personalizados da Facebook](https://www.facebook.com/ads/manage/customaudiences/tos.php) na sua conta da Facebook. Sem fazer isso, as atualizações de público-alvo falharão.

>[!MORELIKETHIS]
>
>* [Criar um público-alvo personalizado no Facebook](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurar Anúncios De Cliente Potencial Da Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
