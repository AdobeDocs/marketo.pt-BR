---
unique-page-id: 12976798
description: Configurar LinkedIn Lead Gen Forms - Documentos do Marketo - Documentação do produto
title: Configurar o LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Configurar o LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Use o LinkedIn Lead Gen Forms para executar campanhas de anúncios no LinkedIn e gerar leads para Marketo.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Ir para o Marketo **Administrador**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Ir para **LaunchPoint**, clique em **Novo** e selecione **Novo Serviço**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Insira um **Nome de exibição** para o seu serviço, selecione o **Gerente líder da linkedIn** na lista suspensa e clique em **Próximo**.

   ![](assets/linkedin-lead-gen.png)

1. O Marketo abre uma nova guia no mesmo navegador para [linkedin.com](https://www.linkedin.com). Faça logon no LinkedIn usando a conta que deseja usar para a integração.

   >[!NOTE]
   >
   >A conta do LinkedIn precisa acessar todas as contas comerciais da LinkedIn para as quais você está criando campanhas patrocinadas.

   ![](assets/linkedin-login.png)

1. Depois de fazer logon no LinkedIn, volte para a Marketo e clique em **Autorizar**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando solicitado, clique em **Permitir** para aceitar a instalação do aplicativo Marketo no LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Você perceberá que está autorizado. Clique em **Próximo**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >O serviço expira automaticamente um ano após a autorização. Para recuperar o acesso, basta clicar em **Autorizar novamente**. Talvez seja necessário digitar novamente a senha do LinkedIn, dependendo das configurações do navegador.

1. Selecione a(s) conta(s) que você deseja que o lead genere do LinkedIn entre no Marketo e clique em **Próximo**.

   >[!TIP]
   >
   >Se você não vir as Contas comerciais que está esperando, verifique se a conta LinkedIn do usuário que está sendo autorizada tem Permissões de Gerente de formulário de lead para a Conta comercial no LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Para aceitar os mapeamentos de campo padrão do LinkedIn para Marketo, basta clicar em **Criar**. Se desejar alterar o mapeamento de campo padrão, remover um mapeamento de campo ou adicionar um novo mapeamento de campo, é possível fazer isso por campo por meio do modal abaixo.

   >[!CAUTION]
   >
   >O Marketo suporta o mapeamento de dois campos LinkedIn para um único campo do Marketo, **mas somente quando** os dois campos LinkedIn não estão no mesmo formulário. Se dois campos forem mapeados do mesmo formulário LinkedIn para um único campo do Marketo, talvez não seja possível as pessoas entrarem no banco de dados do Marketo.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Somente os campos do LinkedIn que já foram salvos em um [modelo de formulário](https://www.linkedin.com/help/lms/answer/79634) no LinkedIn Campaign Manager será exibido como Campos do LinkedIn que podem ser mapeados para campos do Marketo.

   ![](assets/linkedin-installed-services.png)

Muito bem! As pessoas que enviam formulários do LinkedIn Lead Gen começarão a fluir para o Marketo à medida que você executa campanhas bem-sucedidas no lado do LinkedIn.

>[!NOTE]
>
>Você só pode autorizar uma única conta de usuário do LinkedIn. Se você tiver várias contas comerciais que gostaria de vincular ao Marketo, verifique se a conta do LinkedIn do usuário que está sendo autorizada tem permissões de gerente de formulário do lead para a conta comercial no LinkedIn.

>[!MORELIKETHIS]
>
>[Usar filtros e acionadores de formulário do líder do LinkedIn em uma campanha inteligente](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
