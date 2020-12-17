---
unique-page-id: 10617187
description: Noções Gerais das Configurações de Privacidade - Documentos do Marketing - Documentação do Produto
title: Noções Gerais das Configurações de Privacidade
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---


# Noções Gerais das Configurações de Privacidade {#understanding-privacy-settings}

## Visão geral {#overview}

O Marketo fornece aos profissionais de marketing uma maneira de obter o consentimento dos visitantes da Web para rastreá-los. Há duas maneiras de opt out, ou você pode escolher ser rastreado por IP anônimo.

* Os visitantes da Web selecionam o recurso Não rastrear (DNT) em seu navegador (e o profissional de marketing atende à solicitação do visitante da Web para Não rastrear)
* Os visitantes da Web usam um cookie opt out fornecido por um profissional de marketing em um site

Ou o comerciante pode rastrear usuários, mas usar um IP anônimo.

Esses métodos podem afetar o valor e a funcionalidade do Marketo em áreas específicas. No entanto, se o comerciante *não* alterar nada na configuração do Marketo, a funcionalidade do Marketo permanecerá a mesma.

## Configurações do navegador para Não rastrear {#browser-settings-for-do-not-track}

Os visitantes da Web podem definir seu navegador para impedir o rastreamento por qualquer site escolhendo &quot;Não rastrear&quot; (DNT). Isso impede o rastreamento desse navegador e dispositivo em particular. Consulte as configurações de privacidade do navegador para obter detalhes completos.

Em Munchkin, um profissional de marketing pode [decidir se deseja suportar ou ignorar a configuração de DNT do navegador](edit-do-not-track-browser-support-settings.md).

Na Personalização da Web, um comerciante pode decidir se [suporta ou ignorar a configuração DNT do navegador](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## opt out de um site específico {#opt-out-from-a-specific-website}

Você também pode permitir que os visitantes do site opt out o rastreamento do site do seu site, independentemente de as configurações **Navegador não rastrear** estarem ou não configuradas. Isso permite que o visitante do site especifique suas preferências de rastreamento diretamente do site.

Para fazer isso, você deve adicionar um parâmetro a um link de opt out em uma página da Web que tenha o rastreamento de deslocamento ativado. Pode ser qualquer página da Web, mas o link da página da Web deve conter o seguinte parâmetro:

?marketo_opt_out=true

Abaixo estão exemplos de uma página da Web com um link de opção de não participação e uma landing page para depois que o link é clicado. O seu vai variar.

Esta é uma página da Web com um botão com o parâmetro &quot;?marketo_opt_out=true&quot; no link para opção de não participação.

![](assets/opt-out-1.png)

Você pode criar e publicar uma landing page como uma página de acompanhamento para quando seu link com o parâmetro &quot;?marketo_opt_out=true&quot; for clicado.

![](assets/opt-out-2.png)

Quando o link é clicado, o Marketo adiciona um cookie chamado **mkto_opt_out** ao navegador do visitante que desativa o rastreamento Munchkin do visitante do site que clica no link com o parâmetro acima.

Para validar se o cookie pode ser plantado, verifique se você é um cliente potencial cookie e clique no link. Em seguida, verifique os cookies do navegador para verificar se o cookie **mkto_opt_out** foi adicionado.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Atualmente, isso funciona apenas com as versões 152 e posteriores do Munchkin.

## opt in {#opt-in}

Os profissionais de marketing podem permitir que os usuários opt in usando os recursos do Marketo em emails, formulários, landings page e outros métodos.

## Rastreamento usando um IP anônimo {#tracking-using-an-anonymized-ip}

Os profissionais de marketing podem preservar a privacidade rastreando usuários com um endereço IP anônimo. Para fazer isso, adicione este código ao RTP ou Munchkin Javascript que está incorporado ao website.

* Para Munchkin, basta adicionar {&quot;anonimizeIP&quot;,true} à função init.

   >[!NOTE]
   >
   >O uso deste parâmetro requer que Munchkin V2 seja ativado. Para ativá-lo para sua subscrição, entre em contato com [Suporte do Marketing](http://nation.marketo.com/community/support_solutions).

* Para personalização da Web (RTP), adicione isso ao javascript:

anonimizar IP : antes de chamar rtp(&#39;send&#39;,&#39;visualização&#39;); add rtp(&#39;set&#39;, &#39;settings&#39;, {&#39;anonimizeIP&#39; : true});

