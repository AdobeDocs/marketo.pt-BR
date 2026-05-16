---
unique-page-id: 12983101
description: Saiba como mapear campos personalizados de anúncios de lead do Facebook para o Marketo. Verifique se os dados dos anúncios principais estão mapeados para os campos de pessoa corretos no Marketo.
title: Mapear campos personalizados para o Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
TQID: https://experienceleague.adobe.com/whJl1biZjBUAZp0w3kkmM5AplWTDXcV3-2KayHmsMnE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 266
ht-degree: 7%

---

# Mapear campos personalizados para o Marketo {#map-custom-fields-to-marketo}

Você pode coletar mais do que as informações padrão armazenadas por padrão [!DNL Facebook], como a frequência com que alguém usa seu serviço de entrega online. Você pode fazer isso [criando perguntas personalizadas](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) nos seus [!DNL Facebook] anúncios de cliente potencial.

No entanto, o **Marketo não iniciará automaticamente a coleta desses dados**. Para que o Marketo comece a capturar valores de campos personalizados, você **deve** mapear esses campos personalizados para um campo no Marketo.

Siga estas etapas para configurar isso na área LaunchPoint do Administrador.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

1. Vá para a área de Administração e clique em **[!UICONTROL LaunchPoint]**. Em Serviços Instalados, localize e edite os **[!UICONTROL Anúncios de Cliente Potencial do Facebook]**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Clique em **[!UICONTROL Next]**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Deixe a conta autorizada como está, **não** faça alterações. Clique em **[!UICONTROL Next]**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Como antes, deixe as páginas selecionadas como estão, **não** faça alterações. Clique em **[!UICONTROL Next]**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Mapeie o campo personalizado [!DNL Facebook] para seu campo do Marketo. Clique em **[!UICONTROL Adicionar].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Na nova linha, digite o nome do campo personalizado [!DNL Facebook].

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Somente os campos que foram salvos em [!DNL Facebook] modelos de formulário aparecerão como opções aqui.

1. Clique na coluna **[!UICONTROL Campo do Marketo]**. Digite para procurar o campo para o qual deseja mapear. Após selecionar um campo, clique em **[!UICONTROL Salvar]**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Se você ainda não tiver um campo no Marketo para mapear o campo [!DNL Facebook], saiba como [criar campos personalizados](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Você **deve** passar por esse processo para qualquer novo campo [!DNL Facebook] para que a Marketo colete os dados.
