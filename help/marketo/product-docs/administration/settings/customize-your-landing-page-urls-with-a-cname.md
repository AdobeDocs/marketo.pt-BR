---
unique-page-id: 2360189
description: Personalize os URLs de sua página de aterrissagem com um CNAME (Administração) - Documentos do Marketo - Documentação do produto
title: Personalize os URLs de página de aterrissagem com um CNAME (Administração)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 3%

---

# Personalize seus URLs de página inicial com um CNAME  {#customize-your-landing-page-urls-with-a-cname}

Mesmo que o Marketo hospede suas landing pages, o URL deve ser personalizado para sua empresa.

>[!NOTE]
>
>Sem CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME de marca:
>
>https://go.**Sua empresa**.com/UnsuscribePage.html

>[!NOTE]
>
>**Permissões de administrador necessárias**

Vamos definir suas configurações!

1. Escolha um CNAME.

   É a parte frontal do URL. Exemplos:

   * **go**.YourCompany.com/NameOfPage.html
   * **informações**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.html

   A única palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, portanto anote isso.

1. Encontre sua sequência de caracteres da conta.

1. Vá para o **Administrador** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clique em **Páginas de aterrissagem**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. Em **Páginas de aterrissagem** , copie a Sequência de caracteres da conta na seção Configurações .

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. Você também precisará disso mais tarde, portanto anote isso.

1. Enviar solicitação para TI.

1. Solicite que sua equipe de TI configure o seguinte CNAME (substitua a palavra [CNAME] e [STRING DE CONTA] com o texto da etapa anterior):

   [CNAME].YourCompany.com > [STRING DE CONTA].mktoweb.com

1. Conclua a configuração CNAME.

1. Depois que a TI criar o CNAME, volte para a **Administrador** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clique em **Páginas de aterrissagem**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Em **Configurações** seção , clique em **Editar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Insira seu CNAME em **Nome do domínio para páginas de aterrissagem**, insira **Página de fallback**, insira **Página inicial** e clique em **Salvar**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

Sua página de fallback é onde as pessoas serão redirecionadas se a página de aterrissagem do Marketo não estiver disponível.

Excelente! Suas páginas de aterrissagem agora são marcadas com o domínio de sua empresa.
