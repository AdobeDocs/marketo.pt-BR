---
unique-page-id: 42762511
description: Configurar o Adobe Organization Mapping - Documentação do Marketo - Documentação do produto
title: Configurar o mapeamento da organização da Adobe
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
feature: Integrations
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 1%

---

# Configurar o mapeamento da organização da Adobe {#set-up-adobe-organization-mapping}

Para sincronizar com aplicativos do Adobe, como o Audience Manager, o conector B2B CDP Marketo, [!DNL Dynamic Chat] etc., primeiro você deve inserir suas credenciais da Organização IMS da Adobe no Marketo Engage.

>[!NOTE]
>
>* Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.
>* Para que a integração funcione, o Marketo e outros aplicativos da Adobe devem estar na mesma organização.

>[!IMPORTANT]
>
>Para os integrados à Adobe Business Platform e ao Identity Management System, a ID da organização associada à assinatura já estará preenchida e será um campo somente leitura. Sendo assim, as etapas deste artigo não se aplicam.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Em Integração, clique em **[!UICONTROL Mapeamento da organização da Adobe]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Insira sua ID organizacional IMS da Adobe (saiba como localizar [aqui](https://experienceleague.adobe.com/docs/control-panel/using/faq.html){target="_blank"}) e clique em **[!UICONTROL OK]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Clique em **[!UICONTROL Confirmar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Clique em **[!UICONTROL Fechar]**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!IMPORTANT]
   >
   >Por motivos de segurança, você deve ser um Org Admin da Organização da Adobe para a qual deseja mapear. Se você não estiver, a ação falhará. Além disso, o usuário do Adobe e o usuário do Marketo devem usar o mesmo endereço de email ao fazer logon.

1. Se você _não_ já estiver conectado, um pop-up será exibido em uma nova guia/janela. Fazer logon na organização da Adobe (essa ação valida o acesso à organização).

Agora você pode [compartilhar dados de público-alvo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md){target="_blank"} com a Adobe Experience Cloud ou [sincronizar um público-alvo](/help/marketo/product-docs/adobe-experience-cloud-integrations/sync-an-audience-from-adobe-experience-cloud.md){target="_blank"} dela.
