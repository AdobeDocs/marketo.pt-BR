---
description: Configuração do reCAPTCHA v3 - Documentação do Marketo - Documentação do produto
title: Configuração do reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Configuração do reCAPTCHA v3 {#setting-up-recaptcha-v3}

O ReCAPTCHA v3 é uma experiência sem atritos que classifica os envios de formulários com base em quão suspeitos eles são sem usar desafios de texto, imagem ou botão. [Saiba mais](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Recuperar seu data center e a ID do Munchkin {#retrieve-your-data-center-and-munchkin-id}

Na Etapa 6 da seção Configuração inicial do reCAPTCHA v3 abaixo, você precisará do data center da sua assinatura do Marketo Engage e da ID do Munchkin. Veja como encontrá-los.

1. No Marketo, clique em **Admin**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Clique em **Minha conta**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Role para baixo até Informações de suporte.

   ![](assets/setting-up-recaptcha-v3-3.png)

## Configuração inicial do reCAPTCHA v3 {#initial-recaptcha-v3-setup}

As etapas a seguir são executadas fora do Marketo.

1. Vá para [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} e clique no Admin Console v3.

1. Fazer logon/inscrever-se com uma conta da Google.

1. Clique no botão Criar (+) para criar uma nova chave.

1. Crie um rótulo para identificar se a chave deve ser usada para o Marketo Engage.

1. Escolha o tipo **reCAPTCHA v3**. No momento, o Marketo Engage não é compatível com o reCAPTCHA v2.

1. Adicione cada domínio que a assinatura do Marketo Engage usa. Os domínios não definidos aqui retornarão erros em formulários nos quais o reCAPTCHA está habilitado. Lembre-se de substituir as palavras &#39;datacenter&#39; e &#39;munchkinID&#39; pelos [dados da sua assinatura](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * qualquer domínio e alias de landing page configurados na assinatura

   >[!NOTE]
   >
   >Por exemplo, se o data center da sua conta for &quot;sjst&quot;, o domínio em que você incluirá na lista de permissões será `app-sjst.marketo.com`. Se a sua ID do Munchkin for 123-ABC-789, o domínio que você incluirá na lista de permissões será `123-ABC-789.mktoweb.com`.

1. Defina um proprietário e um endereço de email adicional que deve receber alertas sobre este serviço.

1. Aceite os Termos de Serviço do reCAPTCHA.

1. Clique em **Enviar**.

   >[!NOTE]
   >
   >Mantenha a chave do site e a chave secreta acessíveis para a configuração do Marketo Engage.

## Configuração de CAPTCHA no Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>Depois de seguir essas etapas e [habilitar CAPTCHA no primeiro formulário do Marketo](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}, certifique-se de testar o formulário imediatamente, pois qualquer tipo de configuração incorreta na configuração do reCAPTCHA pode quebrar o formulário.

1. No Marketo, clique em **Admin**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Selecione **CAPTCHA** na árvore.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Clique em **Editar** nas configurações de CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Clique na lista suspensa CAPTCHA e escolha reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Insira a chave secreta e a chave do site. Clique em **Salvar** quando terminar.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Habilitar CAPTCHA no Marketo Forms](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
