---
title: Conectar documento do Experience Manager
description: Saiba como conectar o AEM Cloud Services ao Marketo Engage. Use os ativos do AEM ao criar emails no designer.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: 'yes'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 8%
---
# Conectar o Adobe Experience Manager Cloud Services {#connect-adobe-experience-manager-cloud-services}

Saiba como conectar sua conta do AEM Assets Cloud Services à instância do Adobe Marketo Engage para poder aproveitar o repositório do AEM Asset no Marketo Engage Email Designer.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

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
