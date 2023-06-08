---
unique-page-id: 10617187
description: Noções básicas sobre configurações de privacidade - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre configurações de privacidade
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Noções básicas sobre configurações de privacidade {#understanding-privacy-settings}

## Visão geral {#overview}

O Marketo fornece aos profissionais de marketing uma maneira de obter o consentimento dos visitantes da Web para rastreá-los. Há duas maneiras de recusar o acesso ou você pode optar por ser rastreado por IP anônimo.

* Os visitantes da Web selecionam o recurso Não rastrear (DNT) em seu navegador (e o profissional de marketing atende à solicitação do visitante da Web para Não rastrear)
* Os visitantes da Web usam um cookie de opção de não participação fornecido por um profissional de marketing em um site

Ou o profissional de marketing pode rastrear usuários, mas usar um IP anônimo.

Esses métodos podem afetar o valor e a funcionalidade do Marketo em áreas específicas. No entanto, se o profissional _não_ alterar qualquer item na configuração do Marketo, a funcionalidade do Marketo permanece a mesma.

## Configurações do navegador para Do Not Track {#browser-settings-for-do-not-track}

Os visitantes da Web podem definir seu navegador para impedir o rastreamento por qualquer site, escolhendo &quot;Não rastrear&quot; (DNT). Isso impede o rastreamento desse navegador e dispositivo específico. Consulte as configurações de privacidade do navegador para obter detalhes completos.

Entrada [!DNL Munchkin], um profissional de marketing pode [decidir se oferece suporte ou ignora a configuração DNT do navegador](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Na Personalização da Web, um profissional de marketing pode decidir se deseja [suportar ou ignorar a configuração DNT do navegador](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Recusar de um site específico {#opt-out-from-a-specific-website}

Você também pode permitir que os visitantes do site recusem o rastreamento do site, independentemente de fazer ou não o rastreamento **Navegador Não Rastrear** são definidas. Isso permite que o visitante do site especifique suas preferências de rastreamento diretamente do seu site.

Para fazer isso, você deve adicionar um parâmetro a um link de opt out em uma página da Web que tenha [!DNL Munchkin] rastreamento ativado. Pode ser qualquer página da Web, mas o link da página da Web deve conter o seguinte parâmetro:

?marketo_opt_out=true

Abaixo estão exemplos de uma página da Web com um link para opção de não participação e uma página de aterrissagem para depois que o link for clicado. O seu vai variar.

Esta é uma página da Web com um botão com o parâmetro &quot;?marketo_opt_out=true&quot; no link para opção de não participação.

![](assets/understanding-privacy-settings-1.png)

Você pode criar e publicar uma landing page como uma página de acompanhamento para quando seu link com o parâmetro &quot;?marketo_opt_out=true&quot; for clicado.

![](assets/understanding-privacy-settings-2.png)

Quando o link é clicado, o Marketo adiciona um cookie chamado **mkto_opt_out** ao navegador do visitante que desativa o [!DNL Munchkin] para o visitante do site que clica no link com o parâmetro acima.

Para validar se o cookie pode ser plantado, verifique se você é um cliente potencial com cookie e clique no link. Em seguida, verifique os cookies do navegador para verificar se **mkto_opt_out** cookie foi adicionado.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Atualmente, funciona somente com o [!DNL Munchkin] versões 152 e posteriores.

## Aceitar {#opt-in}

Os profissionais de marketing podem permitir que os usuários aceitem usar os recursos do Marketo em emails, formulários, páginas de aterrissagem e outros métodos.

## Rastreamento usando um IP anônimo {#tracking-using-an-anonymized-ip}

Os profissionais de marketing podem preservar a privacidade rastreando usuários com um endereço IP anônimo. Para fazer isso, adicione este código ao RTP ou [!DNL Munchkin] Javascript incorporado ao site.

* Para [!DNL Munchkin], adicione {&quot;anonymizeIP&quot;,true} à função init.

  >[!NOTE]
  >
  >O uso deste parâmetro exige que [!DNL Munchkin] V2 ser habilitada. Para ativá-la para sua assinatura, entre em contato com [Suporte ao Marketo](https://nation.marketo.com/community/support_solutions).

* Para Personalização da Web (RTP), adicione isso ao javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
