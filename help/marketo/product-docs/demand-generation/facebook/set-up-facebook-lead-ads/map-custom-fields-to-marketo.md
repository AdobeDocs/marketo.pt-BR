---
unique-page-id: 12983101
description: Mapear campos personalizados para o Marketo - Documentação do Marketo - Documentação do produto
title: Mapear campos personalizados para o Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Mapear campos personalizados para o Marketo {#map-custom-fields-to-marketo}

Você pode coletar mais do que as informações padrão armazenadas por padrão [!DNL Facebook], como a frequência com que alguém usa seu serviço de entrega online. Você pode fazer isso [criando perguntas personalizadas](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) nos seus [!DNL Facebook] anúncios de cliente potencial.

No entanto, o **Marketo não iniciará automaticamente a coleta desses dados**. Para que o Marketo comece a capturar valores de campos personalizados, você **deve** mapear esses campos personalizados para um campo no Marketo.

Veja como configurar isso na área LaunchPoint do Administrador.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área de Administração e clique em **[!UICONTROL LaunchPoint]**. Em Serviços Instalados, localize e edite os **[!UICONTROL Anúncios de Cliente Potencial do Facebook]**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Deixe a conta autorizada como está. **não** faça alterações. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Como antes, deixe as páginas selecionadas como estão. **não** faça alterações. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Aqui é onde você mapeia o campo personalizado [!DNL Facebook] para seu campo do Marketo. Clique em **[!UICONTROL Adicionar].**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Na nova linha, digite o nome do campo personalizado [!DNL Facebook].

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Somente os campos que foram salvos em [!DNL Facebook] modelos de formulário aparecerão como opções aqui.

1. Clique na coluna **[!UICONTROL Campo do Marketo]**. Digite para procurar o campo para o qual deseja mapear. Depois de selecionar um campo, clique em **[!UICONTROL Salvar]**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Se você ainda não tiver um campo no Marketo para mapear o campo [!DNL Facebook], saiba como [criar campos personalizados](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Você **deve** passar por esse processo para qualquer novo campo [!DNL Facebook] para que a Marketo colete os dados.
