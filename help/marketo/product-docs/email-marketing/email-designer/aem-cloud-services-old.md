---
title: Conectar Experience Manager doc
description: Saiba como conectar o Adobe Experience Manager Cloud Service ao Adobe Marketo Engage para que você possa aproveitar seus ativos do AEM.
hide: true
hidefromtoc: true
source-git-commit: 3a3c3dae689760b720c4823bc1d11bf39da998fe
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Conectar o Adobe Experience Manager Cloud Service {#connect-adobe-experience-manager-cloud-services}

Saiba como conectar sua conta do AEM Assets Cloud Service à sua instância do Adobe Marketo Engage para que você possa aproveitar seu repositório de ativos do AEM no Marketo Engage Email Designer.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. No Marketo Engage, vá para a área **Admin** e selecione **Adobe Experience Manager** na árvore de navegação esquerda.

CAPTURA DE TELA

1. Clique em **Editar** ao lado de _Adobe Experience Manager Cloud Service_.

CAPTURA DE TELA

1. Selecione um ou mais repositórios.

CAPTURA DE TELA

>[!NOTE]
>
>Somente repositórios que foram associados na mesma organização IMS que a sua assinatura do Marketo Engage são listados.

1. Você deve adicionar um [certificado de credencial de serviço](https://experienceleague.adobe.com/pt-br/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) para configurar o repositório. Clique no botão **+ Adicionar certificado**.

CAPTURA DE TELA

1. Arraste e solte o certificado (somente arquivo JSON) ou selecione-o no computador. Clique em **Adicionar** quando terminar.

CAPTURA DE TELA

1. O repositório configurado é exibido abaixo, juntamente com o status e a expiração. Clique no botão de reticências (**...**) para exibir o certificado. Caso contrário, você está pronto.

CAPTURA DE TELA

Agora, todas as imagens da biblioteca de gerenciamento de ativos digitais nesse repositório podem ser acessadas no Marketo Engage Email Designer.

>[!MORELIKETHIS]
>
>[Trabalhar com ativos do Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
