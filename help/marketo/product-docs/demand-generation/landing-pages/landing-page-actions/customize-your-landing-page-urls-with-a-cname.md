---
unique-page-id: 2359746
description: Personalize seus URLs de página de aterrissagem com um CNAME - Documentos do Marketo - Documentação do produto
title: Personalize seus URLs de página inicial com um CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 1%

---

# Personalize seus URLs de página inicial com um CNAME {#customize-your-landing-page-urls-with-a-cname}

Mesmo que o Marketo hospede suas páginas de aterrissagem, o URL pode ser totalmente personalizado. Como é sem um CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

A aparência:

`https://go.YourCompany.com/UnsubscribePage.html`

## Escolha um CNAME {#choose-a-cname}

Escolha uma palavra para ir no início do URL de suas landing pages. É apenas uma palavra e deve ser relativamente curta. Exemplos:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

A única palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, então anote isso.

## Encontrar a ID do Munchkin {#find-your-munchkin-id}

1. Vá para o **Administrador** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clique em **Minha conta**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Permissões de administrador necessárias**

1. Role para baixo até &quot;Informações de suporte&quot; e copie a ID do Munchkin.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Enviar solicitação para TI {#send-request-to-it}

Peça à equipe de TI para configurar o seguinte CNAME: (Substitua a palavra [CNAME] e [Munchkin ID] com o texto da etapa anterior.)

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Concluir configuração CNAME {#complete-cname-setup}

1. Depois que a TI criar o CNAME, acesse o **Administrador** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clique em **Páginas de aterrissagem**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Em **Configurações** seção , clique em **Editar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Insira seu CNAME em **Nome do domínio para páginas de aterrissagem**, insira **Página de fallback**, insira **Página inicial** e clique em **Salvar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Sua página de fallback será a página para a qual os leads serão redirecionados se sua Página de aterrissagem do Marketo não estiver disponível.

Excelente! Suas páginas de aterrissagem agora são marcadas com o domínio de sua empresa.
