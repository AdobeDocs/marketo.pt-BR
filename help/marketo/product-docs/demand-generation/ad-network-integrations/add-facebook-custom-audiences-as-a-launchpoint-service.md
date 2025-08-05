---
unique-page-id: 4720257
description: Adicionar [!DNL Facebook] Públicos-alvo personalizados como um [!DNL LaunchPoint] Serviço - Documentação do Marketo - Documentação do produto
title: Adicionar [!DNL Facebook] Públicos-alvo Personalizados como um [!DNL LaunchPoint] Serviço
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Adicionar [!DNL Facebook] públicos-alvo personalizados como um serviço de [!DNL LaunchPoint] {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Com essa integração, você pode enviar dados de público-alvo de listas estáticas e inteligentes do Marketo para o [!DNL Facebook] para serem usados como Públicos-alvo personalizados em [!DNL Facebook] Campanhas publicitárias. Veja como configurar isso.

1. Vá para o **[!UICONTROL Administrador]** do Marketo.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vá para **[!UICONTROL LaunchPoint]**, clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Novo Serviço]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Digite um **[!UICONTROL Nome para Exibição]** para o seu serviço e selecione o serviço **[!UICONTROL Públicos-Alvo Personalizados do Facebook]** no menu suspenso **[!UICONTROL Serviço]**.

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. Abra uma nova guia no mesmo navegador e vá para [facebook.com](https://www.facebook.com/). Faça logon em [!DNL Facebook] usando a conta que você deseja usar para a integração.

   >[!CAUTION]
   >
   >Para que o Marketo envie públicos-alvo através de várias contas do Ad Manager, o [!DNL Facebook] usuário que você autorizar nas etapas a seguir precisará ter acesso a *todos* dessas contas.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Depois de entrar no [!DNL Facebook], volte para a Marketo. Clique em **[!UICONTROL Autorizar]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >Você *deve* usar uma conta do Business Manager [!DNL Facebook] para que a integração de Públicos-alvo personalizados funcione. Para saber como configurar uma conta do Business Manager, consulte [[!DNL Facebook] Ajuda](https://www.facebook.com/business/help/1710077379203657).

1. Se solicitado, clique em **[!UICONTROL OK]** para aceitar a instalação do aplicativo Marketo em [!DNL Facebook].

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Agora você está autorizado! Selecione um modo correspondente e clique em **[!UICONTROL Criar]**.

   >[!NOTE]
   >
   >**[!UICONTROL Correspondência Básica]** usa apenas endereços de email. **[!UICONTROL Correspondência avançada]** usa sete campos adicionais, o que aumenta a taxa de correspondência, para mais conversão. No entanto, se a política de privacidade da sua empresa não permitir o compartilhamento de campos adicionais ou se os dados não os incluírem, selecione [!UICONTROL Correspondência básica].

   ![](assets/fb-custom-adv-matching-hands.png)

   Excelente trabalho! Agora você pode acessar qualquer lista estática ou inteligente no Marketo e enviar dados de público-alvo para o [!DNL Facebook].

   >[!CAUTION]
   >
   >Oh, antes de ir, certifique-se de [Aceitar [!DNL Facebook]&#39;s Termos de Públicos-alvo personalizados](https://www.facebook.com/ads/manage/customaudiences/tos.php) em sua conta [!DNL Facebook]! Sem fazer isso, as atualizações de público-alvo falharão.

>[!MORELIKETHIS]
>
>* [Criar um público-alvo personalizado em [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [Configurar [!DNL Facebook] Anúncios De Cliente Potencial](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
