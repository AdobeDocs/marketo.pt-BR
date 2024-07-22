---
unique-page-id: 12976798
description: Configurar o LinkedIn Lead Gen Forms — Documentação do Marketo — Documentação do produto
title: Configurar o LinkedIn Lead Gen Forms
exl-id: 554a546c-adeb-4132-830d-ff15ba5cf9a1
feature: Social
source-git-commit: 94ca714d038863ad801551960c66086ea47e6b10
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Configurar o LinkedIn Lead Gen Forms {#set-up-linkedin-lead-gen-forms}

Use o LinkedIn Lead Gen Forms para executar campanhas de publicidade no LinkedIn e gerar leads para o Marketo.

>[!IMPORTANT]
>
>A linkedIn está atualizando as APIs de marketing usadas pelas integrações do Marketo Engage LinkedIn. Essas alterações exigirão a reautenticação de todos os serviços do LinkedIn LaunchPoint no menu **Admin** > **LaunchPoint** entre 7 de junho e 15 de dezembro de 2024 para evitar a interrupção do serviço. Para obter mais informações, consulte as [Perguntas frequentes sobre migração](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Um cliente potencial da LinkedIn não entrará no Marketo Engage se ele corresponder a um registro de pessoa existente no Marketo que esteja associado a um registro de empresa criado usando APIs da empresa, e a assinatura do Marketo não estiver conectada a um CRM.

1. Vá para o **Administrador** do Marketo.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vá para **LaunchPoint**, clique em **Novo** e selecione **Novo Serviço**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Insira um **Nome para Exibição** para seu serviço, selecione o serviço **LinkedIn Lead Gen** no menu suspenso e clique em **Avançar**.

   ![](assets/linkedin-lead-gen.png)

1. O Marketo abre uma nova guia no mesmo navegador em [linkedin.com](https://www.linkedin.com). Faça logon no LinkedIn usando a conta que deseja usar para a integração.

   >[!NOTE]
   >
   >A conta do LinkedIn precisa acessar todas as contas de negócios do LinkedIn para as quais você está criando campanhas patrocinadas.

   ![](assets/linkedin-login.png)

1. Depois de entrar no LinkedIn, volte para o Marketo e clique em **Autorizar**.

   ![](assets/linkedin-lead-gen-authorize.png)

1. Quando solicitado, clique em **Permitir** para aceitar a instalação do aplicativo Marketo no LinkedIn.

   ![](assets/linkedin-marketo-allow.png)

1. Você perceberá que está autorizado. Clique em **Avançar**.

   ![](assets/image2017-9-28-7-3a55-3a14.png)

   >[!CAUTION]
   >
   >O serviço expira automaticamente um ano após a autorização. Para recuperar o acesso, basta clicar em **Reautorizar**. Talvez seja necessário digitar novamente sua senha do LinkedIn, dependendo das configurações do navegador.

1. Selecione as contas das quais você deseja que os clientes potenciais do LinkedIn Lead Gen entrem no Marketo e clique em **Avançar**.

   >[!TIP]
   >
   >Se você não visualizar as Contas comerciais que está esperando, verifique se a conta do LinkedIn do usuário que está sendo autorizada tem Permissões de gerente de formulário de geração de lead para a Conta comercial no LinkedIn.

   ![](assets/linkedin-pages-to-capture.png)

1. Para aceitar o LinkedIn padrão para mapeamentos de campo do Marketo, basta clicar em **Criar**. Se você quiser alterar o mapeamento de campo padrão, remover um mapeamento de campo ou adicionar um novo mapeamento de campo, poderá fazer isso por campo por meio do modal abaixo.

   >[!CAUTION]
   >
   >O Marketo permite mapear dois campos do LinkedIn para um único campo do Marketo, **mas somente quando** os dois campos do LinkedIn não estiverem no mesmo formulário. Se você mapear dois campos do mesmo formulário do LinkedIn para um único campo do Marketo, as pessoas podem falhar ao inserir seu banco de dados do Marketo.

   ![](assets/linkedin-lead-gen-mapping.png)

   >[!NOTE]
   >
   >Somente os campos do LinkedIn que já foram salvos em um [modelo de formulário](https://www.linkedin.com/help/lms/answer/79634) no LinkedIn Campaign Manager serão exibidos como Campos do LinkedIn que podem ser mapeados para campos do Marketo.

   ![](assets/linkedin-installed-services.png)

Muito bem! As pessoas que enviam formulários de geração de lead da LinkedIn começarão a fluir para o Marketo à medida que você executa campanhas bem-sucedidas no lado do LinkedIn.

>[!NOTE]
>
>Você só pode autorizar uma única conta de usuário do LinkedIn. Se você tiver várias Contas comerciais que gostaria de vincular ao Marketo, verifique se a conta do LinkedIn do usuário que está sendo autorizada tem Permissões de gerente de formulário de geração de lead para a Conta comercial no LinkedIn.

>[!MORELIKETHIS]
>
>[Usar acionadores e filtros de formulário de geração de lead da LinkedIn em uma campanha inteligente](/help/marketo/product-docs/demand-generation/social/social-functions/use-linkedin-lead-gen-form-filters-and-triggers-in-a-smart-campaign.md)
