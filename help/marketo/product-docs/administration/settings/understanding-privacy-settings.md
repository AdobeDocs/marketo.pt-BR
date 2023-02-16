---
unique-page-id: 10617187
description: Noções básicas sobre configurações de privacidade - Documentos do Marketo - Documentação do produto
title: Noções básicas sobre configurações de privacidade
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
source-git-commit: bd6f049d5959356a99314e81bb6cfe517c2efdfa
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Noções básicas sobre configurações de privacidade {#understanding-privacy-settings}

## Visão geral {#overview}

O Marketo fornece aos profissionais de marketing uma maneira de obter o consentimento dos visitantes da Web para rastreá-los. Há duas maneiras de rejeitar, ou você pode optar por ser rastreado por IP anônimo.

* Os visitantes da Web selecionam o recurso Não rastrear (DNT) em seu navegador (e o profissional de marketing atende à solicitação do visitante da Web para não rastrear)
* Os visitantes da Web usam um cookie de opção fornecido por um profissional de marketing em um site

Ou o profissional de marketing pode rastrear usuários, mas usar um IP anônimo.

Esses métodos podem afetar o valor e a funcionalidade da Marketo em áreas específicas. No entanto, se o profissional de marketing *does not* altere qualquer coisa na configuração do Marketo, a funcionalidade do Marketo permanece a mesma.

## Configurações do navegador para Não rastrear {#browser-settings-for-do-not-track}

Os visitantes da Web podem definir seu navegador para impedir o rastreamento por qualquer site escolhendo &quot;Não rastrear&quot; (DNT). Isso impede o rastreamento desse navegador e dispositivo específico. Consulte as configurações de privacidade do navegador para obter detalhes completos.

Em Munchkin, um profissional de marketing pode [decidir se suporta ou ignora a configuração DNT do navegador](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Na personalização da Web, um profissional de marketing pode decidir se deseja [suportar ou ignorar a configuração de DNT do navegador](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Recusar de um site específico {#opt-out-from-a-specific-website}

Também é possível permitir que os visitantes do site optem por não participar do rastreamento por site, independentemente de a atividade ser ou não realizada **Navegador não rastreia** são configuradas. Isso permite que o visitante do site especifique suas preferências de rastreamento diretamente do site.

Para fazer isso, você deve adicionar um parâmetro a um link para opção de não participação em uma página da Web que tenha o rastreamento de cliques ativado. Pode ser qualquer página da Web, mas o link da página da Web deve conter o seguinte parâmetro:

?marketo_opt_out=true

Abaixo estão exemplos de uma página da Web com um link para opção de não participação e uma página de aterrissagem para depois que o link é clicado. O seu vai variar.

Aqui está uma página da Web com um botão com o parâmetro &quot;?marketo_opt_out=true&quot; no link para opção de não participação.

![](assets/understanding-privacy-settings-1.png)

Você pode criar e publicar uma landing page como uma página de acompanhamento de quando clicar no link com o parâmetro &quot;?marketo_opt_out=true&quot;.

![](assets/understanding-privacy-settings-2.png)

Quando o link é clicado, o Marketo adiciona um cookie chamado **mkto_opt_out** para o navegador do visitante que desativa o rastreamento do Munchkin para o visitante do site que clica no link com o parâmetro acima.

Para validar se o cookie pode ser plantado, verifique se você é um lead cookie e clique no link . Em seguida, verifique os cookies do navegador para verificar se a variável **mkto_opt_out** foi adicionado.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Atualmente, isso funciona somente com as versões 152 e superior do Munchkin.

## Aceitar {#opt-in}

Os profissionais de marketing podem permitir que os usuários incluam recursos da Marketo em emails, formulários, landing pages e outros métodos.

## Rastreamento usando um IP anônimo {#tracking-using-an-anonymized-ip}

Os profissionais de marketing podem preservar a privacidade rastreando usuários com um endereço IP anônimo. Para fazer isso, adicione esse código ao Javascript RTP ou Munchkin incorporado no site.

* Para o Munchkin, basta adicionar {&quot;anonymizeIP&quot;,true} à função init.

   >[!NOTE]
   >
   >O uso desse parâmetro requer que o Munchkin V2 seja habilitado. Para habilitá-lo para sua assinatura, entre em contato com [Suporte Marketo](https://nation.marketo.com/community/support_solutions).

* Para Personalização da Web (RTP), adicione isso ao javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
