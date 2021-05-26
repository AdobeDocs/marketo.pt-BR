---
unique-page-id: 42762511
description: Configurar o compartilhamento de público na Adobe Experience Cloud - Documentos do Marketo - Documentação do produto
title: Configurar o compartilhamento de público na Adobe Experience Cloud
exl-id: d20be0d5-508f-40b9-a267-b6752643c311
source-git-commit: c225facfb3fce2d9e03ca1db5aa1ce0fee4f686c
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Configurar o compartilhamento de público no Adobe Experience Cloud {#set-up-adobe-experience-cloud-audience-sharing}

Para compartilhar dados do público-alvo nos aplicativos do Adobe, primeiro você deve inserir suas credenciais da Org do Adobe IMS no Marketo. Veja como.

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo não pode usar essa integração.

1. No Marketo, clique em **Admin**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-1.png)

1. Em Integração, clique em **Mapeamento da organização do Adobe**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-2.png)

1. Clique em **Editar**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-3.png)

1. Insira sua ID organizacional Adobe IMS (saiba como encontrar esse [aqui](https://experienceleague.adobe.com/docs/control-panel/using/faq.html)) e clique em **OK**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-4.png)

1. Clique em **Confirmar**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-5.png)

1. Clique em **Fechar**.

   ![](assets/set-up-adobe-experience-cloud-audience-sharing-6.png)

   >[!NOTE]
   >
   >Por motivos de segurança, você deve ser um Org Admin da organização do Adobe para a qual deseja mapear. Se não estiver, a ação falhará.

1. Se você já estiver _não_ conectado, uma pop-up será exibida em uma nova guia/janela. Faça logon na organização do Adobe (esta ação valida o acesso da organização).

E é isso! Agora é possível [compartilhar dados de público-alvo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md) em ou [sincronizar um público-alvo](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/sync-an-audience-from-adobe-experience-cloud.md) do Adobe Experience Cloud.
