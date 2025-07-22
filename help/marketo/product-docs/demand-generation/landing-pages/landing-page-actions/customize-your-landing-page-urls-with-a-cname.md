---
unique-page-id: 2359746
description: Personalizar os URLs da sua página de aterrissagem com um CNAME - Documentação do Marketo - Documentação do produto
title: Personalizar os URLs da sua landing page com um CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 1%

---

# Personalizar os URLs da sua landing page com um CNAME {#customize-your-landing-page-urls-with-a-cname}

Embora o Marketo hospede suas páginas de aterrissagem, o URL pode ser totalmente personalizado. Como se parece sem um CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

A aparência desejada:

`https://go.YourCompany.com/UnsubscribePage.html`

## Escolha um CNAME {#choose-a-cname}

Escolha uma palavra para ir no início do URL das páginas de aterrissagem. É apenas uma palavra e deve ser relativamente curta. Exemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

A palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, então anote-o.

## Encontrar a Munchkin ID {#find-your-munchkin-id}

1. Vá para a área **Administrador**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clique em **Minha conta**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Permissões de administrador necessárias**

1. Role para baixo até &quot;Informações de suporte&quot; e copie sua Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Enviar solicitação para TI {#send-request-to-it}

Peça à sua equipe de TI para configurar o seguinte CNAME: (Substitua a palavra [CNAME] e [Munchkin ID] pelo texto da etapa anterior.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Concluir configuração de CNAME {#complete-cname-setup}

1. Depois que o departamento de TI criar o CNAME, vá para a área **Administrador**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clique em **Landing Pages**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Na seção **Configurações**, clique em **Editar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Digite seu CNAME em **[!UICONTROL Nome do domínio para Páginas de Aterrissagem]**, digite sua **[!UICONTROL Página de fallback]**, digite sua **[!UICONTROL Página inicial]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Sua página de fallback será a página para a qual os leads serão redirecionados se a sua página de aterrissagem do Marketo não estiver disponível.

Excelente! As páginas de aterrissagem agora são marcadas com o domínio da empresa.
