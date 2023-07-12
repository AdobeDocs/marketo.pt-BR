---
unique-page-id: 42762511
description: Configurar o mapeamento da organização do Adobe - Documentação do Marketo - Documentação do produto
title: Configurar o mapeamento da organização do Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: dd4fb7dfc92580c58da70d603b6d92bd8f64493c
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Configurar o mapeamento da organização do Adobe {#set-up-adobe-organization-mapping}

Para sincronizar com aplicativos Adobe, como o Audience Manager, o conector B2B CDP Marketo, [!DNL Dynamic Chat], etc., você deve primeiro inserir suas credenciais da Organização Adobe IMS no Marketo.

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.

>[!CAUTION]
>
>Para clientes integrados ao Adobe Business Platform e ao Identity Management System, a ID da organização associada à assinatura já estará preenchida e será um campo somente leitura.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Em Integração, clique em **[!UICONTROL Mapeamento da organização Adobe]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Insira sua ID organizacional IMS da Adobe (saiba como descobrir isso) [aqui](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) e clique em **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Clique em **[!UICONTROL Confirmar o]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Clique em **[!UICONTROL Fechar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Por motivos de segurança, você deve ser um Org Admin para a Organização Adobe para a qual deseja mapear. Se você não estiver, a ação falhará. Além disso, o usuário do Adobe e o usuário do Marketo devem usar o mesmo endereço de email ao fazer logon.

1. Se você estiver _não_ já conectado, uma janela pop-up será exibida em uma nova guia/janela. Faça logon na organização Adobe (essa ação valida o acesso à organização).

E é isso! Agora você pode [compartilhar dados de público](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} to, or [sync an audience](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} do Adobe Experience Cloud.
