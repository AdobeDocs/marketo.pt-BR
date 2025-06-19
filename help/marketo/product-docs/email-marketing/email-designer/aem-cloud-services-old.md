---
title: Conectar documento do Experience Manager
description: Saiba como conectar o Adobe Experience Manager Cloud Services ao Adobe Marketo Engage para poder aproveitar seus ativos da AEM.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Conectar o Adobe Experience Manager Cloud Services {#connect-adobe-experience-manager-cloud-services}

Saiba como conectar sua conta do AEM Assets Cloud Services à instância do Adobe Marketo Engage para poder aproveitar o repositório do AEM Asset no Marketo Engage Email Designer.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. No Marketo Engage, vá para a área **Admin** e selecione **Adobe Experience Manager** na árvore de navegação esquerda.

CAPTURA DE TELA

1. Clique em **Editar** ao lado de _Adobe Experience Manager Cloud Services_.

CAPTURA DE TELA

1. Selecione um ou mais repositórios.

CAPTURA DE TELA

>[!NOTE]
>
>Somente repositórios que foram associados na mesma organização IMS que sua assinatura do Marketo Engage são listados.

1. Você deve adicionar um [certificado de credencial de serviço](https://experienceleague.adobe.com/pt-br/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) para configurar o repositório. Clique no botão **+ Adicionar certificado**.

CAPTURA DE TELA

1. Arraste e solte o certificado (somente arquivo JSON) ou selecione-o no computador. Clique em **Adicionar** quando terminar.

CAPTURA DE TELA

1. O repositório configurado é exibido abaixo, juntamente com o status e a expiração. Clique no botão de reticências (**...**) para exibir o certificado. Caso contrário, você está pronto.

CAPTURA DE TELA

Agora, todas as imagens da biblioteca de gerenciamento de ativos digitais nesse repositório podem ser acessadas no Marketo Engage Email Designer.

>[!MORELIKETHIS]
>
>[Trabalhar com ativos da Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
