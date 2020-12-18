---
unique-page-id: 12976798
description: Configurar o LinkedIn Lead Gen Forms - Documentos do Marketing - Documentação do produto
title: Configurar o LinkedIn Lead Gen Forms
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 0%

---


# Configurar o LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Use o LinkedIn Lead Gen Forms para executar campanhas de publicidade no LinkedIn e gerar clientes potenciais para o Marketing.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para Marketo **Admin**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vá para **LaunchPoint**, clique em **Novo** e selecione **Novo Serviço**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Digite um **Nome de exibição** para seu serviço, selecione o serviço **Gen de cliente potencial do LinkedIn **no menu suspenso e clique em **Próximo**.

   ![](assets/linkedin-lead-gen.png)

1. O Marketo abre uma nova guia no mesmo navegador para [www.linkedin.com](http://www.linkedin.com). Faça logon no LinkedIn usando a conta que deseja usar para a integração.

   >[!NOTE]
   >
   >A conta do LinkedIn precisa acessar todas as contas comerciais do LinkedIn para as quais você está criando campanhas patrocinadas.

   ![](assets/linkedin-login.png)

1. Depois de se conectar ao LinkedIn, volte ao Marketing e clique em **Autorizar**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando solicitado, clique em **Permitir **para aceitar a instalação do aplicativo Marketo no LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Você vai notar que agora está autorizado. Clique em **Próximo**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >O serviço expira automaticamente um ano após a autorização. Para recuperar o acesso, basta clicar em **Autorizar novamente**. Talvez seja necessário digitar novamente sua senha do LinkedIn, dependendo das configurações do navegador.

1. Selecione a(s) conta(s) da qual deseja que o LinkedIn Lead Gen entre no Marketing e clique em **Próximo**.

   >[!TIP]
   >
   >Se você não vir as Contas comerciais que está esperando, verifique se a conta do LinkedIn do usuário que está sendo autorizada tem permissões de gerente de formulário principal para a conta comercial no LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Para aceitar mapeamentos de campos padrão do LinkedIn para o Marketing, basta clicar em **Criar**. Se você deseja alterar o mapeamento de campo padrão, remover um mapeamento de campo ou adicionar um novo mapeamento de campo, é possível fazer isso por campo por meio do modal abaixo.

   >[!CAUTION]
   >
   >O Marketo oferece suporte ao mapeamento de dois campos do LinkedIn para um único campo do Marketo, **mas somente quando** os dois campos do LinkedIn não estão no mesmo formulário. Se dois campos forem mapeados do mesmo formulário do LinkedIn para um único campo de marketing, talvez as pessoas não consigam entrar no banco de dados do Marketing to.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Somente os campos do LinkedIn que já foram salvos em um [modelo de formulário](https://www.linkedin.com/help/lms/answer/79634) no Gerenciador de Campanhas do LinkedIn serão exibidos como Campos do LinkedIn que podem ser mapeados para campos do Marketo.

   ![](assets/linkedin-installed-services.png)

Muito bem! As pessoas que enviam formulários do LinkedIn Lead Gen serão start fluindo para o Marketo à medida que você executa campanhas bem-sucedidas no lado do LinkedIn.

>[!NOTE]
>
>Você só pode autorizar uma única conta de usuário do LinkedIn. Se você tiver várias contas comerciais que deseja vincular ao Marketo, verifique se a conta do LinkedIn do usuário que está sendo autorizada tem permissões de gerente de formulário principal para a conta comercial no LinkedIn.

>[!MORELIKETHIS]
>
>* [Usar Filtros e acionadores de formulário do LinkedIn em uma Campanha inteligente](use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)

>



