---
unique-page-id: 2360189
description: Personalizar os URLs da sua página de aterrissagem com um CNAME (Administração) - Documentação do Marketo - Documentação do produto
title: Personalizar os URLs da sua landing page com um CNAME (Administração)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 3%

---

# Personalizar os URLs da sua landing page com um CNAME  {#customize-your-landing-page-urls-with-a-cname}

Embora o Marketo hospede suas páginas de aterrissagem, o URL deve ser personalizado para sua empresa.

>[!NOTE]
>
>Sem CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME com marca:
>
>https://go.**Sua empresa**.com/UnsuscribePage.html

>[!NOTE]
>
>**Permissões de administrador necessárias**

Vamos definir suas configurações!

1. Escolha um CNAME.

   É a parte frontal da URL. Exemplos:

   * **ir**.YourCompany.com/NameOfPage.html
   * **informações**.YourCompany.com/NameOfPage.html
   * **páginas**.YourCompany.com/NameOfPage.html

   A palavra (mais YourCompany.com) é chamada de CNAME. Você precisará disso mais tarde, então anote-o.

1. Encontre sua sequência de caracteres da conta.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clique em **[!UICONTROL Landing Pages]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. No **[!UICONTROL Landing Pages]** , copie a sequência de caracteres da conta na seção Configurações.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. Você também precisará disso mais tarde. Anote-o.

1. Envie a solicitação para a TI.

1. Peça à sua equipe de TI para configurar o seguinte CNAME (substitua a palavra [CNAME] e [SEQUÊNCIA DE CARACTERES DA CONTA] com o texto da etapa anterior):

   [CNAME].YourCompany.com > [SEQUÊNCIA DE CARACTERES DA CONTA].mktoweb.com

1. Conclua a configuração de CNAME.

1. Depois que o departamento de TI criar o CNAME, volte para a **[!UICONTROL Admin]** área.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clique em **[!UICONTROL Landing Pages]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. No **[!UICONTROL Configurações]** clique em **[!UICONTROL Editar]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Insira seu CNAME em **[!UICONTROL Nome de domínio para landing pages]**, insira seu **[!UICONTROL Página de fallback]**, insira seu **[!UICONTROL Página inicial]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

Sua página de fallback é o local para onde as pessoas serão redirecionadas se a sua página de aterrissagem do Marketo não estiver disponível.

Excelente! As páginas de aterrissagem agora são marcadas com o domínio da empresa.
