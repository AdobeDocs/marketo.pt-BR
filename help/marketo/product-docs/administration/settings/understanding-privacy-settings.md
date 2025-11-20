---
unique-page-id: 10617187
description: Noções básicas sobre configurações de privacidade - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre configurações de privacidade
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: eccf4a66f5d3c581a82a363918b40ae37aa73576
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Noções básicas sobre configurações de privacidade {#understanding-privacy-settings}

## Visão geral {#overview}

O Marketo fornece aos profissionais de marketing uma maneira de obter o consentimento dos visitantes da Web para rastreá-los. Há duas maneiras de recusar o acesso ou você pode optar por ser rastreado por IP anônimo.

* Os visitantes da Web selecionam o recurso Não rastrear (DNT) em seu navegador (e o profissional de marketing atende à solicitação do visitante da Web para Não rastrear)
* Os visitantes da Web usam um cookie de opção de não participação fornecido por um profissional de marketing em um site

Ou o profissional de marketing pode rastrear usuários, mas usar um IP anônimo.

Esses métodos podem afetar o valor e a funcionalidade do Marketo em áreas específicas. No entanto, se o profissional de marketing _não_ alterar nada na configuração do Marketo, a funcionalidade do Marketo permanecerá a mesma.

## Configurações do navegador para Do Not Track {#browser-settings-for-do-not-track}

Os visitantes da Web podem definir seu navegador para impedir o rastreamento por qualquer site, escolhendo &quot;Não rastrear&quot; (DNT). Isso impede o rastreamento desse navegador e dispositivo específico. Consulte as configurações de privacidade do navegador para obter detalhes completos.

Em [!DNL Munchkin], um profissional de marketing pode [decidir se oferece suporte ou ignora a configuração de DNT do navegador](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

No Web Personalization, um profissional de marketing pode decidir se [oferece suporte ou ignora a configuração de DNT do navegador](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Recusar de um site específico {#opt-out-from-a-specific-website}

Você também pode permitir que os visitantes do site recusem o rastreamento do seu site, independentemente de as configurações do **Navegador não rastrear** estarem definidas ou não. Isso permite que o visitante do site especifique suas preferências de rastreamento diretamente do seu site.

Para fazer isso, você deve adicionar um parâmetro a um link para opção de não participação em uma página da Web com o rastreamento de [!DNL Munchkin] habilitado. Pode ser qualquer página da Web, mas o link da página da Web deve conter o seguinte parâmetro:

?marketo_opt_out=true

Abaixo estão exemplos de uma página da Web com um link para opção de não participação e uma página de aterrissagem para depois que o link for clicado. O seu vai variar.

Esta é uma página da Web com um botão com o parâmetro &quot;?marketo_opt_out=true&quot; no link para opção de não participação.

![](assets/understanding-privacy-settings-1.png)

Você pode criar e publicar uma landing page como uma página de acompanhamento para quando seu link com o parâmetro &quot;?marketo_opt_out=true&quot; for clicado.

![](assets/understanding-privacy-settings-2.png)

Quando o link é clicado, o Marketo adiciona um cookie chamado **mkto_opt_out** ao navegador do visitante que desativa o rastreamento [!DNL Munchkin] para o visitante do site que clica no link com o parâmetro acima.

Para validar se o cookie pode ser plantado, verifique se você é um cliente potencial com cookie e clique no link. Em seguida, verifique os cookies do navegador para confirmar se o cookie **mkto_opt_out** foi adicionado.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Atualmente, isso funciona somente com [!DNL Munchkin] versões 152 e superiores.

## Aceitar {#opt-in}

Os profissionais de marketing podem permitir que os usuários aceitem usar os recursos do Marketo em emails, formulários, páginas de aterrissagem e outros métodos.

## Rastreamento usando um IP anônimo {#tracking-using-an-anonymized-ip}

Os profissionais de marketing podem preservar a privacidade rastreando usuários com um endereço IP anônimo. Para fazer isso, adicione este código ao RTP ou Javascript [!DNL Munchkin] que está incorporado no site.

* Para [!DNL Munchkin], adicione `{"anonymizeIP",true}` à [função de inicialização](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/configuration){target="_blank"}.

* Para o Web Personalization (RTP), adicione isso ao javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
